---
title: Nieuwe commerciële promoties
ms.topic: article
ms.date: 09/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over nieuwe commerce-ervaringen voor het detecteren en kopen van promoties.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 45411827f200f205dc20b9a9c2d60519d4aba4eb
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/29/2021
ms.locfileid: "129249307"
---
# <a name="introduction-new-commerce-promotions"></a>Inleiding: Nieuwe commerciële promoties

**Juiste rollen**

- Beheeragent
- Verkoopagent
- Globale beheerder

> [!Note] 
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technical preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Microsoft biedt ondersteuning voor promoties in nieuwe handel. Deze promoties hebben verschillende kortingsbedragen en -duur. 

## <a name="discovering-promotions"></a>Promoties detecteren ##

Partners kunnen promoties ontdekken door de achterstand van promoties te bezoeken of door de getPromotions-API aan te roepen. De achterstand bij promoties is een Microsoft-lijst met beschikbare promoties die partners moeten kennen. De lijst wordt maandelijks opeengepdatet en bijgewerkt. 


## <a name="operationalize-promotions"></a>Niveaupromoties operationeel maken ##

Partners kunnen de promoties operationeel maken door de [getPromotions-API te implementeren.](/partner-center/develop/get-promotions) Deze API retourneert alle promoties die bestaan voor een bepaalde markt (het land van de klant) en het segment. De API retourneert de lijst met promoties en belangrijke informatie om de partner te helpen begrijpen welke promoties beschikbaar zijn voor klanten in verschillende landen. 


De getPromotions-API bevat de volgende gegevens voor een bepaalde promotie:

- Duur van de promotie
- Het kortingspercentage voor de promotie
- De producten en SKU's voor welke promotie beschikbaar is

Promoties worden toegepast door het partnercentrum wanneer de partner de product-SKU koopt waarop de promotie beschikbaar is. Partneracties zijn beschikbaar in de gebruikersinterface van de partnercentrumcatalogus in de product-SKU-details. Ze kunnen klikken op De details van de promotie weergeven voor meer informatie over de promotie. De mogelijkheid om de promotiedetails weer te geven, is toegankelijk via de SKU-details op de cataloguspagina, de beoordelingspagina voorafgaand aan het indienen van de aankoop, de bevestiging nadat de order is verzonden en de pagina ordergeschiedenis. 

## <a name="verify-eligibility"></a>Geschiktheid controleren ##

Partners kunnen bekijken of een klantaankoop in aanmerking komt voor een promotie door de informatie te bekijken op de beoordelingspagina in het partnercentrum voordat ze het product kopen. Partners kunnen ook de [verifyPromotionEligibility-API aanroepen,](/partner-center/develop/verify-promotion-eligibility)door de tenant-id van de klant en de promotie-id door te geven. De aanroep retourneert true als de klant in aanmerking komt. Als de klant niet in aanmerking komt, retourneert de API de voorwaarden die niet zijn voldaan om de promotie van toepassing te laten zijn. 

Partners kunnen controleren of ze in aanmerking komen aanroepen en resultaten terug krijgen. Geschiktheidsfouten kunnen worden gebaseerd op het aantal seats, incompatibele voorwaarden of limieten voor het aantal keren dat een promotie kan worden toegepast op de product-SKU van een klant.

Belangrijke onderwerpen voor api's voor nieuwe commercepromoties:

- [GetPromotions-API](/partner-center/develop/get-promotions)
- [GetPromotionsById-API](/partner-center/develop/get-promotion-by-id)
- [VerifyPromtionEligibilities](/partner-center/develop/verify-promotion-eligibility)
- [Resources voor promoties](/partner-center/develop/promotion-resources)

>[!IMPORTANT]
> Partners moeten promoties controleren voordat ze een transactie indienen. Op de Partner Center  controlepagina als partners geen promotie zien, wordt deze niet toegepast op de transactie. De partner krijgt de prijs voor niet-promotie. Partners kunnen ook de API voor winkelwagenlijnitem bekijken om te zien of de promotie aanwezig is voordat ze een transactie indienen. Partners kunnen de API voor verificatiepromoties aanroepen voordat ze transacties verzenden om te controleren of de combinatie van klantproduct-SKU in aanmerking komt voor de promotie en zo niet, de redenen voor ineligibility.

Er zijn drie redenen waarom een klant mogelijk niet in aanmerking komt voor een promotie. Deze niet-in aanmerking komende typen worden geretourneerd in de API voor validatiepromotie in gevallen waarin de klant niet in aanmerking komt.

### <a name="seat-count"></a>Aantal seat ###

Veel promoties hebben een seat van maximaal 2400 seats. In dergelijke gevallen wordt een transactie met meer dan 2400 ingediend tegen de niet-promotieprijzen. Deze aantal plaatsen worden ook afgedwongen bij het toevoegen van seats aan een promotieabonnement met deze limieten. Partners krijgen een foutmelding als ze proberen een abonnement met promotielimieten te verhogen. De limieten voor plaatsen van promoties worden afgedwongen tussen partners, dus als een partner een promotie van 2300 seats met een limiet voor het aantal plaatsen voor promotie koopt, krijgt een tweede partner die 200 seats koopt, de abonnementsprijs tegen de prijs voor niet-promotie. Niveaupromotie wordt afgedwongen op het niveau van de product-SKU dat de partner afbeeert, zodat een partner promotieprijzen kan krijgen voor 2400 seats van Microsoft 365 E3 en voor een andere product-SKU-Microsoft 365 E5. Partners kunnen de [API subscribedSKUs](/partner-center/develop/get-a-list-of-available-licenses) aanroepen om te zien hoeveel licenties een klant heeft voor een bepaalde inrichtende SKU.

Als een partner meer licenties wil dan de 2400 seats en de promotie wil, kan de partner gewoon één abonnement aanschaffen tot de limiet van 2400 tegen de promotieprijs en een tweede abonnement tegen de prijs die niet is gepromotieed.

### <a name="term"></a>Termijn ###

Termenbeperkingen definiëren welke product-SKU-voorwaarden zijn afgestemd op een bepaalde promotie. Voor veel promoties zijn verschillende kortingen gedefinieerd op basis van de termijn. Als een partner een transactie indient en de termijn niet in overeenstemming is met de promotie, verwachten ze dat de transactie de niet-promotieprijs heeft die ze verwachten. Voorbeelden van voorwaarden *zijn jaarlijks* *of maandelijks.*

### <a name="first-purchase"></a>Eerste aankoop ###

Sommige promoties dwingen af dat ze slechts één keer worden verkregen. Een partner ziet de geschiktheid onwaar *met behulp* van de API voor valideren van geschiktheid met het fouttype *FirstPurchase*. Een partner kan nog steeds de opgegeven product-SKU kopen, maar het abonnement heeft de prijs voor niet-promotie. Deze beperking geldt per klant, niet per partner. Zodra een klant een promotie met deze regel heeft, kan er geen tweede exemplaar van de promotie worden toegepast door een tweede partner.

## <a name="promotions-and-renewals"></a>Promoties en verlengingen ##

Aanbiedingskortingen die worden toegepast, gelden voor de duur van de aankoop. Abonnementen met toegepaste promoties behouden de actieprijs als de verlengingsdatum binnen het datumbereik van de promotieduur valt. Verlengingen buiten het datumbereik van de promotieduur worden verlengd tot de prijs die niet is gepromotie (in de lijst met prijzen). Partners kunnen de verlengingsstatus bijhouden voor de prijspunten op de pagina met abonnementsgegevens en op de instructies voor gegevensvernieuwing voor getSubscription.

## <a name="promotions-and-upgrades"></a>Promoties en upgrades ##
Partners die upgraden van een abonnement naar een andere SKU laten de promotieprijs achter. Deze actie treedt op omdat de promotie is geconfigureerd voor de SKU die ze verlaten wanneer ze upgraden naar een andere SKU. Partners die upgraden naar een SKU die mogelijk een promotie heeft, krijgen niet automatisch de promotieprijs. Als ze de promotieprijs nodig hebben of willen hebben voor de SKU waar ze naar willen gaan, moeten ze de nieuwe SKU handmatig aanschaffen als een nieuw abonnement. Momenteel worden promoties alleen toegepast op nieuwe abonnementen en verlengingen.

## <a name="promotions-and-migrations"></a>Promoties en migraties ##
Partners kunnen de abonnementen van hun klanten migreren van traditionele Microsoft 365/Dynamics 365 naar nieuwe commerce-versies van hun abonnementen. De migraties zijn beschikbaar via de Partner Center gebruikersinterface of vanuit het aanroepen van de migratie-API's. Partners die migreren van een traditioneel abonnement naar nieuwe commerce, krijgen de promotie wanneer ze migreren, zolang de product-SKU die ze verplaatsen, in overeenstemming is met de promotiedefinitie. Partners moeten de API voor geschiktheid controleren aanroepen om ervoor te zorgen dat de doelproduct-SKU de promotieprijs vóór de migratie zal toepassen.

## <a name="cross-channel-considerations"></a>Overwegingen voor kruiskanaal ##
Cloud Solution Provider (CSP) promotielimieten en -beperkingen worden niet afgedwongen voor alle kanalen, zoals Enterprise Agreement (EA). Een CSP-partner kan een promotie verkrijgen met een beperking van 2400 promotie, zelfs wanneer de klant mogelijk 3000 seats van EA heeft.  

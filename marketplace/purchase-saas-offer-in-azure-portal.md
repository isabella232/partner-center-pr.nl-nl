---
title: Een SaaS-aanbieding kopen in Azure Portal
description: Meer informatie over het zoeken en kopen van een SaaS-aanbieding in Azure Portal.
author: mingshen-ms
ms.author: mingshen
ms.reviewer: dannyevers
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: how-to
ms.date: 06/29/2021
ms.openlocfilehash: 5c5c1565f8e1f2703e82bd75881e9920a1fc71d611d78ef282f771cfb30fcd00
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115688366"
---
# <a name="purchase-a-saas-offer-in-azure-portal"></a>Een SaaS-aanbieding kopen in Azure Portal

In dit artikel worden de verschillende opties en vereisten beschreven voor het zoeken, proberen en kopen van een SaaS-aanbieding (Software-as-a-Service) van de Azure Portal.

## <a name="create-a-saas-subscription"></a>Een SaaS-abonnement maken

Als u een SaaS-abonnement wilt kopen, hebt u een Azure-gebruikersaccount nodig met toegang tot een geschikt Azure-abonnement. Dit abonnement wordt gebruikt voor facturering en voor compartimentering van uw aangeschafte cloudbronnen. Zie Een extra Azure-abonnement maken voor meer informatie [over Azure-abonnementen.](/azure/cost-management-billing/manage/create-subscription)

Selecteer in Azure Portal de gewenste SaaS-aanbieding in de **sectie Marketplace.**

Een Software-as-a-Service-abonnement biedt het recht om een service voor een bepaalde periode te gebruiken via een online abonnement in plaats van lokale installatie op afzonderlijke computers. Een abonnement is een overeenkomst voor het gebruik van een of meer cloudplatforms of -services, waarvoor kosten in rekening worden gebracht op basis van licentiekosten per gebruiker of op basis van resourceverbruik in de cloud. Een organisatie kan meerdere SaaS-abonnementen hebben.

Beperkingen voor SaaS-abonnementen zijn onder andere:

- Geen studentabonnementen.
- Geen Visual Studio Enterprise-abonnement.
- Geen gratis tegoedabonnementen.
- Voor betaalde aanbiedingen is een betaalmiddel vereist.

## <a name="saas-offers-discovery-in-azure-portal"></a>SaaS biedt detectie in Azure Portal

Zodra u zich in Azure Portal, zijn er een aantal manieren om uw zoekopdracht te beperken om u te richten op SaaS-aanbiedingen.

### <a name="narrowing-your-search"></a>Uw zoekopdracht beperken

Selecteer op de startpagina onder **Azure-services** **de optie + Een resource maken** of **Marketplace.** Of gebruik de snelkoppeling **G + N** overal in het platform.

- Verklein de resultaten tot SaaS-aanbiedingen met behulp van het filter **Aanbiedingstype** en selecteer **vervolgens SaaS.**
- Gebruik de algemene zoekopdracht bovenste navigatiebalk om een specifieke SaaS-aanbieding te vinden.

Zoek een [privé-SaaS-aanbieding door](./private-offers.md) de banner boven aan de **marketplace-startpagina te** selecteren. Niet alle aanbiedingen of abonnementen zijn beschikbaar in alle geografische gebieden en sommige worden mogelijk alleen weergegeven voor bepaalde tenants.

De gefilterde weergave toont elke beschikbare SaaS-aanbieding die wordt vertegenwoordigd door een titel. Selecteer er een om de pagina met productdetails weer te geven. Deze bevat de volgende secties:

- Overzicht: details over de service, marketing en het leermateriaal
- Abonnementen en prijzen: elke aanbieding bevat ten minste één abonnement met verschillende factureringsvoorwaarden en -prijzen
- Gebruiksgegevens en ondersteuning: omvat Publisher id, aanbiedings-id en abonnements-id
- Beoordeling en beoordelingen van de specifieke SaaS-aanbieding

## <a name="available-billing-models-plansskus-for-saas-offers"></a>Beschikbare factureringsmodellen (abonnementen/SKU's) voor SaaS-aanbiedingen

Elke SaaS-aanbieding heeft een of meer plannen. Aan elke aanbieding is een prijsmodel gekoppeld: vast tarief of per gebruiker. Elke abonnementsprijs is terugkerende kosten, die nul dollar kunnen zijn (alle vermelde prijzen zijn alleen bedoeld voor voorbeelddoeleinden en zijn niet bedoeld om de werkelijke kosten weer te geven). Deze kosten zijn vast tarief of prijs per gebruiker. Beschikbare typen abonnementen:

- **Maandelijkse abonnementen:** terugkerende maandelijkse kosten; vast of per gebruiker, maandelijkse kosten die worden betaald op basis van een maandelijks terugkeerpatroon. Wanneer de termijn is beëindigd, wordt het plan automatisch vernieuwd.
- **Jaarlijkse abonnementen:** terugkerende jaarlijkse kosten; vaste of jaarlijkse kosten per gebruiker die worden betaald op basis van een jaarlijks terugkeerpatroon. Wanneer de termijn is beëindigd, wordt het plan automatisch vernieuwd.
- **Aangepaste meters:** naast de terugkerende kosten kan een vast tariefplan ook optionele aangepaste dimensies met een meter bevatten voor het uitvalgebruik dat niet is opgenomen in het vast tarief. Elke dimensie vertegenwoordigt een factureerbare eenheid. Dit zijn variabele kosten die veranderen op basis van het gebruik van gemeten eenheden, zoals: bandbreedte, tickets of verwerkte e-mail. Er worden maandelijks kosten in rekening gebracht op basis van uw verbruik van deze dimensies. Houd er rekening mee dat het uitvalverbruik alleen begint wanneer u alle eenheden naar gebruik hebt gebruikt die zijn opgenomen in het vast tarief.
- **Gratis proefversie:** in sommige gevallen bevat het abonnement een proefperiode van één maand, waarin u de software gratis kunt gebruiken.  Zodra de proefperiode is afgelopen, worden er kosten in rekening gebracht op basis van uw abonnement. Proefaanbiedingen zijn niet compatibel met aangepaste meters.

Deze prijsmodellen zijn beschikbaar voor openbare en persoonlijke abonnementen.

## <a name="saas-purchase-experience"></a>SaaS-aankoopervaring

1. Selecteer op de productpagina een plan dat aan uw behoeften voldoet en ga door **met instellen en abonneren**
2. Als onderdeel van het aankoopproces wordt u  omgeleid naar het tabblad Basisinformatie en moet u het volgende doen:
    1. *Definieer* welk abonnement u wilt gebruiken voor facturering. Voor het Azure-abonnement dat u gebruikt, moet een geldige aankoopmethode zijn gedefinieerd. U moet het juiste machtigingsniveau hebben of een resourcegroep onder dat abonnement hebben met het juiste machtigingsniveau. Het land van facturering moet ook een land zijn waar de aanbieding kan worden gekocht. Azure-abonnementen zonder geldige betalingswijze (bijvoorbeeld een MSDN-abonnement) kunnen alleen worden gebruikt om gratis abonnementen te kopen
    1. Kies of maak een **resourcegroep waarvan* de SaaS-resource deel zal uitmaken.
    1. Typ een *naam voor* het SaaS-abonnement om dit later gemakkelijk te identificeren. Na aanschaf kunt u de naam niet meer wijzigen.
    1. Onder **Plan** ziet u het abonnement dat u hebt geselecteerd op de pagina met productdetails (PDP). Als u nog geen actieve selectie hebt gemaakt in de PDP, ziet u het standaardplan. U kunt uw selectie wijzigen door de koppeling **Plan wijzigen te** selecteren. Selecteer de relevante factureringsperiode en kies vervolgens een ander abonnement. Mogelijk kunt u het plan na de aankoop wijzigen als de uitgever dit ondersteunt. U kunt de termijn echter niet wijzigen van maandelijks in jaarlijks of van jaarlijks in maandelijks.
    1. Als het prijsmodel per gebruiker *is,* moet u mogelijk het aantal gebruikers *opgeven.* De prijs die u ziet, wordt gewijzigd op basis van het abonnement, het abonnement en de periode die u hebt geselecteerd.
3. Ga door **naar het** tabblad *Tags: tags* zijn door de gebruiker gedefinieerde sleutel-waardeparen, die rechtstreeks op een resource of resourcegroep kunnen worden geplaatst. U kunt tags gebruiken om uw SaaS-resource later gemakkelijk te vinden. Azure ondersteunt momenteel maximaal 50 tags per resource en resourcegroep. Tags kunnen worden geplaatst op een resource op het moment dat deze wordt gemaakt of worden toegevoegd aan een bestaande resource.
4. Ga door **naar Beoordelen en abonneren om** de details van de aanbieding en het abonnement te bekijken.
    1. Bekijk *Gebruiksrechtovereenkomst,* *wijzigingen* en *privacybeleid van* de uitgever en ook voor Azure Marketplace
    1. U wordt mogelijk gevraagd om uw contactgegevens toe te voegen
    1. *Basisbeginselen* en *tags bekijken*
5. Selecteer na bevestiging **Abonneren.**

## <a name="saas-subscription-and-configuration"></a>SaaS-abonnement en -configuratie

Wanneer u Abonneren selecteert, wordt het bericht 'Uw SaaS-abonnement wordt uitgevoerd' weergegeven. Dit proces duurt enkele minuten. Sluit het venster pas als het is voltooid.

Zodra het abonnement is voltooid, wordt er een bericht weergegeven dat uw SaaS-abonnement is voltooid en moet u het account configureren om van uw aankoop te profiteren. U ontvangt ook een e-mailbericht waarin u wordt gevraagd het nieuwe abonnement te activeren. Als u niet degene bent die het SaaS-account gaat configureren, moet u dit e-mailbericht doorsturen naar de relevante persoon.

Als u het proces wilt voltooien en de SaaS wilt gaan gebruiken, moet u beginnen met het configureren van uw abonnement. Als u de **knop Account nu configureren** selecteert, wordt u omgeleid naar de website van de uitgever.

U kunt ook de status van uw abonnement controleren door in de rechterbovenhoek van de koptekst het belpictogram te selecteren.

Als u het configuratieproces niet binnen *30* dagen voltooit, wordt dit SaaS-abonnement *automatisch verwijderd.* De facturering begint nadat uw account is geconfigureerd op de website van de uitgever.

Foutberichten die u tijdens het proces tegenkomt:

- De *abonnementsnaam van het geselecteerde abonnement kan* niet worden gekocht in een gratis abonnement
  - Upgrade uw account. Zie https://aka.ms/UpgradeFreeSub voor meer informatie.

- De aankoop is mislukt omdat er geen geldige creditcard is gevonden en er geen betalingswijze is gekoppeld aan uw Azure-abonnement.
  - Gebruik een ander Azure-abonnement of voeg de huidige creditcard of betalingswijze toe voor dit abonnement en doe het opnieuw.

- De *abonnementsnaam van het abonnement dat* door de uitgever van de aanbieding is geselecteerd, is niet beschikbaar voor aankoop volgens de regels die zijn ingesteld door uw IT-beheerder.  
  - Neem contact op met uw IT-beheerder.

- De *abonnementsnaam van het abonnement* dat is geselecteerd door de uitgever van de aanbieding, is niet beschikbaar voor aankoop vanwege de privé-marketplace-instellingen die zijn gemaakt door de IT-beheerder van uw tenant.  
  - Neem contact op met uw IT-beheerder

- De aankoop is mislukt omdat de aangevraagde factureringsperiode leeg of ongeldig is.
  - Probeer een ander abonnement/andere factureringsperiode aan te schaffen.

- De aankoop is mislukt omdat de ondertekening van de juridische overeenkomst niet kan worden geverifieerd.
  - Opnieuw. Als de fout zich blijft voordoen, probeert u de aankoop te doen met een ander Azure-abonnement of kunt u contact opnemen met de ondersteuning.

- De aankoop van *offerID by* publisher *publisherID* is mislukt. Deze aanbieding is momenteel niet beschikbaar voor aankoop.
  - Probeer het later opnieuw. Als u na een uur dit foutbericht blijft ontvangen, neem dan contact op met de ondersteuning.  

- De aankoop van plan *planID* van *offerID* van aanbieding door uitgever *publisherID* is mislukt. Dit abonnement is momenteel niet beschikbaar voor aankoop.
  - Probeer het later opnieuw. Als u na een uur dit foutbericht blijft ontvangen, neem dan contact op met de ondersteuning. 

- Het *e-mailadres van de* client met object-id *ObjectID* is niet autorisatie om de actie *DeploymentValidationAction* uit te voeren via scope *ResourceGroup; DeploymentScope* of het bereik is ongeldig.  
  - U krijgt dit bericht als u niet de juiste machtigingen hebt voor het Azure-abonnement/de resourcegroep.  
    Als er onlangs toegang is verleend, vernieuwt u uw referenties.  
    Als u resources wilt implementeren in een resourcegroep, moet u ten minste inzenderstoegang hebben. Controleer uw toegangsstatus onder **Resourcegroepen** en klik **Access Control.** Hier ziet u wie de 'eigenaar' is, die u kunt vragen om u toe te wijzen als 'Inzender'.

- Het abonnement dat voor deze aankoop wordt gebruikt, staat geen Marketplace-aankopen toe.  
  - Gebruik een ander abonnement of vraag uw beheerder om de definitie voor dit abonnement te wijzigen en het opnieuw te proberen.

## <a name="next-steps"></a>Volgende stappen

- Als u al een aanbieding hebt aangeschaft in marketplace, gaat u naar [Facturering en facturering](./billing-invoicing.md)
- U vindt hier ook meer informatie over [opties voor persoonlijke](./private-offers.md) abonnementen.
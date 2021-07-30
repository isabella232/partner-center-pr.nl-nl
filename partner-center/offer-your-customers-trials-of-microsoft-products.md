---
title: Klanten proefversies van Microsoft-producten aanbieden
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Laat klanten microsoft-abonnementsproducten 30 dagen uitproberen. Meld u aan voor deze gratis proefversies in de catalogus, net zoals veel andere onlineservices.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 393bd70096ba3cd7d1c9889d5b521cc94a389d90
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114845972"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Klanten 30 dagen gratis proefversies van Microsoft-producten geven

**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Verkoopagent

Een goede manier om klanten kennis te laten maken met nieuwe Microsoft-producten is het aanbieden van gratis proefversies van 30 dagen. U kunt zich aanmelden voor de proefversies in de catalogus, net zoals veel andere onlineservices. Alle partners kunnen deelnemen.

## <a name="available-trial-offers"></a>Beschikbare proefaanbiedingen

U vindt al uw openstaande proefaanbiedingen op de **pagina** Klant. Op deze pagina worden alle abonnementen weergegeven, inclusief gratis proefversies en betaalde abonnementen. (Deze functie is momenteel niet beschikbaar in China.)

Elke klant heeft recht op één gratis proefversie voor elke beschikbare aanbieding. Ze kunnen bijvoorbeeld één gratis proefversie voor Microsoft 365 Business Standard en één gratis proefversie voor Office 365 E3. Als de klant echter al eigenaar is van de aanbieding, kan deze geen gratis proefversie voor die aanbieding gebruiken.

### <a name="available-products"></a>Beschikbare producten

Gratis proefversies zijn beschikbaar voor de meest uitgebreide en populaire licentieaanbiedingen. Er kunnen maandelijks nieuwe proefaanbiedingen worden geïntroduceerd.

Partners kunnen proefversies vinden in de lijst met maandelijkse prijzen op de **pagina met** prijzen en aanbiedingen in Partner Center. Proefaanbiedingen worden vermeld in de prijslijst Secundair **licentietype.**

Er zijn momenteel **geen gratis proefversies voor** overheidsaanbiedingen, onderwijsaanbiedingen of invoegaanbiedingen.

## <a name="licenses-for-free-trial-offers"></a>Licenties voor gratis proefaanbiedingen

Alle gratis proefversies bieden 25 licenties. U kunt dit nummer niet wijzigen tijdens de proefversie. U kunt geen licenties toevoegen aan of verwijderen uit de gratis proefversie. Nadat de proefversie is geconverteerd naar een betaald abonnement, kunt u meer licenties toevoegen aan het abonnement.

Licenties voor proefversies moeten op dezelfde manier worden toegewezen aan gebruikers als aan betaalde services.

## <a name="sign-customers-up-for-trials"></a>Klanten registreren voor proefversies

Een proefversie voor uw klant krijgen in Partner Center:

1. Ga **vanuit** Verkopen op Partner Center naar **Catalogus**. 
2. Selecteer in de catalogus bij **Factureringsfrequentie** de optie **Proefaanbieding.** Hierdoor kunnen alleen gratis proefversies worden weergegeven en worden andere aanbiedingen uitgeschakeld die niet gratis zijn. Proefversies worden weergegeven op het **tabblad Proefversies** in de catalogus.
3. Selecteer de gratis proefversie die u wilt aanbieden en selecteer vervolgens **Verzenden.** Alle proefversies zijn gedurende 30 dagen waarin u niet wordt gefactureerd. U kunt het ook op elk moment tijdens de proefversie converteren naar een betaald abonnement.

## <a name="converting-trials-to-paid-subscriptions"></a>Proefversies converteren naar betaalde abonnementen

Een gratis proefversie wordt niet automatisch geconverteerd naar een betaald abonnement. Na 30 dagen moet een gratis proefversie worden geconverteerd naar een betaald abonnement, anders verloopt [deze.](#expiring-offers) Gratis proefversies kunnen niet worden uitgebreid.

U moet de proefversie zelf omzetten in een betaald abonnement. U kunt dit doen [met behulp van de Partner Center](#convert-trials-using-partner-center) of via de Partner Center [API's](#convert-trials-using-apis).

> [!NOTE]
> Gratis proefversies van klanten voor het Cloud Solution Provider(CSP)-programma kunnen niet worden geconverteerd naar een andere programmaten tenant (zoals EA, Open of MOSP).

### <a name="convert-trials-using-partner-center"></a>Proefversies converteren met Partner Center

U kunt proefversies converteren naar betaalde abonnementen met behulp van Partner Center:

1. Ga naar de abonnementspagina van de klant en selecteer de gratis proefversie.
2. Selecteer **Proefversie converteren naar betaald abonnement.**
3. Voer de gewenste licentiehoeveelheid en factureringsfrequentie in en selecteer **Toepassen.**
4. De facturering voor het betaalde abonnement begint op de conversiedatum en het abonnement wordt 12 maanden na de conversiedatum automatisch verlengd. 

### <a name="convert-trials-using-apis"></a>Proefversies converteren met behulp van API's

Mogelijk moet u uw API's wijzigen om de conversie van een gratis proefversie naar een betaald abonnement mogelijk te maken. Zie de volgende documentatie voor ontwikkelaars voor meer informatie:

- [Een proefabonnement converteren naar betaald](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Een lijst met aanbiedingen voor omzetten van de proefversie ophalen](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Proefversies zonder conversies

Niet alle proefversies kunnen worden geconverteerd naar betaalde abonnementen. Partners kunnen een proefversie gebruiken die geen conversies heeft tot de vervaldatum. Partners kunnen compatibele aanbiedingen kopen die dezelfde services ondersteunen als de proefversie.  Dit moet worden gedaan voordat de proefversie verloopt om ervoor te zorgen dat de services van de nieuw gekochte aanbiedingen zijn afgestemd op de services van de proefversie. 

|**Proefversie**   |**Compatibele aanbiedingen voor kleine bedrijven**   |**Compatibele Enterprise-aanbiedingen**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Microsoft Teams Proefversie van commerciële cloud (door gebruiker geïnitieerd)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (voorheen F1), Office 365 for Enterprise (E1, E3 en E5), Microsoft 365 F1/F3, Microsoft 365 Enterprise (E3)   |

>[!NOTE]
>De bovenstaande aanbiedingen hebben vergelijkbare serviceplannen met vergelijkbare functionaliteit, maar er zijn mogelijk enkele verschillen tussen de aanbiedingen.

### <a name="expiring-offers"></a>Verlopende aanbiedingen

U wordt niet op de hoogte gesteld van verlopen aanbiedingen. U kunt toekomstige vervaldatums bijhouden met behulp van de klantweergave op Partner Center of door een query uit te voeren op de API. Het is een goed idee om deze datums regelmatig te controleren, zodat u de juiste vervolgacties kunt ondernemen met klanten wanneer ze een beslissingspunt benaderen.

Nadat een proefversie is verlopen, ziet een klant die zich probeert aan te melden bij die proefversie een verlopen bericht. De gegevens worden echter opgeslagen volgens de standaarden voor gegevensretentie. Nadat u een nieuw abonnement met dezelfde serviceabonnementen hebt aangeschaft, kunnen de gegevens van uw klant opnieuw worden geopend vanuit het zojuist geactiveerde abonnement.

## <a name="billing"></a>Billing

Jaarlijkse facturering en gratis proefversies zijn hetzelfde in onafhankelijke clouds en de openbare cloud. Het enige verschil is de proef-SKU's die beschikbaar zijn op het moment van starten.

## <a name="billing-for-free-trials"></a>Facturering voor gratis proefversies

Gratis proefversies kunnen worden gebruikt voor maandelijks en jaarlijks gefactureerde abonnementen. U kunt de factureringsfrequentie selecteren wanneer u de proefversie converteert naar een betaald abonnement.

De begindatum van het abonnement is gebaseerd op de conversiedatum. Als de gratis proefversie wordt geconverteerd naar een betaalde aanbieding met jaarlijkse facturering, is de verlengingsdatum van het abonnement 12 maanden na de conversiedatum. Als de gratis proefversie wordt geconverteerd naar een betaalde aanbieding met maandelijkse facturering, is de verlengingsdatum van het abonnement twaalf maanden vanaf de factureringsdatum na de conversiedatum.

### <a name="invoices"></a>Facturen

Er worden geen gratis proefversies weergegeven in uw factuur- of licentieafstemmingsbestand. Gratis proefversies worden alleen weergegeven op uw factuur- en licentieafstemmingsbestand nadat u een gratis proefversie hebt omgezet in een betaald abonnement. Het geconverteerde abonnement wordt op dezelfde manier weergegeven als elk nieuw abonnement.

### <a name="incentives"></a>Incentives

Gratis proefversies hebben geen invloed op incentives.

## <a name="support"></a>Ondersteuning

Voor ondersteuning bij gratis proefversies dient u een serviceaanvraag in via Partner Center.
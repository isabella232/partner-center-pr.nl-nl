---
title: Klanten testen van micro soft-producten bieden
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Laat klanten de producten van micro soft-abonnement 30 dagen proberen. Meld u aan voor deze gratis proef versies in de catalogus, net als veel andere onlineservices.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a51504a5e560f8a8041c448c3e5d9e7f0cfdae07
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528472"
---
# <a name="give-customers-30-day-free-trials-of-microsoft-products"></a>Bied klanten 30 dagen gratis proef versies van micro soft-producten

**Van toepassing op**

- Partnercentrum

**Juiste rollen**
-   Globale beheerder 
-   Gebruikersbeheerder
-   Verkoop agent

Een goede manier om klanten te introduceren voor nieuwe micro soft-producten is gratis proef versies van 30 dagen aanbieden. U kunt zich registreren voor de experimenten in de catalogus, net als veel andere onlineservices. Alle partners kunnen deel nemen.

## <a name="available-trial-offers"></a>Beschik bare proef aanbiedingen

U kunt alle aanbiedingen van openstaande proef versies vinden op de pagina **klant** . Op deze pagina worden alle abonnementen weer gegeven, met inbegrip van gratis proef versies en betaalde abonnementen. (Deze functie is momenteel niet beschikbaar in China.)

Elke klant heeft recht op één gratis proef versie voor elke beschik bare aanbieding. Ze kunnen bijvoorbeeld een gratis proef versie van Microsoft 365 Business Standard en één gratis proef versie voor Office 365 E3 krijgen. Als de klant echter al eigenaar is van de aanbieding, kunnen ze geen gratis proef versie gebruiken voor die aanbieding.

### <a name="available-products"></a>Beschik bare producten

Gratis proef versies zijn beschikbaar voor de meest uitgebreide en populaire licesen-aanbiedingen. Nieuwe proef aanbiedingen kunnen maandelijks worden geïntroduceerd.

Partners kunnen proef versies vinden in de lijst met maandelijkse prijzen op de pagina **prijzen en aanbiedingen** van het partner centrum. Voor proef abonnementen wordt ' proef versie ' weer gegeven in de kolom prijs lijst **secundair licentie type** .

Er zijn momenteel **geen gratis proef versies** voor aanbiedingen van de overheid, onderwijs of invoeg toepassingen.

## <a name="licenses-for-free-trial-offers"></a>Licenties voor gratis proef abonnementen

Alle gratis proef versies bieden 25 licenties. U kunt dit nummer niet wijzigen tijdens de proef versie. U kunt geen licenties toevoegen aan of verwijderen uit de gratis proef versie. Nadat de proef versie is geconverteerd naar een betaald abonnement, kunt u aanvullende licenties aan het abonnement toevoegen.

Proef licenties moeten worden toegewezen aan gebruikers op dezelfde manier als de betaalde service licentie worden toegewezen.

## <a name="sign-customers-up-for-trials"></a>Klanten registreren voor proef versies

Down load een proef versie voor uw klant in Partner Center:

1. Ga **vanuit het** Partner Center naar **Catalog** . 
2. Klik in de catalogus, van **facturerings frequentie** , op **proef** abonnement. Hiermee kunnen alleen gratis proef versies worden weer gegeven en andere aanbiedingen die niet gratis zijn, worden uitgeschakeld. De proef versies worden weer gegeven op het tabblad **Trials** in de catalogus.
3. Selecteer de gratis proef versie die u wilt aanbieden en selecteer vervolgens **verzenden** . Alle experimenten duren dertig dagen waarin u niet wordt gefactureerd. U kunt deze ook op elk gewenst moment tijdens de proef versie converteren naar een betaald abonnement.

## <a name="converting-trials-to-paid-subscriptions"></a>Experimenten converteren naar betaalde abonnementen

Een gratis proef versie wordt niet automatisch omgezet in een betaald abonnement. Na dertig dagen moet een gratis proef versie worden geconverteerd naar een betaald abonnement of [verlopen](#expiring-offers). Gratis proef versies kunnen niet worden uitgebreid.

U moet de proef versie in een betaald abonnement zelf omzetten. U kunt dit doen [met behulp van het partner centrum](#convert-trials-using-partner-center) of [via de Api's van het partner centrum](#convert-trials-using-apis).

> [!NOTE]
> Gratis proef versies van klanten voor het programma Cloud Solution Provider (CSP) kunnen niet worden geconverteerd naar een andere programma-Tenant (zoals EA, open of MOSP).

### <a name="convert-trials-using-partner-center"></a>Experimenten converteren met behulp van partner centrum

U kunt met behulp van partner centrum experimenten converteren naar betaalde abonnementen:

1. Ga naar de abonnements pagina van de klant en selecteer de gratis proef versie.
2. Selecteer **proef versie naar betaald abonnement converteren** .
3. Voer de gewenste licentie hoeveelheid en facturerings frequentie in en selecteer **Toep assen** .
4. De facturering voor het betaalde abonnement begint op de conversie datum en het abonnement wordt twaalf maanden na de conversie datum verlengd. 

### <a name="convert-trials-using-apis"></a>Experimenten converteren met behulp van Api's

Mogelijk moet u uw Api's aanpassen om de conversie van een gratis proef versie naar een betaald abonnement te kunnen bieden. Raadpleeg de volgende documentatie voor ontwikkel aars voor meer informatie:

- [Een proef abonnement converteren naar betaald](/partner-center/develop/convert-a-trial-subscription-to-paid)
- [Een lijst met aanbiedingen voor proef conversie ophalen](/partner-center/develop/get-a-list-of-trial-conversion-offers)

### <a name="trials-without-conversions"></a>Experimenten zonder conversies

Niet alle experimenten kunnen naar betaalde abonnementen worden geconverteerd. Partners kunnen een proef versie gebruiken die tot de verval datum geen conversies heeft. Partners kunnen compatibele aanbiedingen aanschaffen die dezelfde services als de proef aanbieding ondersteunen.  Dit moet worden gedaan voordat de proef versie verloopt om ervoor te zorgen dat de services die nieuw zijn gekocht, worden afgestemd op de services van de proef versie. 

|**Proefversie**   |**Compatibele aanbiedingen voor kleine bedrijven**   |**Compatibele Enter prise-aanbiedingen**   |
|----------------------------|:---------------------------------|:------------------------------------------|
|Proef versie van micro soft teams Commercial Cloud (door gebruiker gestart)   |Microsoft 365 Business Basic, Microsoft 365 Business Standard, Microsoft 365 Business Premium   | F3 (voorheen F1), Office 365 voor ondernemingen (E1, E3 en E5), M365 F1/F3, M365 Enter prise (E3)   |

>[!NOTE]
>De bovenstaande aanbiedingen hebben vergelijk bare service plannen met vergelijk bare functionaliteit, maar er zijn mogelijk een aantal verschillen tussen de aanbiedingen.

### <a name="expiring-offers"></a>Aanbiedingen verlopen

U wordt niet op de hoogte gesteld van verlopende aanbiedingen. U kunt toekomstige verloop datums bijhouden met behulp van de klanten weergave van het partner centrum of door de API te doorzoeken. Het is een goed idee deze datums regel matig te bewaken, zodat u de juiste opvolgings acties kunt ondernemen met klanten wanneer zij een beslissings punt volgen.

Nadat een proef versie is verlopen, wordt een verlopen bericht weer gegeven door een klant die zich probeert aan te melden bij deze proef versie. De gegevens worden echter opgeslagen in overeenstemming met de standaarden voor het bewaren van gegevens. Nadat u een nieuw abonnement met dezelfde service plannen hebt aangeschaft, kunnen de gegevens van uw klant opnieuw worden geopend vanuit het zojuist geactiveerde abonnement.

## <a name="billing"></a>Billing

Het jaarlijkse facturerings-en gratis proef abonnement zijn hetzelfde in soevereine Clouds en de open bare Cloud. Het enige verschil is de trial-Sku's die beschikbaar zijn op het moment van starten.

## <a name="billing-for-free-trials"></a>Gratis proef versies factureren

Gratis proef versies kunnen worden gebruikt voor zowel maandelijkse als jaarlijkse gefactureerde abonnementen. U kunt de facturerings frequentie selecteren wanneer u de proef versie naar een betaald abonnement converteert.

De begin datum van het abonnement is gebaseerd op de conversie datum. Als de gratis proef versie wordt omgezet in een betaald aanbod met jaarlijkse facturering, wordt de vernieuwings datum van het abonnement twaalf maanden na de conversie datum. Als de gratis proef versie wordt omgezet in een betaald aanbod met maandelijkse facturering, wordt de vernieuwings datum van het abonnement twaalf maanden na de factuur datum na de conversie datum.

### <a name="invoices"></a>Facturen

U ziet geen gratis proef versies die worden vermeld in uw factuur of afstemmings bestand op basis van licentie. Gratis proef versies worden alleen weer gegeven op uw factuur en op basis van licentie afstemmings bestanden nadat u een gratis versie hebt geconverteerd naar een betaald abonnement. Het geconverteerde abonnement wordt weer gegeven op dezelfde manier als een nieuw abonnement.

### <a name="incentives"></a>Ter

Gratis proef versies hebben geen invloed op prikkels.

## <a name="support"></a>Ondersteuning

Voor ondersteuning voor gratis proef versies moet u een service aanvraag indienen via partner Center.
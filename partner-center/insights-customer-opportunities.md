---
title: Partner Center Insights - CloudAscent Propensity-rapporten
description: Meer informatie over de CloudAscent Propensity-rapporten in Partner Center. Bevat informatie over de wil van een klant om Microsoft-producten te kopen.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 4248c3d72512073ba361bf1e0ee276a766b04176
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957364"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent Propensity-rapporten die beschikbaar zijn via Partner Center dashboard

**Juiste rollen:** Rapportviewer voor leidinggevenden | Rapportviewer

Het Partner Center dashboard bevat downloadbare propensiteitsgegevens uit het CloudAscent-programma. De gegevens tonen de kans van klanten om Microsoft-producten te kopen.  In dit artikel wordt de uitsplitsing van deze gegevens beschreven, hoe u de score gebruikt en wat deze betekent.

## <a name="summary-definitions"></a>Samenvattingsdefinities

- **SMC-klanten:** dit is het totale aantal klanten in de eigenaarsdownloads.  Klanten worden geïdentificeerd door de recordpartner.
- **Verlopen overeenkomsten:** binnen het huidige boekjaar geven we het aantal verlopende overeenkomsten op.
- **Open Expiring Revenue:** de omzet die is gekoppeld aan de openstaande verloopovereenkomsten.

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="Schermopname van het dashboard Samenvatting van verkoopkansen van klanten.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB-segmentatie

Het segment voor kleine tot middelgrote bedrijven (SMB) is onderverdeeld in drie afzonderlijke subsegmenten.

1. **De belangrijkste Onmanaged** omvat de grootste SMB-klanten met de meeste mogelijkheden voor Microsoft. Typische niet-beheerde klanten delen vergelijkbare kenmerken als beheerde accounts, met een groot aantal werknemers, grote IT-budgetten en -uitgaven en grote hoeveelheden potentiële omzet voor Microsoft.

   We definiëren Top Unmanaged op twee manieren:

   - **Belangrijkste niet-beherende gebruikers:** bevat accounts met 300 of meer werknemers. User-Based-accounts zijn geweldige doelen voor de eerste aankoop of uitbreiding van abonnementsproducten op basis van gebruikers, zoals Microsoft 365, Dynamics 365 of Surface.
   - **Belangrijkste onmanaged rekenkracht:** bevat accounts met een Azure-potentieel van meer dan $ 10.000. Compute-accounts omvatten bestaande Azure. accounts met aanzienlijk potentieel voor het komende jaar en accounts die Azure nog niet hebben aangeschaft, maar een potentieel hebben voor Azure van meer dan $ 10.000.

2. **Middelgrote bedrijven** omvatten bestaande klanten en prospectaccounts met 25 tot 300 werknemers.

3. **Kleine bedrijven** omvatten bedrijven met 10-25 werknemers.

4. **Zeer kleine bedrijven** zijn bedrijven met 1-9 werknemers.

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="Klant op SMC-type.":::

**De belangrijkste subsegmenten Unmanaged** en **Medium Business** vertegenwoordigen klanten met een hoge levensduur (LTV) voor Microsoft en Microsoft-partners. Daarom zijn ze de hoofdgebieden van de focus om de groei in dit segment te stimuleren. In deze twee subsegmenten zijn we beter in staat om de socket te verkrijgen met Microsoft 365, verder geld te verdienen met D365-/Azure LOB-apps (Line-Of-Business) en een hoge LTV voor Microsoft te realiseren.

Op dit moment hebben we twee belangrijke gebieden van kansen: 1. onze klant voegt groei toe; 2. hoewel we goed zijn in het verkrijgen van cloudsockers die Microsoft 365, hebben we een grote kans in Dynamics 365 en Azure.

De volgende schermopname vertegenwoordigt de vier SMB-subsegmenten. CloudAscent prioriteert de profilering, score en modellering van alle niet-beherende en middelgrote zakelijke accounts.

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="Schermopname van SMB-subsegmenten.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB maakt gebruik machine learning om voorspellingen van verkoop- en marketingklant binnen de segmenten Top Unmanaged en Medium Business te stimuleren. Hoe worden signalen verzameld en omgezet in aanbevelingen voor goedheid?

- **Gegevensverzameling:** web-crawlers scannen en verzamelen miljarden klantsignalen door de bedrijfsdomeinen te pingen en blogposts, drukreleases, sociale streams en technische forums te bewaken.  Naast de verzamelde signalen wordt er firmographics-informatie verzameld uit zowel interne als externe bronnen, zoals D&B, een intern Microsoft-abonnement en transactionele gegevens.

- **Machine Learning:** De signalen worden ingevoerd in het machine learning-model dat per cloudproduct en cluster een gestructureerde gegevensset van verkoop- en marketingvoorspellingen voor elke klant uitvoert.  Elke klant wordt op basis van een look-gelijk model gescored op de belangrijkste SMB van Microsoft die bepaalt wat de klant past, en machine learning-algoritmen die het onlinegedrag van de klant integreren, definiëren als Intentie. De score wordt samengevoegd in clusters die laten zien dat een klant microsoft cloudproducten wil kopen.

- **Optimalisatie:** het Machine Learning optimaliseert de modellen door de transactiegegevens maandelijks en de abonnementsgegevens per kwartaal te gebruiken.  Met behulp van de winst-/verliesgegevens past de Machine Learning de algoritmen aan en controleert deze of de modellen werken zoals verwacht door clusteraanbevelingen te vergelijken met verkoopkansen die in MSX worden gebruikt.

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="Schermopname van SMB-machine learning.":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Hoe worden aanbevelingen voor de eigenheid gemaakt?

Met behulp van signalen die worden verzameld via web-crawlers en gegevens die afkomstig zijn uit verschillende bronnen, consolideren we de firmographics-gegevens en de signalen voor sociale media van de klant.  De score maakt gebruik van deze signalen en gegevens in vergelijkingsmodellen voor geschikte en scoring-modellen voor Intentie.

1. Passend klantaccount

   - Interne en externe gegevenspunten die firmographics definiëren.

   - Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft Cloud Products.

   - Passend scoren wordt elk kwartaal bijgewerkt

2. Intentie van klantaccount

   - Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie.

   - Het scoren van intenties wordt boven op fit om de clusters te definiëren.

   - Het scoren van intenties wordt maandelijks bijgewerkt.

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="CloudAscent SMB-voorspellende modellen.":::

3. Clustering

   De signalen voor passend en intentie worden samengevoegd in een clusteringscore. CloudAscent heeft vier clusters:

      - Nu actie ondernemen - klanten die klaar zijn voor verkoop
      - Evalueren - klanten die klaar zijn voor marketing
      - Ouverture - bewustzijnscampagnes aandurveren
      - Opleiden : intenties opleiden en controleren

   Met de clustering kunnen gebruikers zich richten op specifieke klanten voor verkoop- en marketinginitiatieven op basis van segmentfactoren, bijvoorbeeld: product, geo, branche en verticaal.

   Het **tabblad Propensity-model** in de CloudAscent Workbooks deelt de eigenaarschap en de geschatte witruimte-omzet. Voor het definiëren van de clustering van Fit and Intent doorlopen we de volgende stappen:

      1. Met ML Modellen berekenen we eerst De score voor klantfitting en intentiescore op een schaal van 100.  Exacte scores variëren op basis van ML modellen.  Voorbeeldscores hieronder:

         |**Classificatie**|**Score**|
         |---------|:---------|
         |Hoog|75 - 100|
         |Normaal|55 - 74|
         |Beperkt|30 - 54|
         |Zeer laag|0 - 29|

      2. Met behulp van de bovenstaande regel classificeren we bedrijven als Hoog, Gemiddeld, Laag en Zeer laag voor zowel klantgeschikt als intentiesignalen.

      3. We plotten signalen over passendheid van klanten en intenties op een 2D-matrix met elk snijpunt dat de gelijkenis vertegenwoordigt. Bijvoorbeeld High Fit + High Intent = A1, die de hoogste prioriteit vertegenwoordigt.

      4. Ten slotte worden deze segmenten gegroepeerd om clusters te vormen.  A1, A2, A3, A4 vormen bijvoorbeeld het cluster Nu handelen.

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="CloudAscent-modellen.":::

   Voor deze klanten raden we u aan om zich te richten op Nu handelen en Klanten evalueren.

## <a name="cloudascent-products--models"></a>CloudAscent Products & modellen

De volgende afbeelding geeft een weergave van elk propensiteitsmodel in CloudAscent:

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="CloudAscent propensity model.":::

Witruimtemodellen bestaan uit voorspellingen voor bestaande Microsoft-klanten waar ze geen product hebben en/of net nieuwe potentiële klanten zijn.

Bij upsell-modellen worden transactiegegevens gebruikt om de potentiële upsell in Azure te voorspellen en Microsoft 365 SKU's.

Deze klanten hebben al zowel Azure als Microsoft 365 en het upsell-model laat zien dat ze waarschijnlijk meer van hun bestaande SKU zullen kopen.

EOS deelt de EOS-klanten (End of Service) voor Win 7, Office 2010, SQL Server en Windows Server. De EOS-gegevens worden uit MS Sales gehaald en worden waar beschikbaar over de CloudAscent-propensiteitsmodelleren heen getrokken. EOS-gegevens zijn te zien in Modern Work en Azure Sales.

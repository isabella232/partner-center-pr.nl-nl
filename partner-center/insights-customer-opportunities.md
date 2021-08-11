---
title: Partner Center Insights - CloudAscent Propensity-rapporten
description: Meer informatie over de CloudAscent Propensity-rapporten in Partner Center. Bevat informatie over de reensiteit van een klant om Microsoft-producten te kopen.
ms.topic: conceptual
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 04/27/2021
ms.openlocfilehash: 9c9c592a5720642c9d2d0c7b5ac8c2a4aa23387d4d6c063ca1e064959a340c1e
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115686303"
---
# <a name="cloudascent-propensity-reports-available-from-partner-center-dashboard"></a>CloudAscent Propensity-rapporten die beschikbaar zijn via Partner Center dashboard

**Juiste rollen:** Rapportviewer voor leidinggevenden | Rapportviewer

Het Partner Center dashboard bevat downloadbare propensiteitsgegevens uit het CloudAscent-programma. De gegevens tonen de kans van klanten om Microsoft-producten te kopen.  In dit artikel wordt de uitsplitsing van deze gegevens beschreven, hoe u de score gebruikt en wat het betekent.

## <a name="summary-definitions"></a>Samenvattingsdefinities

- **SMC-klanten:** dit is het totale aantal klanten in de smc-downloads.  Klanten worden geïdentificeerd door de recordpartner.
- **Verlopen-overeenkomsten:** binnen het huidige fiscale jaar geven we het aantal verlopende overeenkomsten op.
- **Open Expiring Revenue:** de omzet die is gekoppeld aan de openstaande verlopende overeenkomsten.

:::image type="content" source="images/insights/customer-opportunity-1.png" alt-text="Schermopname van het dashboard Verkoopkansen van klanten.":::

## <a name="cloudascent-smb-segmentation"></a>CloudAscent SMB-segmentatie

Het segment voor kleine tot middelgrote bedrijven (SMB) is onderverdeeld in drie afzonderlijke subsegmenten.

1. **Top Unmanaged** omvat de grootste SMB-klanten met de meeste mogelijkheden voor Microsoft. Veel klanten die het meest worden beheerd, hebben vergelijkbare kenmerken als beheerde accounts, met een groot aantal werknemers, grote IT-budgetten en uitgaven en grote hoeveelheden potentiële omzet voor Microsoft.

   We definiëren Top Unmanaged op twee manieren:

   - **Belangrijkste niet-managed op basis van gebruikers:** accounts met 300 of meer werknemers. User-Based-accounts zijn fantastische doelen voor de eerste aankoop of uitbreiding van abonnementsproducten op basis van gebruikers, zoals Microsoft 365, Dynamics 365 of Surface.
   - **Belangrijkste onmanaged rekenkracht:** omvat accounts met een Azure-potentieel van meer dan $ 10.000. Rekenaccounts omvatten bestaande Azure. accounts met een aanzienlijk potentieel voor het komende jaar en accounts die Azure nog moeten aanschaffen, maar een potentieel hebben voor Azure groter dan $ 10.000.

2. **Middelgrote bedrijven** omvatten bestaande klanten en prospectaccounts met 25 tot 300 werknemers.

3. **Kleine bedrijven** omvatten bedrijven met 10-25 werknemers.

4. **Zeer kleine bedrijven** omvatten bedrijven met 1-9 werknemers.

:::image type="content" source="images/insights/customer-opportunity-2.png" alt-text="Klant op SMC-type.":::

**De belangrijkste subsegmenten Unmanaged** en **Medium Business** vertegenwoordigen klanten met een hoge levensduurwaarde (LTV) voor Microsoft en Microsoft-partners. Daarom zijn ze de hoofdgebieden voor het stimuleren van de groei in dit segment. In deze twee subsegmenten is het beter om de socket met Microsoft 365 te verkrijgen, geld te verdienen met D365-/Azure LOB-apps (Line-Of-Business) en een hoge LTV voor Microsoft te realiseren.

Vandaag de dag hebben we twee belangrijke gebieden van kansen: 1. onze klant voegt groei toe; 2. hoewel we goed werken aan het verkrijgen van cloudsockers die Microsoft 365, hebben we een grote kans in Dynamics 365 en Azure.

De volgende schermopname vertegenwoordigt de vier SMB-subsegmenten. CloudAscent geeft prioriteit aan de profilering, score en modellering van alle accounts met de hoogste onmanagede en middelgrote bedrijven.

:::image type="content" source="images/insights/customer-opportunity-3.png" alt-text="Schermopname van SMB-subsegmenten.":::

## <a name="cloudascent-machine-learning"></a>CloudAscent Machine Learning

SMB maakt gebruik machine learning om voorspellingen van verkoop- en marketingklant binnen de segmenten Top Unmanaged en Medium Business te stimuleren. Hoe worden signalen verzameld en omgezet in aanbevelingen voor goedheid?

- **Gegevensverzameling:** web-crawlers scannen en verzamelen miljarden klantsignalen door de bedrijfsdomeinen te pingen en blogposts, releases, sociale streams en technische forums te bewaken.  Naast de verzamelde signalen worden er firmographics-gegevens verzameld uit zowel interne als externe bronnen, zoals D&B, een intern Microsoft-abonnement en transactionele gegevens.

- **Machine Learning:** De signalen worden ingevoerd in het machine learning-model dat een gestructureerde gegevensset met verkoop- en marketingvoorspellingen voor elke klant op basis van cloudproduct en cluster als uitvoer geeft.  Elke klant wordt op basis van een look-gelijk model scoren op de belangrijkste SMB van Microsoft die de Fit-algoritmen van de klant bepaalt, en machine learning-algoritmen die het onlinegedrag van de klant integreren, definiëren als Intentie. De score wordt samengevoegd in clusters die laten zien dat een klant microsoft-cloudproducten wil kopen.

- **Optimalisatie:** het Machine Learning optimaliseert de modellen door de transactiegegevens maandelijks en de abonnementsgegevens per kwartaal te gebruiken.  Met behulp van de winst-/verliesgegevens past de Machine Learning de algoritmen aan en controleert deze of de modellen werken zoals verwacht door clusteraanbevelingen te vergelijken met verkoopkansen die in MSX worden gebruikt.

:::image type="content" source="images/insights/customer-opportunity-4.png" alt-text="Schermopname van SMB machine learning.":::

## <a name="cloudascent-propensity"></a>CloudAscent Propensity

Hoe worden aanbevelingen voor aan-eigenheid gemaakt?

Met behulp van signalen die worden verzameld via web-crawlers en gegevens die afkomstig zijn uit verschillende bronnen, consolideren we de firmographics-gegevens en de signalen voor sociale media van de klant.  De score maakt gebruik van deze signalen en gegevens in vergelijkingsmodellen voor fit- en scoremodellen voor Intent.

1. Klantaccount aanpassen

   - Interne en externe gegevenspunten die firmographics definiëren.

   - Passend scoren maakt gebruik van een vergelijkbaar model voor onze beste SMB om klanten te vergelijken en te zien of ze mogelijk geschikt zijn voor Microsoft Cloud-producten.

   - Passend scoren wordt elk kwartaal bijgewerkt

2. Intentie van klantaccount

   - Signalen met betrekking tot sociale media en het onlinegedrag van een klant definiëren Intentie.

   - Het scoren van intenties wordt boven op fit om de clusters te definiëren.

   - Intentiescores worden maandelijks bijgewerkt.

   :::image type="content" source="images/insights/customer-opportunity-5.png" alt-text="Voorspellende cloudascent SMB-modellen.":::

3. Clustering

   De signalen voor fit en intent worden samengevoegd in een clusteringscore. CloudAscent heeft vier clusters:

      - Nu actie ondernemen - klanten die klaar zijn voor verkoop
      - Evalueren - klanten die klaar zijn voor marketing
      - Nurture : bewustzijnscampagnes aandurveren
      - Opleiden : intenties opleiden en controleren

   Met clustering kunnen gebruikers zich richten op specifieke klanten voor verkoop- en marketinginitiatieven op basis van segmentfactoren, bijvoorbeeld: product, geo, branche en verticaal.

   Het **tabblad Propensity-model** in de CloudAscent Workbooks deelt de propensiteit en de geschatte witruimte-omzet. Voor het definiëren van de clustering van Fit and Intent doorlopen we de volgende stappen:

      1. Met ML Modellen berekenen we eerst de Customer Fit Score en intentiescore op een schaal van 100.  Exacte scores variëren op basis van ML modellen.  Voorbeeldscores hieronder:

         |**Classificatie**|**Score**|
         |---------|:---------|
         |Hoog|75 - 100|
         |Normaal|55 - 74|
         |Beperkt|30 - 54|
         |Zeer laag|0 - 29|

      2. Met behulp van de bovenstaande regel classificeren we bedrijven als Hoog, Gemiddeld, Laag en Zeer laag voor zowel Klantfitte als Intentiesignalen.

      3. We plotten signalen over de passen van klanten en intenties op een 2D-matrix met elk snijpunt dat de achterheid vertegenwoordigt. Bijvoorbeeld High Fit + High Intent = A1, die de hoogste reensiteit vertegenwoordigt.

      4. Ten slotte worden deze segmenten gegroepeerd om clusters te vormen.  Zo vormen A1, A2, A3 en A4 het cluster Nu reageren.

         :::image type="content" source="images/insights/customer-opportunity-6.png" alt-text="CloudAscent-modellen.":::

   Voor deze klanten wordt u aangeraden zich te richten op Nu handelen en Klanten evalueren.

## <a name="cloudascent-products--models"></a>CloudAscent Products & modellen

De volgende afbeelding geeft een weergave van elk ondersteuningsmodel in CloudAscent:

:::image type="content" source="images/insights/customer-opportunity-7.png" alt-text="CloudAscent propensity-model.":::

Witruimtemodellen bestaan uit voorspellingen voor bestaande Microsoft-klanten waar ze geen product hebben en/of net nieuwe prospectklanten zijn.

Bij upsell-modellen worden transactiegegevens gebruikt om de kans op upsell in Azure te voorspellen en Microsoft 365 SKU's.

Deze klanten hebben al zowel Azure als Microsoft 365 en het upsell-model laat zien dat ze waarschijnlijk meer van hun bestaande SKU zullen aanschaffen.

EOS deelt de EOS-klanten (end-of-service) voor Win 7, Office 2010, SQL Server en Windows Server. De EOS-gegevens worden uit MS Sales gehaald en waar beschikbaar over de CloudAscent-propensiteitsmodelleren heen getrokken. EOS-gegevens zijn te zien in Modern Work en Azure Sales.

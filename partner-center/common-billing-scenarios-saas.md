---
title: 'Facturering: SaaS-transacties op basis van licenties'
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Meer informatie over algemene factureringsscenario's in Partner Center voor SaaS-transacties (software als een dienst) op basis van licenties.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 85b5b4c33226236b7fcc3ce6b4833c3d58aba58ebb281b80576c9f26d04ecfe3
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115682246"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Algemene factureringsscenario's voor SaaS-transacties op basis van licenties in Partner Center

**Juiste rollen:** beheeragent | Factureringsbeheerder | Helpdeskagent | Verkoopagent


Deze [veelvoorkomende factureringsscenario's](common-billing-scenarios.md) zijn van toepassing op SaaS-abonnementen (Software as a Service) op basis van licenties in Partner Center.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Een gratis proefabonnement op SaaS converteren naar een betaald abonnement

In dit scenario wordt de facturering voor de verlenging van een saaS-abonnement op basis van een gratis proefversie beschreven. De verlenging converteert de gratis proefversie naar een betaald abonnement aan het einde van de gratis proefperiode.

In dit voorbeeld hebt u op 10 juni een gratis proefversie aangeschaft van een SaaS-abonnement op basis van licenties (software als een service). Deze gratis proefversie wordt automatisch verlengd als een betaald abonnement wanneer de gratis proefperiode eindigt.

De recon-bestanden bevatten de volgende kosten:

| Aankoopdatum | Begindatum van kosten | Einddatum van kosten | Eenheidsprijs | Eenheidshoeveelheid | Totaalbedrag | Kostentype | Beschrijving van het abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $ 0 | 1 | $ 0 | Nieuw | Gratis proefversie |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | $ 2 | 1 | $ 2 | Verlengen | Betaald abonnement |

## <a name="cancel-a-free-trial-saas-subscription"></a>Een gratis proefabonnement op SaaS annuleren

> [!TIP]
> U kunt een saaS-abonnement op basis van een licentie op elk moment annuleren, zelfs tijdens de gratis proefperiode.

In dit scenario hebt u op 1 juli een gratis saaS-proefabonnement op basis van licenties aangeschaft en dit abonnement vervolgens onmiddellijk geannuleerd in Partner Center.

Het recon-bestand bevat de volgende kosten:

| Aankoopdatum | Begindatum van kosten | Einddatum van kosten | Eenheidsprijs | Eenheidshoeveelheid | Totaalbedrag | Kostentype | Beschrijving van het abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Nieuw | Gratis proefversie |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Annuleren | Gratis proefversie |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>SaaS-abonnement voor aangepaste meters converteren naar een andere SKU

In dit scenario wordt beschreven hoe u op dezelfde datum een SaaS-abonnement voor aangepaste meters converteert van de ene SKU (Stock Keeping Unit) naar een andere SKU voor hetzelfde product.

In dit scenario hebt u één SKU (Silver) aangeschaft onder een product en deze op dezelfde datum geconverteerd naar een andere beschikbare SKU (Brons) onder dit product.

Het recon-bestand bevat de volgende kosten:

| Aankoopdatum | SKU | Begindatum van kosten | Einddatum van kosten | Eenheidsprijs | Eenheidshoeveelheid | Totaalbedrag | Kostentype | Beschrijving van het abonnement |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Zilver | 06/10/2019 | 06/10/2019 | $ 20 | 1 | $ 20 | Nieuw | SaaS-abonnement voor aangepaste meter |
| 06/10/2019 | Zilver | 06/10/2019 | 06/10/2019 | $ 20 | 1 | -$20 | Converteren | Prorated rebill for custom meter SaaS subscription (Prorated Rebill voor SaaS-abonnement met aangepaste meter) |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | $ 10 | 1 | $ 10 | Converteren | SaaS-abonnement voor aangepaste meter |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Op dezelfde datum een SaaS-abonnement voor een klantmeter kopen en annuleren

In dit scenario wordt de facturering beschreven voor een SaaS-abonnement voor klantmeters dat u op dezelfde Azure Portal hebt aangeschaft en geannuleerd.

In dit scenario hebt u een SaaS-abonnement voor aangepaste meters aangeschaft op Azure Portal. Vervolgens hebt u het abonnement op dezelfde datum geannuleerd.

| Aankoopdatum | SKU | Begindatum van kosten | Einddatum van kosten | Eenheidsprijs | Eenheidshoeveelheid | Totaalbedrag | Kostentype | Beschrijving van het abonnement |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | $ 10 | 1 | $ 10 | Nieuw | SaaS-abonnement voor aangepaste meter |
| 06/10/2019 | Bronze | 06/10/2019 | 06/10/2019 | $ 10 | 1 | -$10 | AnnulerenImmediate | SaaS-abonnement voor aangepaste meter |

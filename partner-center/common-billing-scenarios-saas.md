---
title: Op de factuur gebaseerde SaaS-trans acties
ms.topic: article
ms.date: 05/05/2020
description: Meer informatie over algemene facturerings scenario's in het partner centrum voor SaaS-trans acties (Software-as-a-Service) op basis van licenties.
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 3d63e8345bf127cb91f1812193b1f0311cd569b3
ms.sourcegitcommit: a8adb5f044f06bd684a5b7a06c8efe9f8b03d2db
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/14/2020
ms.locfileid: "92528682"
---
# <a name="common-billing-scenarios-for-license-based-saas-transactions-in-partner-center"></a>Algemene facturerings scenario's voor SaaS-trans acties op basis van licenties in het partner centrum

**Juiste rollen**

- Beheer agent
- Factureringsbeheerder
- Helpdesk medewerker
- Verkoop agent


Deze [veelvoorkomende facturerings scenario's](common-billing-scenarios.md) zijn van toepassing op op licenties gebaseerde SaaS-abonnementen (Software as a Service) in partner centrum.

## <a name="convert-a-free-trial-saas-subscription-to-a-paid-subscription"></a>Een gratis SaaS-abonnement voor een proef versie converteren naar een betaald abonnement

In dit scenario wordt de facturering beschreven voor het verlengen van een op licentie gebaseerd SaaS-abonnement voor een gratis proef versie. Met de verlenging wordt de gratis proef versie geconverteerd naar een betaald abonnement aan het einde van de gratis proef periode.

In dit voor beeld hebt u een gratis proef versie van een op een licentie gebaseerd SaaS-abonnement (software als een service) aangeschaft op 10 juni. Deze gratis proef versie wordt automatisch vernieuwd als een betaald abonnement wanneer de gratis proef periode eindigt.

De afstemmings bestanden bevatten de volgende kosten:

| Aankoop datum | Begin datum van kosten | Eind datum van de lading | Eenheidsprijs | Eenheids hoeveelheid | Totaalbedrag | Kostentype | Beschrijving van abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $ 0 | 1 | $ 0 | Nieuw | Gratis proefversie |
| 07/10/2019 | 07/10/2019 | 08/09/2019 | $2 | 1 | $2 | Verlengen | Betaald abonnement |

## <a name="cancel-a-free-trial-saas-subscription"></a>Een gratis SaaS-abonnement op een proef versie annuleren

> [!TIP]
> U kunt op elk gewenst moment een op licentie gebaseerd SaaS-abonnement voor een gratis proef versie annuleren, zelfs tijdens de gratis proef periode.

In dit scenario hebt u op 1 juli een op licenties gebaseerd SaaS-abonnement voor een gratis proef versie aangeschaft en vervolgens onmiddellijk geannuleerd in het partner centrum.

Het afstemmings bestand bevat de volgende kosten:

| Aankoop datum | Begin datum van kosten | Eind datum van de lading | Eenheidsprijs | Eenheids hoeveelheid | Totaalbedrag | Kostentype | Beschrijving van abonnement |
| ------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Nieuw | Gratis proefversie |
| 06/10/2019 | 06/10/2019 | 07/09/2019 | $ 0 | 11 | $ 0 | Annuleren | Gratis proefversie |

## <a name="convert-custom-meter-saas-subscription-to-another-sku"></a>SaaS-abonnement op aangepaste meter converteren naar een andere SKU

In dit scenario wordt beschreven hoe u een aangepaste meter SaaS-abonnement van één Stock Keeping Unit (SKU) converteert naar een andere SKU voor hetzelfde product, op dezelfde datum.

In dit scenario hebt u één SKU (zilver) aangeschaft onder een product en deze op dezelfde datum geconverteerd naar een andere beschik bare SKU (bronzen).

Het afstemmings bestand bevat de volgende kosten:

| Aankoop datum | SKU | Begin datum van kosten | Eind datum van de lading | Eenheidsprijs | Eenheids hoeveelheid | Totaalbedrag | Kostentype | Beschrijving van abonnement |
| ------------- | ----------------- | ----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Zilver | 06/10/2019 | 06/10/2019 | $ 20 | 1 | $ 20 | Nieuw | SaaS-abonnement aangepaste meter |
| 06/10/2019 | Zilver | 06/10/2019 | 06/10/2019 | $ 20 | 1 | -$20 | Converteren | Naar rato gefactureerd opnieuw betalen voor een SaaS-abonnement met aangepaste meter |
| 06/10/2019 | Bron | 06/10/2019 | 06/10/2019 | $ 10 | 1 | $ 10 | Converteren | SaaS-abonnement aangepaste meter |

## <a name="purchase-and-cancel-a-customer-meter-saas-subscription-on-same-date"></a>Een SaaS-abonnement van de klant meter op dezelfde datum kopen en annuleren

In dit scenario wordt de facturering van een SaaS-abonnement van de klant meter beschreven die u op dezelfde datum hebt aangeschaft en geannuleerd via de Azure Portal.

In dit scenario hebt u een aangepast SaaS-abonnement op de meter aangeschaft op het Azure Portal. Vervolgens hebt u het abonnement op dezelfde datum geannuleerd.

| Aankoop datum | SKU | Begin datum van kosten | Eind datum van de lading | Eenheidsprijs | Eenheids hoeveelheid | Totaalbedrag | Kostentype | Beschrijving van abonnement |
| ------------- | ------------- |----------------- | --------------- | ---------- | ------------- | ------------ | ----------- | ----------------- |
| 06/10/2019 | Bron | 06/10/2019 | 06/10/2019 | $ 10 | 1 | $ 10 | Nieuw | SaaS-abonnement aangepaste meter |
| 06/10/2019 | Bron | 06/10/2019 | 06/10/2019 | $ 10 | 1 | -$10 | CancelImmediate | SaaS-abonnement aangepaste meter |

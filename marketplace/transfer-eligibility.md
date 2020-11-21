---
title: Geschiktheid voor overdragen – richt lijnen voor het overdragen van een abonnement tussen facturerings accounts, Azure Marketplace
description: Richt lijnen voor commerciële controles voorafgaand aan het overdragen van een abonnement tussen facturerings accounts in de Azure Portal.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: a6a3c8954643ea982ae5107ae417a900ed51e77d
ms.sourcegitcommit: 1aa43438ad181278052788f15e017f9ae7777943
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 11/21/2020
ms.locfileid: "95007498"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Geschiktheid voor een abonnement overdragen tussen facturerings accounts

U kunt [een abonnement overzetten](/azure/cost-management-billing/understand/subscription-transfer) van het ene facturerings account naar het andere in het gedeelte Facturering van de Azure Portal. Vóór een overdracht wordt het abonnement gescand op producten van derden. De overdracht is alleen toegestaan als *alle* producten zijn gewist voor overdracht (Zie de onderstaande [criteria](#criteria-for-transfer-approval-or-denial) ). Het systeem genereert relevante fout berichten voor de apps die niet kunnen worden gewist om de volgende stappen te bepalen.

> [!NOTE]
> Dit artikel is niet van toepassing op SaaS-aanbiedingen omdat SaaS-resources zijn gekoppeld aan een Tenant, niet op een abonnement. SaaS-resources zijn overdraagbaar van het ene facturerings account naar het andere, maar dit gebeurt per resource en Azure-ondersteuning als ondersteunings aanvraag.

## <a name="criteria-for-transfer-approval-or-denial"></a>Criteria voor het goed keuren van de overdracht of weigering

U kunt een abonnement niet overdragen als een van de apps van derden aan een van de volgende criteria voldoet:

- Het doel account is commercieel en de app is opt-out voor de verkoop via partners.
- De app is opt-in voor geselecteerde partners en het doel account bevindt zich niet in de acceptatie lijst.
- De aanbieding is in het verleden een preview-aanbieding voor geselecteerde abonnementen of het is een privé-aanbieding en het abonnement is niet langer beschikbaar in de acceptatie lijst.
- Het nieuwe facturerings account bevindt zich in een andere regio dan waar de aanbieding wordt verkocht en de aanbieding wordt niet in die regio verkocht.

Een geblokkeerde overdracht blijft van kracht totdat u de resource uit het abonnement verwijdert, waarna u de overdracht opnieuw kunt proberen.

## <a name="next-steps"></a>Volgende stappen

[Ontvang ondersteuning voor Microsoft AppSource en Azure Marketplace](get-support.md)


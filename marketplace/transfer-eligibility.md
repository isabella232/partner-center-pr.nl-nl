---
title: 'Geschiktheid voor overdracht: richtlijnen voor het overdragen van een abonnement tussen factureringsaccounts, Azure Marketplace'
description: Richtlijnen voor commerciële controles vóór de overdracht van een abonnement tussen factureringsaccounts in de Azure Portal.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 11/20/2020
ms.openlocfilehash: 4b235bd462915fc205813ae86e92f98b4fd49fe4
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126245572"
---
# <a name="transfer-eligibility-for-a-subscription-between-billing-accounts"></a>Geschiktheid voor een abonnement overdragen tussen factureringsrekeningen

U kunt [een abonnement van het ene](/azure/cost-management-billing/understand/subscription-transfer) naar het andere factureringsaccount overdragen in de factureringssectie van de Azure Portal. Voorafgaand aan een overdracht wordt het abonnement gescand op producten van derden. De overdracht is alleen toegestaan als *alle* producten zijn gew cleared voor overdracht (zie de [onderstaande criteria).](#criteria-for-transfer-approval-or-denial) Het systeem genereert relevante foutberichten voor de apps die niet zijn gewreed, zodat u de volgende stappen kunt bepalen.

> [!NOTE]
> Dit artikel is niet van toepassing op SaaS-aanbiedingen omdat SaaS-resources zijn gekoppeld aan een tenant, niet aan een abonnement. SaaS-resources kunnen worden overdraagbaar van de ene factureringsrekening naar de andere, maar dit gebeurt per resource en door ondersteuning voor Azure als een ondersteuningsaanvraag.

## <a name="criteria-for-transfer-approval-or-denial"></a>Criteria voor goedkeuring of weigering van overdracht

U kunt een abonnement niet overdragen als een van de apps van derden voldoet aan een van de volgende criteria:

- Het doelaccount is commercieel en de app wordt uitgeschreven om te worden verkocht via partners.
- De app is ingeschakeld voor geselecteerde partners en het doelaccount staat niet in de lijst met toegestane partners.
- De aanbieding was in het verleden een preview-aanbieding voor geselecteerde abonnementen of was een privéaanbieding en het abonnement staat niet meer in de lijst met toegestane abonnementen.
- De nieuwe factureringsrekening is in een andere regio dan waar de aanbieding wordt verkocht EN de aanbieding mag niet in die regio worden verkocht.

Een geblokkeerde overdracht blijft van kracht totdat u de resource uit het abonnement verwijdert, waarna u de overdracht opnieuw kunt proberen.

## <a name="next-steps"></a>Volgende stappen

[Ondersteuning voor Microsoft AppSource en Azure Marketplace](get-support.md)


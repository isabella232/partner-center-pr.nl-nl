---
title: Partnertegoed voor beheerde services
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe het verdiende tegoed van microsoft-partners (PEC) voor beheerde services wordt berekend en betaald, en hoe u ervoor kunt zorgen dat u in aanmerking komt.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ba422a2feae2affb9c2b60ad345c4d6bb0d525c7
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110145861"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Hoe het verdiende tegoed van de partner wordt berekend en betaald

**Juiste rollen:** Globale | Gebruikersbeheerbeheer | Beheeragent | Factureringsbeheerders | Verkoopagent

Partnertegoed voor beheerde services (PEC) herkent en beloont partners die eigenaar zijn van het 24x7 IT-operationele beheer en beheer van onderdelen van of de volledige Azure-omgeving van hun klanten. Standaard krijgen partners in CSP de benodigde toegangsrechten voor het abonnement van de klant, zodat ze 24 x 7 operationeel beheer en beheer van de resources op het abonnement kunnen uitvoeren. Andere manieren waarop klanten toegang voor partners kunnen inrichten, wordt beschreven in de volgende sectie. Het maandelijkse factuurbedrag is het nettobedrag van het partnertegoed. Partners kunnen de details van de PEC bekijken over hun maandelijkse recon-bestand. Lees Abonnementen en resources beheren onder het [Azure-plan](azure-plan-manage.md)voor aanvullende manieren waarop een klant toegang kan inrichten voor de ver transacting partner.

Lees ook [Beheerdersbevoegdheden voor Azure CSP herstellen](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Subsidiabiliteit

Voor het ontvangen van het partnertegoed (PEC) gelden de volgende vereisten: 

- U moet een actieve MPN-overeenkomst en een geldige RBAC-rol (op rollen gebaseerd toegangsbeheer) hebben om verdiend tegoed te ontvangen voor de Azure-assets die u beheert.

- U moet 24x7 operationeel beheer en beheer hebben van de Azure-resources van de klant in CSP. Dit betekent dat u beheerdersbevoegdheden moet hebben voor het Azure-abonnement, de Azure-resourcegroep en de Azure-resource van de klant. In het geval van indirecte providers en hun indirecte resellers komt de indirecte provider in aanmerking voor PEC als de indirecte provider of de indirecte reseller of beide deze operationele controle hebben. Zie Beheerdersbevoegdheden voor Azure CSP [herstellen voor meer informatie.](./revoke-reinstate-csp.md)

- Naast de bovenstaande vereisten is PEC alleen van toepassing op services die worden vermeld in de prijzen voor azure-abonnementsverbruik, die u kunt exporteren op de pagina [prijzen voor Azure-plannen.](https://partner.microsoft.com/commerce/sales)

- PEC is **niet** van toepassing op de volgende services:
    - Reserveringen voor Azure-plannen
    - Producten van derden die zijn geïdentificeerd als derde partij in de kolom Tags van de prijs van het Azure-planverbruik
    - Producten in de marketplace-prijslijst
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC wordt verdiend tot het Azure-resourceniveau. Als u geldige toegang hebt op het niveau van het abonnement of de resourcegroep, verdient elke resource die wordt geworpen naar de hogere entiteit PEC.

- Meer informatie over PEC is ook beschikbaar op de [pagina Azure Cost Management.](/azure/cost-management-billing/costs/get-started-partners)

### <a name="calculation"></a>Berekening

PEC wordt dagelijks berekend en kan worden bekeken in het dagelijkse gebruiksbestand en het maandelijkse factuur reconbestand. Een partner (indirecte provider of indirecte reseller) moet toegang hebben voor de hele dag (24x7) om ervoor te zorgen dat hij of zij PEC verdient. PEC wordt dagelijks berekend op basis van de beheerde Azure-assets. Partners die permanente bevoegde toegang behouden tot de maand (toegangsbereik) en voor alle in aanmerking komende resources (toegangsbereik) verdienen volledige PEC. Bereik- en bereikvermindering resulteert in een lager PEC-tarief voor de maand. Het bestand met dagelijks beoordeeld gebruik wordt dagelijks op een Azure-asset gebruikt, ongeacht of PEC al dan niet wordt toegepast. Partners kunnen zich ook registreren voor waarschuwingen om wijzigingen in permanente bevoegde toegang te bewaken.

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) met behulp van Kostenanalyse kunt u als partner de kosten bekijken die het voordeel van PEC hebben ontvangen.  

1. Meld u Azure Portal aan [bij](https://portal.azure.com)uw partner-tenant en selecteer **Cost Management + Billing**.

2. Kostenbeheer **selecteren**

3. Kostenanalyse **selecteren**

   In de weergave Kostenanalyse worden de kosten voor uw factureringsrekening weergegeven voor alle services die zijn gekocht en verbruikt tegen de prijzen die u Microsoft betaalt.

4. Selecteer **PartnerEarnedCreditApplied** in de vervolgkeuzelijst in een draaigrafiek om de kosten te zien die zijn toegepast op PEC. Wanneer **de eigenschap PartnerEarnedCreditApplied** True is, hebben de bijbehorende kosten het voordeel van het verdiende tegoed van de partner. 

   Wanneer de eigenschap PartnerEarnedCreditApplied Onwaar is, voldoen de gekoppelde kosten niet aan de vereiste geschiktheid voor het tegoed of komt de aangeschafte service niet in aanmerking voor partnertegoed.

   >[!NOTE] 
   >Normaal gesproken duurt het 8-24 uur voordat het gebruik voor services wordt weergegeven in **Cost Management** en wordt het PEC-tegoed binnen 48 uur na het moment van toegang in Azure Cost Management.

5. U kunt ook groeperen op, en filteren op, de  **eigenschap PartnerEarnedCreditApplied** met behulp van de filterfuncties Groeperen op en Filterfuncties toevoegen om in te zoomen op kosten met PEC en de kosten die geen PEC hebben toegepast.

## <a name="next-steps"></a>Volgende stappen

- [Partnertegoed - overzicht](partner-earned-credit.md)

- Gedetailleerde voorbeelden van partnertegoedberekeningen vindt u in de prijslijst die u kunt bereiken via Partner Center dashboard (aanmelden vereist).

- [Verplaatsen naar Azure-plan - aan de slag](azure-plan-get-started.md)

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)

- [Beheerdersbevoegdheden voor uw Azure CSP intrekken of opnieuw intrekken](revoke-reinstate-csp.md)

---
title: Het tegoed van de partner voor beheerde services
ms.topic: article
ms.date: 12/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe micro soft partner (PEC) voor beheerde services wordt berekend en betaald, en hoe u ervoor kunt zorgen dat u in aanmerking komt.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 022e7aabd0d850660f8236dce9a4fab9069af01b
ms.sourcegitcommit: 10765386b2df0d4c2e8da9b302a692f452e1090d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "106087124"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Hoe het verdiende tegoed van de partner wordt berekend en betaald

**Juiste rollen**

- Globale beheerder
- Beheerder van gebruikers beheer
- Beheer agent
- Factureringsbeheerder
- Verkoop agent

De partner die het tegoed voor beheerde services (PEC) heeft behaald, erkent en beloont partners die eigenaar zijn van het operationele beheer en het beheer van onderdelen van, of de volledige Azure-omgeving van hun klanten. In CSP krijgen partners standaard de benodigde toegangs rechten voor het abonnement van de klant, zodat ze 24 X 7 operationeel beheer en beheer van de resources in het abonnement kunnen uitvoeren. In het volgende gedeelte worden de andere manieren beschreven waarop klanten toegang kunnen inrichten voor transactie partners. Het maandelijkse factuur bedrag is het netto van het tegoed van de partner. Partners kunnen de PEC-gegevens zien op hun maandelijkse afstemmings bestand. Lees [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)voor meer informatie over de manier waarop een klant toegang kan inrichten voor de handelende partner.

Lees ook de [beheerders bevoegdheden voor Azure CSP-abonnementen opnieuw invoeren](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Geschiktheid

De volgende vereisten zijn van toepassing op het ontvangen van de partner (PEC): 

- U moet over een actieve MPN-overeenkomst en een geldige RBAC-rol (Role-based Access Control) beschikken om het ontvangen van tegoed voor de door u beheerde Azure-assets te krijgen.

- U moet over een 24x7 operationeel beheer en beheer van de Azure-resources van de klant in CSP beschikken. Dit betekent dat u beheerders bevoegdheden nodig hebt voor het Azure-abonnement van de klant, Azure-resource groep, Azure-resource. In het geval van indirecte providers en hun indirecte wederverkopers komt de indirecte provider in aanmerking voor PEC als hetzij de indirecte provider ofwel de indirecte reseller ofwel beide over dit operationele beheer beschikken. Zie [beheerders bevoegdheden voor Azure CSP-abonnementen herstellen voor](./revoke-reinstate-csp.md)meer informatie.

- Naast de bovenstaande vereisten is PEC alleen van toepassing op Services die worden vermeld in de prijzen van het Azure-abonnement. deze kunt u exporteren via de prijs pagina voor [Azure-abonnementen](https://partner.microsoft.com/commerce/sales) .

- PEC is **niet** van toepassing op de volgende services:
    - Azure plan-reserve ringen
    - Producten van derden geïdentificeerd als derde partij in de kolom Tags van de verbruiks prijs van het Azure-abonnement
    - Producten in de prijs lijst voor Marketplace
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

- PEC wordt naar het Azure-resource niveau geverdiend. Als u geldige toegang hebt op het niveau van het abonnement of de resource groep, verdient elke resource die tot de hogere entiteit rolt, een PEC.

- Meer informatie over PEC is ook beschikbaar op de pagina [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners) .

### <a name="calculation"></a>Berekening

PEC wordt dagelijks berekend en kan worden weer gegeven in het dagelijks gebruiks bestand en het maandelijkse factuur afstemmings bestand. Een partner (een indirecte provider of een indirecte wederverkoper) moet toegang hebben tot de hele dag (24x7) om ervoor te zorgen dat ze PEC verdienen. PEC wordt dagelijks berekend op basis van de beheerde Azure-assets. Partners die permanente privileged Access via de maand (toegangs duur) bewaren en voor alle in aanmerking komende resources (bereik van toegang), verdienen volledige PEC. De beperking van het bereik en de periode resulteert in een lager PEC-tempo voor de maand. Dagelijks geclassificeerd gebruiks bestand wordt dagelijks op een Azure-Asset weer gegeven, of PEC wordt toegepast. Partners kunnen ook worden inge schreven in waarschuwingen om wijzigingen in permanente toegang te controleren.

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) met behulp van kosten analyse kunt u als partner de kosten bekijken die het voor deel van PEC hebben ontvangen.  

1. Meld u aan bij de partner-Tenant in het [Azure Portal](https://portal.azure.com)en selecteer **Cost Management + facturering**.

2. **Kosten beheer** selecteren

3. **Kosten analyse** selecteren

   In de weer gave kosten analyse worden de kosten voor uw facturerings account weer gegeven, voor alle services die zijn gekocht en verbruikt tegen de prijzen die u micro soft betaalt.

4. Selecteer **PartnerEarnedCreditApplied** in de vervolg keuzelijst van een draai grafiek om de kosten weer te geven waarop PEC is toegepast. Wanneer de eigenschap **PartnerEarnedCreditApplied** is ingesteld op True, hebben de bijbehorende kosten het voor deel van het tegoed van de partner. 

   Wanneer de eigenschap PartnerEarnedCreditApplied is ingesteld op False, voldoen de bijbehorende kosten niet aan het vereiste recht voor het tegoed of is de aangeschafte service niet in aanmerking komen voor een partner die het tegoed ontvangt.

   >[!NOTE] 
   >Normaal gesp roken duurt het gebruik voor Services 8-24 uur in **Cost Management** en de PEC-tegoeden worden binnen 48 uur na de toegangs tijd weer gegeven in azure Cost Management.

5. U kunt ook groeperen op, en filteren op, de eigenschap **PartnerEarnedCreditApplied** met behulp **van de Group by en** filter functies toevoegen om te zoomen op de kosten met PEC en de kosten waarop geen PEC is toegepast.

## <a name="next-steps"></a>Volgende stappen

- [Creditering van de partner-overzicht](partner-earned-credit.md)

- Gedetailleerde voor beelden van de credit berekeningen van de partner bevinden zich in de prijs lijst die u kunt bereiken via het dash board van de partner centrum (aanmelden is vereist).

- [Naar Azure-plan gaan-aan de slag](azure-plan-get-started.md)

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)

- [Beheerders bevoegdheden voor Azure CSP-abonnementen intrekken of terugzetten](revoke-reinstate-csp.md)

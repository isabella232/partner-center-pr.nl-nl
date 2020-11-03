---
title: Het tegoed van de partner voor beheerde services
ms.topic: article
ms.date: 05/26/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe micro soft partner (PEC) voor beheerde services wordt berekend en betaald, en hoe u ervoor kunt zorgen dat u in aanmerking komt.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 89fce612d5756da3f9674d4170ac8c0c3a48abfe
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92528777"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Hoe het tegoed van de partner wordt berekend en betaald

**Juiste rollen**

- Globale beheerder
- Gebruikersbeheerder
- Beheer agent
- Factureringsbeheerder
- Verkoop agent

De partner die het tegoed voor beheerde services (PEC) heeft behaald, erkent en beloont partners die eigenaar zijn van het operationele beheer en het beheer van onderdelen van, of de volledige Azure-omgeving van hun klanten. In CSP krijgen partners standaard de benodigde toegangs rechten voor het abonnement van de klant, zodat ze 24 X 7 operationeel beheer en beheer van de resources in het abonnement kunnen uitvoeren. In de volgende sectie worden extra manieren beschreven waarop de klant toegang kan inrichten voor het handelen van partners. Het maandelijkse factuurbedrag is het nettobedrag van het tegoed van de partner. Partners kunnen de PEC-gegevens zien op hun maandelijkse afstemmings bestand. Lees [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)voor meer informatie over de manier waarop een klant toegang kan inrichten voor de handelende partner.

Lees ook de [beheerders bevoegdheden voor Azure CSP-abonnementen opnieuw invoeren](revoke-reinstate-csp.md)

## <a name="important-eligibility-and-calculation-information"></a>Belangrijke informatie over geschiktheid en berekening

- De partner moet beschikken over een actieve MPN-overeenkomst en een geldige RBAC-rol voor het ontvangen van tegoed voor de Azure-assets die ze beheren. 

- In het geval van indirecte providers en hun indirecte wederverkopers komt de indirecte provider in aanmerking voor PEC als de indirecte provider of de indirecte reseller, of beide over een beschik bare operationele controle en beheer van de Azure-resources van de klant in CSP.

- PEC is gekoppeld aan gefactureerd (Factureerbaar) verbruik van het Azure-eigendom van de klant in CSP die wordt beheerd door de partner. PEC wordt alleen beschikbaar gesteld voor partners in CSP, gefactureerd door micro soft (indirecte provider en directe factuur partner). 

- In aanmerking komende Services: het tegoed van de partner is van toepassing op Services die worden vermeld in de prijzen van het **Azure-abonnement** . de partners kunnen exporteren van de prijs pagina van het [Azure-abonnement](https://partner.microsoft.com/commerce/sales) . Het tegoed van de partner is niet van toepassing op producten van derden die zijn geïdentificeerd als **derde partij** in de **kolom Tags** van de prijs lijst voor verbruiks abonnementen van Azure, Azure-plan reserveringen, producten in de prijs lijst Marketplace en [Azure spot virtual machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/).

- PEC wordt dagelijks berekend en kan worden weer gegeven in het dagelijks gebruiks bestand en het maandelijkse factuur afstemmings bestand. Een partner (een indirecte provider of een indirecte wederverkoper) moet toegang hebben tot de hele dag (24x7) om ervoor te zorgen dat ze PEC verdienen. PEC wordt dagelijks berekend op basis van de beheerde Azure-assets. De maximale PEC voor een bepaalde facturerings periode is 15%. Partners die permanente privileged Access via de maand (toegangs duur) bewaren en voor alle in aanmerking komende resources (bereik van toegang), verdienen een volledige PEC van 15%. De beperking van het bereik en de periode resulteert in een lager PEC-tempo voor de maand. Dagelijks geclassificeerd gebruiks bestand wordt dagelijks op basis van een Azure-Asset weer gegeven, ongeacht of de PEC wordt toegepast. Partners kunnen ook worden inge schreven in waarschuwingen om te detecteren of er wijzigingen zijn in permanente toegang.

- PEC wordt naar het Azure-resource niveau geverdiend. Als de partner geldige toegang heeft op het abonnement of het niveau van de resource groep, verdient elke resource die rollen tot de hogere entiteit heeft, de PEC.  

- Er zijn ook PEC-Details beschikbaar in [Azure Cost Management](/azure/cost-management-billing/costs/get-started-partners)

## <a name="azure-cost-management"></a>Azure Cost Management

Azure Cost Management (ACM) met behulp van kosten analyse kunt u als partner de kosten bekijken die het voor deel van PEC hebben ontvangen.  

1. Meld u aan bij de partner-Tenant in het [Azure Portal](https://portal.azure.com)en selecteer **Cost Management + facturering** .

2. **Kosten beheer** selecteren

3. **Kosten analyse** selecteren

   In de weer gave kosten analyse worden de kosten voor uw facturerings account weer gegeven, voor alle services die zijn gekocht en verbruikt tegen de prijzen die u micro soft betaalt.

4. Selecteer **PartnerEarnedCreditApplied** in de vervolg keuzelijst van een draai grafiek om de kosten weer te geven waarop een PEC is toegepast. Wanneer de eigenschap **PartnerEarnedCreditApplied** is ingesteld op True, hebben de bijbehorende kosten het voor deel van het tegoed van de partner. 

Wanneer de eigenschap PartnerEarnedCreditApplied is ingesteld op False, voldoen de bijbehorende kosten niet aan het vereiste recht voor het tegoed of is de aangeschafte service niet in aanmerking komen voor een partner die het tegoed ontvangt.

>[!NOTE] 
>Normaal gesp roken duurt het gebruik voor Services 8-24 uur in **Cost Management** en de PEC-tegoeden worden binnen 48 uur na de toegangs tijd weer gegeven in azure Cost Management.

5. U kunt ook groeperen op, en filteren op, de eigenschap **PartnerEarnedCreditApplied** met behulp **van de Group by en** filter functies toevoegen om te zoomen op de kosten met PEC en de kosten waarop geen PEC is toegepast.

## <a name="next-steps"></a>Volgende stappen

- [Creditering van de partner-overzicht](partner-earned-credit.md)

- Gedetailleerde voor beelden van de credit berekeningen van de partner bevinden zich in de prijs lijst die u kunt bereiken via het dash board van de partner centrum (aanmelden is vereist).

- [Naar Azure-plan gaan-aan de slag](azure-plan-get-started.md)

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)

- [Beheerders bevoegdheden voor Azure CSP-abonnementen intrekken of opnieuw instatussen](revoke-reinstate-csp.md)

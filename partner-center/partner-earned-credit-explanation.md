---
title: Partnertegoed voor beheerde services
ms.topic: article
ms.date: 08/12/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over hoe het verdiend tegoed van microsoft-partners (PEC) voor beheerde services wordt berekend en betaald, en hoe u ervoor kunt zorgen dat u in aanmerking komt.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 56884a5a6cbfbade881154275129c63dcd3456d8
ms.sourcegitcommit: fb9ca808f6362e81d65a6ba5770dc8820834a0ed
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/24/2021
ms.locfileid: "128422431"
---
# <a name="how-the-partner-earned-credit-is-calculated-and-paid"></a>Hoe het verdiende tegoed van de partner wordt berekend en betaald

**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Beheeragent | Factureringsbeheerders | Verkoopagent

Partner earned credit (PEC) for managed services recognizes and rewards partners who own IT operational control and management of some or all of a customers's Azure environment. 

Als CSP-partner krijgt u standaard de benodigde toegangsrechten voor het abonnement van uw klant, zodat u operationeel beheer en beheer kunt uitvoeren van de resources in het abonnement. Andere manieren waarop klanten toegang voor partners kunnen inrichten, wordt beschreven in de volgende sectie.

Het maandelijkse factuurbedrag is het nettobedrag van het tegoed van de partner. U kunt de details van PEC bekijken in uw maandelijkse recon-bestand. Zie de volgende artikelen voor aanvullende manieren waarop een klant toegang kan inrichten voor de transacting partner:

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)
- [Beheerdersbevoegdheden voor Azure CSP-abonnementen opnieuw instellen](revoke-reinstate-csp.md)

## <a name="eligibility"></a>Subsidiabiliteit

Voor het ontvangen van partnertegoed (PEC) gelden de volgende vereisten:

- U moet een actieve MPN-overeenkomst en een geldige [RBAC-rol](/azure/role-based-access-control/overview) (role-based [access control)](azure-roles-perms-pec.md) hebben.
- U moet beheerdersbevoegdheden namens [(AOBO)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) hebben voor het Azure-abonnement, de Azure-resourcegroep of de Azure-resource van de klant, of een geldige [RBAC-rol.](azure-roles-perms-pec.md)
- In het geval van indirecte providers en hun indirecte resellers komt een indirecte provider in aanmerking voor PEC als de indirecte provider of de indirecte reseller ofwel AOBO-bevoegdheden of een in aanmerking komende RBAC-rol hebben. Zie Beheerdersbevoegdheden voor Azure CSP [herstellen voor meer informatie.](revoke-reinstate-csp.md)
- De MPN-id van de partner moet behoren tot dezelfde v-org als de MPN-id van de koper of de MPN-id van Partner of Record (MPN). Zie [Uw partner-id koppelen om de impact op gedelegeerde resources te volgen](/azure/lighthouse/how-to/partner-earned-credit) voor meer informatie.
- PEC wordt verdiend op Azure-resourceniveau, resourcegroep of abonnement. Als een partner geldige toegang heeft op het niveau van het abonnement of de resourcegroep, verdient elke resource die wordt geworpen naar de hogere entiteit PEC.
- PEC is niet van toepassing op de volgende services:
    - Reserveringen voor Azure-plannen
    - Producten van derden die zijn geïdentificeerd als derde partij in de kolom Tags van de prijs van het Azure-planverbruik
    - Producten in de marketplace-prijslijst
    - [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

Naast de bovenstaande vereisten is PEC alleen van toepassing op services die worden vermeld in de prijzen voor azure-abonnementsverbruik. U kunt deze bekijken en exporteren op de pagina [met prijzen voor Azure-plannen.](https://partner.microsoft.com/commerce/sales)

Zie de pagina Azure [Cost Management](/azure/cost-management-billing/costs/get-started-partners) voor meer informatie over PEC.

Zie Rollen en machtigingen die zijn vereist om partnertegoed te verdienen voor meer informatie [over geschiktheid.](azure-roles-perms-pec.md)

## <a name="calculation"></a>Berekening

PEC wordt dagelijks berekend. U wordt betaald voor elke dag dat u voor PEC in aanmerking komt voor toegang tot elk abonnement. Hoewel PEC-gegevens niet op uw maandelijkse factuur worden weergegeven, worden de PEC-inkomsten in de aangepaste nettokostenregel in de factuur meegenomen. U vindt meer PEC-gegevens over het [dagelijkse gebruiksbestand](daily-rated-usage-recon-files.md) en in het maandelijkse factuur reconbestand.

:::image type="content" source="images/advanced-specializations/recon-file.png" alt-text="Schermopname van een Partner Center afstemmingsbestand dat kolommen identificeert." border="false":::

In de onderstaande tabel worden de PEC-elementen beschreven die zijn gevonden in het maandelijkse factuur reconbestand. Alle waarden zijn in USD, zoals wordt weergegeven in de kolom AI, PricingCurrency.

| Kolom  | Beschrijving  |
| --------  | -------  |
| Kolom C  | CustomerName  |
| Kolom P | UnitPrice |
| Kolom AD | EffectiveUnitPrice. Dit is de prijs nadat PEC is toegepast en aan de vereisten is voldaan. Wanneer PEC wordt toegepast, ziet u dat effectiveUnitPrice in kolom AD een percentage kleiner is dan de UnitPrice in kolom P.   |
| Kolom V  | PriceAdjustmentDescription. Dit is leeg als er niet aan de vereisten voor PEC wordt voldaan of als de PEC %-PEC wordt toegepast op UnitPrice. Mogelijk komt u echter in aanmerking voor extra tegoed. Als dat het zo is, worden ze weergegeven in deze kolom. Voorbeeld: 100% Korting op laag 1.   |

PEC-toegang bewaken:

- **Bestand met dagelijks beoordeeld gebruik** laat zien waar PEC dagelijks wordt toegepast (of niet)

- [**Azure Monitor-waarschuwingen**](azure-plan-manage.md) controleren wijzigingen in permanente bevoegde toegang.

Het bestand met dagelijks beoordeeld gebruik:

:::image type="content" source="images/advanced-specializations/partner-daily.png" alt-text="Schermopname van een Partner Center een dagelijks beoordeeld gebruiksbestand met de effectieve eenheidsprijs." border="false":::

## <a name="partner-earned-credit-api"></a>Partnertegoed-API

Een PEC-API is beschikbaar als onderdeel van de Azure API-toolset. Zie Een Azure-account koppelen aan een partner-id voor meer informatie over PowerShell- en [CLI-API's.](/azure/cost-management-billing/manage/link-partner-id)

## <a name="azure-cost-management-and-pec"></a>Azure Cost Management en PEC

Azure Cost Management (ACM) met behulp van Kostenanalyse kunt u als partner de kosten bekijken die het voordeel van PEC hebben ontvangen. Zie de CSP Spotlight-aanroep van mei [2021](https://commercial_licensing.eventbuilder.com/2021MayCSPSpotlight)voor een gedetailleerde presentatie over ACM.

## <a name="use-acm-to-view-your-partner-earned-credit"></a>ACM gebruiken om het tegoed van uw partner weer te geven

1. Meld u [in Azure Portal](https://portal.azure.com/)aan bij uw partner-tenant en selecteer **Cost Management + Billing**.
2. Selecteer **Kostenbeheer.**
3. Selecteer **Kostenanalyse.**
In de weergave Kostenanalyse worden de kosten voor uw factureringsaccount weergegeven voor alle services die zijn gekocht en verbruikt tegen de prijzen die u microsoft betaalt.

:::image type="content" source="images/advanced-specializations/partner-cost.png" alt-text="Schermopname van de pagina Kostenanalyse voor kostenbeheer." border="false":::

4. Selecteer partnerEarnedCreditApplied in de vervolgkeuzelijst draaigrafiek. 

    Als deze waarde **True** is, hebben de bijbehorende kosten het voordeel van het partnertegoed.

    Als deze waarde **Onwaar** is, voldoen de bijbehorende kosten niet aan de vereiste geschiktheid voor het tegoed of komt de aangeschafte service niet in aanmerking voor partnertegoed.

>[!NOTE]
>Normaal gesproken duurt het 8-24 uur voordat het gebruik voor services wordt weergegeven in Cost Management en het PEC-tegoed wordt binnen 48 uur na het moment van toegang in Azure Cost Management.

U kunt ook groeperen op en filteren op de eigenschap **PartnerEarnedCreditApplied** met behulp van de filterfuncties **Groeperen op** **en** Toevoegen. Op deze manier kunt u inzoomen op kosten met PEC en de kosten die geen PEC hebben toegepast.

## <a name="how-is-pec-paid"></a>Hoe wordt PEC betaald?
PEC-inkomsten worden in rekening gebracht op de aangepaste nettokostenregel binnen de factuur. Het **totaal** van de hieronder weergegeven factuur illustreert dit. Zie het maandelijkse factuurafstemmingsbestand en het dagelijks beoordeelde gebruiksbestand van Azure voor meer informatie over correcties.

:::image type="content" source="images/advanced-specializations/invoice.png" alt-text="Schermopname van een Partner Center met de melding dat aanpassingsgegevens worden weergegeven in recon- en dagelijkse gebruiksbestanden van Azure." border="false":::

## <a name="next-steps"></a>Volgende stappen

- [Prijslijst voor de nieuwe commerce-ervaring voor Azure in CSP](azure-plan-price-list.md)
- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)
- [Nieuwe Commerce-ervaring in CSP - Azure-facturering](azure-plan-billing.md)
- [Beheerdersbevoegdheden voor Azure CSP-abonnementen opnieuw instellen](revoke-reinstate-csp.md)
- [Partnertegoed - overzicht](partner-earned-credit.md)
- [Rollen, machtigingen voor partnertegoed](azure-roles-perms-pec.md)
- [Inzicht in partnertegoed (handleiding)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (aanmelding vereist)
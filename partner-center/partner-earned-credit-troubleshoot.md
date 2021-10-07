---
title: Problemen met partnertegoed oplossen
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over het oplossen van factuurproblemen en andere problemen met betrekking tot partnertegoed (PEC).
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: a8bb370c7154c8033990cac798c28e01eec7e17f
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593222"
---
# <a name="troubleshooting-partner-earned-credit"></a>Problemen met partnertegoed oplossen

**Juiste rollen:** Globale | Gebruikersbeheerbeheer | Beheeragent | Factureringsbeheerders | Verkoopagent

## <a name="troubleshooting-guide"></a>Handleiding voor het oplossen van problemen

Als u problemen hebt met PEC, zoals toegang of ontbrekende gegevens, controleert u de onderstaande items in de vermelde volgorde.

1. Zorg ervoor dat u de factuur voor G (Modern) en het recon-bestand ziet. Azure-plan en PEC worden niet weergegeven op de D-factuur (verouderd) of het recon-bestand.

2. Identificeer het type partner. (Indirecte resellers komen niet in aanmerking.)

3. Controleer of uw MPN-overeenkomst actief is.

4. Zorg er bij Indirecte providers voor dat de MPN-id van de reseller die is ingevoerd in Partner Center (of via API) overeenkomt met de MPN-id van de reseller die is ingevoerd in de Azure Portal.

5. Controleer of uw aanbieding in aanmerking komt. (Oude Azure-aanbiedingen, gereserveerde Instanties van Azure en producten van derden komen niet in aanmerking.)

6. Controleer of u een geldige rol Voor beheer namens (AOBO) of Role-Based Access Control (RBAC) hebt voor het abonnement/de resourcegroep/resource.

7. Bepaal of de klant uw RBAC-rol heeft verwijderd. Als dit het zo is, zie Beheerdersbevoegdheden voor de Azure CSP van een klant herstellen

8. Controleer of u de hele dag beheerderstoegang hebt.

9. Controleer of u de juiste kolommen in uw dagelijkse gebruiksbestand bekijkt.

## <a name="next-steps"></a>Volgende stappen

- [Prijslijst voor de nieuwe commerce-ervaring voor Azure in CSP](azure-plan-price-list.md)
- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)
- [Nieuwe Commerce-ervaring in CSP - Azure-facturering](azure-plan-billing.md)
- [Beheerdersbevoegdheden voor Azure CSP-abonnementen opnieuw instellen](reinstate-csp.md)
- [Partnertegoed - overzicht](partner-earned-credit.md)
- [Rollen, machtigingen voor partnertegoed](azure-roles-perms-pec.md)
- [Inzicht in partnertegoed (handleiding)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (aanmelding vereist)

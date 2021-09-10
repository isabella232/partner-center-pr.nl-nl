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
ms.openlocfilehash: 7ce31bd688c32da956f466d63beede3f0fc9f9ef
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957791"
---
# <a name="troubleshooting-partner-earned-credit"></a>Problemen met partnertegoed oplossen

**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Beheeragent | Factureringsbeheerder | Verkoopagent

## <a name="troubleshooting-guide"></a>Handleiding voor het oplossen van problemen

Als u problemen hebt met PEC, zoals toegang of ontbrekende gegevens, controleert u de onderstaande items in de vermelde volgorde.

1. Zorg ervoor dat u de factuur voor G (Modern) en het recon-bestand ziet. Azure-plan en PEC worden niet weergegeven op de D-factuur (verouderd) of het recon-bestand.

2. Identificeer het type partner. (Indirecte resellers komen niet in aanmerking.)

3. Controleer of uw MPN-overeenkomst actief is.

4. Zorg er bij Indirecte providers voor dat de MPN-id van de reseller die is ingevoerd in Partner Center (of via API) overeenkomt met de MPN-id van de reseller die is ingevoerd in de Azure Portal.

5. Controleer of uw aanbieding in aanmerking komt. (Oude Azure-aanbiedingen, gereserveerde Azure-instanties en producten van derden komen niet in aanmerking.)

6. Controleer of u een geldige rol hebt voor Beheer namens (AOBO) of Role-Based Access Control (RBAC) voor het abonnement/de resourcegroep/resource.

7. Bepaal of de klant uw RBAC-rol heeft verwijderd. Zo ja, zie Beheerdersbevoegdheden voor de abonnementsabonnementen van een klant Azure CSP herstellen

8. Controleer of u de hele dag beheerderstoegang hebt.

9. Controleer of u de juiste kolommen in uw dagelijkse gebruiksbestand bekijkt.

## <a name="next-steps"></a>Volgende stappen

- [Prijslijst voor de nieuwe commerce-ervaring voor Azure in CSP](azure-plan-price-list.md)
- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)
- [Nieuwe Commerce-ervaring in CSP - Azure-facturering](azure-plan-billing.md)
- [Beheerdersbevoegdheden voor Azure CSP-abonnementen opnieuw instellen](revoke-reinstate-csp.md)
- [Partnertegoed - overzicht](partner-earned-credit.md)
- [Rollen, machtigingen voor partnertegoed](azure-roles-perms-pec.md)
- [Inzicht in partnertegoed (handleiding)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (aanmelding vereist)

---
title: 'Azure-plan: abonnementen en resources & beheren'
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe partners verschillende opties voor op rollen gebaseerd toegangsbeheer (RBAC) kunnen gebruiken om operationeel beheer en beheer van de Azure-resources van een klant te krijgen.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: a885d8bbbd7541e199365a7c732aba0b67128053
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/17/2021
ms.locfileid: "112277144"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Abonnementen en resources beheren onder het Azure-abonnement

**Juiste rollen:** Beheerdersagent


In dit artikel wordt uitgelegd hoe CSP-partners verschillende opties voor op rollen gebaseerd toegangsbeheer (RBAC) kunnen gebruiken om operationeel beheer en beheer van de Azure-resources van een klant te krijgen. Wanneer u een klant overplaatst naar het Azure-plan, krijgt u standaard bevoorrechte beheerdersrechten toegewezen in Azure (abonnementseigenaarsrechten via beheerder namens).

 > [!NOTE]
 > Beheerdersrechten voor het Azure-abonnement kunnen door de klant worden verwijderd op abonnements-, resourcegroep- of workloadniveau. 

 Partners kunnen 24x7 operationeel beheer en beheer van de Azure-resources van een klant in CSP krijgen door gebruik te maken van verschillende opties die worden geboden via de functie voor op rollen gebaseerd toegangsbeheer (RBAC). 

- **Admin on Behalf Of (AOBO)** - Met [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)heeft elke gebruiker met de rol Beheerderagent in de partnerten tenant RBAC-eigenaarstoegang tot Azure-abonnementen die u via het CSP-programma maakt.

- **Azure Lighthouse:** AOBO biedt niet de flexibiliteit om afzonderlijke groepen te maken die met verschillende klanten werken of om verschillende rollen in te stellen voor groepen of gebruikers. Met Azure Lighthouse kunt u verschillende groepen toewijzen aan verschillende klanten of rollen. Omdat gebruikers het juiste toegangsniveau hebben via gedelegeerd resourcebeheer van Azure, kunt u het aantal gebruikers met de rol Beheerderagent verminderen (en dus volledige AOBO-toegang hebben). Dit helpt de beveiliging te verbeteren door onnodige toegang tot de resources van uw klanten te beperken. Het biedt u ook meer flexibiliteit om meerdere klanten op schaal te beheren. Lees voor meer informatie [Azure Lighthouse en het Cloud Solution Provider programma](/azure/lighthouse/concepts/cloud-solution-provider).

- **Directory- of gastgebruikers of [service-principals:](/azure/active-directory/develop/app-objects-and-service-principals)** u kunt gedetailleerde toegang tot CSP-abonnementen delegeren door gebruikers toe te voegen in de klantmap of gastgebruikers toe te voegen en specifieke RBAC-rollen toe te wijzen.

Microsoft raadt gebruikers aan de minimale machtigingen te hebben die ze nodig hebben om hun werk uit te voeren als beveiligingspraktijken. Zie [Azure Active Directory Privileged Identity Management resources](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="link-your-partner-id-mpn-id-to-your-credentials-for-managing-customers-azure-resources"></a>Uw partner-id (MPN-id) koppelen aan uw referenties voor het beheren van de Azure-resources van de klant

In de volgende tabel ziet u de methoden die worden gebruikt om uw partner-id te koppelen aan verschillende RBAC-toegangsopties.

|**Categorie**   |**Scenario**   |**MPN-id-associatie**|
|-----------------|:------------------------|:------------------|
|Aobo   |Directe CSP-partner of indirecte provider maakt het abonnement voor de klant, waardoor de directe CSP-partner of indirecte provider de standaardeigenaar van het abonnement wordt met behulp van AOBO; Directe CSP-partner of indirecte provider geven indirecte reseller toegang tot het abonnement met behulp van AOBO.|Automatisch (geen partnerwerk vereist)|
|Azure Lighthouse|Partner maakt een nieuwe [Managed Services-aanbieding in Marketplace.](/azure/lighthouse/concepts/managed-services-offers) Deze aanbieding wordt geaccepteerd in het CSP-abonnement en de partner krijgt toegang tot het CSP-abonnement.|Automatisch (geen partnerwerk vereist)|
|Azure Lighthouse|Partner implementeert [ARM-sjabloon](/azure/lighthouse/how-to/onboard-customer) in Azure-abonnement|De partner moet de MPN-id koppelen aan de gebruiker of service-principal in de partner-tenant. Voor meer informatie: [koppeling partner-id](/azure/billing/billing-partner-admin-link-started).|
|Directory- of gastgebruiker|Partner maakt een nieuwe gebruiker of service-principal in de klantmap en geeft de gebruiker toegang tot het CSP-abonnement. Partner maakt een nieuwe gebruiker of service-principal in de directory van de klant. De partner voegt de gebruiker toe aan een groep en geeft toegang tot het CSP-abonnement aan de groep.|De partner moet de MPN-id koppelen aan de gebruiker of service-principal in de tenant van de klant. Voor meer informatie: [koppeling partner-id](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Bevestig dat u beheerderstoegang hebt

U hebt beheerderstoegang nodig om de services van uw klant te beheren en om verdiend tegoed te ontvangen. Lees [Partnertegoeden voor](partner-earned-credit.md) gedetailleerde informatie over verdiend tegoed. U hebt twee manieren om ervoor te zorgen dat u weet dat u beheerderstoegang hebt.

- Het dagelijkse gebruiksbestand controleren: dit kan worden bepaald door de eenheidsprijs en de effectieve eenheidsprijs in het dagelijkse gebruiksbestand te bekijken en te controleren of er korting wordt toegepast. Als u de korting ontvangt, bent u de beheerder.

- Een Azure Monitor-waarschuwing maken: u kunt een [](/azure/azure-monitor/platform/alerts-activity-log) waarschuwing voor Azure Monitor activiteitenlogboek maken om een melding te ontvangen wanneer uw RBAC-toegang wordt verwijderd uit het CSP-abonnement.

### <a name="create-an-azure-monitor-alert"></a>Een Azure Monitor-waarschuwing maken

1. Waarschuwing maken.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="azure-waarschuwing.":::

2. Selecteer het type actie dat u wilt dat de waarschuwing moet ondernemen. Als u bijvoorbeeld opgeeft dat u een e-mailbericht wilt ontvangen, ontvangt u een e-mail met de melding dat een roltoewijzing wordt verwijderd.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="waarschuwing configureren.":::

### <a name="aobo-removal"></a>AOBO verwijderen

Klanten kunnen de toegang tot hun abonnementen beheren door naar **Access Control** op de Azure Portal. Op het **tabblad Roltoewijzingen** selecteren ze **Toegang verwijderen.** Als dit gebeurt, kunt u het volgende doen:

- Praat met uw klant om te zien of beheerderstoegang opnieuw kan worden ingesteld.

- Gebruik de toegang die wordt geboden [via op rollen gebaseerd toegangsbeheer (RBAC).](/azure/role-based-access-control/overview)

- Gebruik toegang die wordt geboden [via Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

Toegang op basis van rollen verschilt van beheerderstoegang. Rollen bepalen precies wat u wel en niet kunt doen. Beheerderstoegang is breder.

Lees Rollen en machtigingen voor het partnertegoed om te zien welke rollen in aanmerking komen om PEC [te verdienen.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)

## <a name="next-steps"></a>Volgende stappen

- [Beheerdersbevoegdheden voor uw Azure CSP ingetrokken en opnieuw in te stellen](revoke-reinstate-csp.md)

- [Partnertegoed - overzicht](partner-earned-credit.md)

- [Partnertegoed voor beheerde services](partner-earned-credit-explanation.md)
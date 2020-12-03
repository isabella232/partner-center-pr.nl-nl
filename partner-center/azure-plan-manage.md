---
title: 'Azure-abonnement: abonnementen & resources beheren'
ms.topic: article
ms.date: 05/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ontdek hoe partners verschillende RBAC-opties (op rollen gebaseerd toegangs beheer) kunnen gebruiken om operationele controle en beheer van de Azure-resources van een klant te verkrijgen.
author: amitravat
ms.author: amrava
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 31e9c6862a5aa19407fa6da5e15333bb7e696720
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534927"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Abonnementen en resources beheren onder het Azure-abonnement

**Juiste rollen**

- Beheer agent


In dit artikel wordt uitgelegd hoe CSP-partners verschillende RBAC-opties (op rollen gebaseerd toegangs beheer) kunnen gebruiken om operationele controle en beheer van de Azure-resources van een klant te verkrijgen. Wanneer u een klant overstapt naar het Azure-abonnement, worden er standaard privileged-beheerders rechten toegewezen in azure (eigendoms rechten van het abonnement door de beheerder.

 > [!NOTE]
 > Beheerders rechten voor het Azure-abonnement kunnen worden verwijderd door de klant op een abonnement, resource groep of workload-niveau. 

 Partners kunnen het operationele beheer en het beheer van de Azure-resources van een klant in CSP belopen door gebruik te maken van verschillende opties die worden gegeven via de op rollen gebaseerde functie voor toegangs beheer (RBAC). 

- **Beheerder namens (administrate)** : met [administrate](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO)heeft elke gebruiker met de rol beheerder in de partner-Tenant toegang tot de Azure-abonnementen die u via het CSP-programma maakt.

- Met **Azure Lighthouse**: administrate is het niet mogelijk om afzonderlijke groepen te maken die samen werken met verschillende klanten, of om verschillende rollen in te scha kelen voor groepen of gebruikers. Met Azure Lighthouse kunt u verschillende groepen toewijzen aan verschillende klanten of rollen. Omdat gebruikers over het juiste toegangs niveau beschikken via het beheer van gedelegeerde resources van Azure, kunt u het aantal gebruikers met de rol beheerder (en dus volledige ADMINISTRATE) verminderen. Dit helpt de beveiliging te verbeteren door het beperken van onnodige toegang tot de resources van uw klanten. Daarnaast hebt u meer flexibiliteit om meerdere klanten op schaal te beheren. Lees [Azure Lighthouse en het Cloud Solution Provider-programma](/azure/lighthouse/concepts/cloud-solution-provider)voor meer informatie.

- **Map-of gast gebruikers of [service-principals](/azure/active-directory/develop/app-objects-and-service-principals)**: u kunt nauw KEURige toegang tot CSP-abonnementen delegeren door gebruikers toe te voegen aan de klanten Directory of door gast gebruikers toe te VOEGen en specifieke RBAC-rollen toe te wijzen.

Micro soft raadt aan dat gebruikers de minimale machtigingen hebben die ze nodig hebben om hun werk uit te voeren als een beveiligings procedure. Zie [Azure Active Directory privileged Identity Management resources](/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Koppel uw partner-ID (MPN-ID) aan uw referenties voor het beheren van de Azure-resources van de klant

De volgende tabel bevat de methoden die worden gebruikt voor het koppelen van uw partner-ID met verschillende RBAC-toegangs opties.

|**Categorie**   |**Scenario**   |**MPN-ID-koppeling**|
|-----------------|:------------------------|:------------------|
|ADMINISTRATE   |CSP direct-partner of indirecte provider maakt het abonnement voor de klant die de CSP direct-partner of de standaard eigenaar van de provider van het abonnement met ADMINISTRATE. CSP direct-partner of indirecte provider geven indirecte wederverkopers toegang tot het abonnement met behulp van ADMINISTRATE.|Automatisch (geen partner werk vereist)|
|Azure Lighthouse|Partner maakt een nieuw [aanbod voor beheerde services op Marketplace](/azure/lighthouse/concepts/managed-services-offers). Deze aanbieding wordt geaccepteerd op het CSP-abonnement en de partner krijgt toegang tot het CSP-abonnement.|Automatisch (geen partner werk vereist)|
|Azure Lighthouse|Partner implementeert [arm-sjabloon](/azure/lighthouse/how-to/onboard-customer) in azure-abonnement|De partner moet de MPN-ID koppelen aan de gebruiker of Service-Principal in de partner Tenant. Voor meer informatie- [koppeling partner-id](/azure/billing/billing-partner-admin-link-started).|
|Map of gast gebruiker|Partner maakt een nieuwe gebruiker of Service-Principal in de klanten Directory en biedt toegang tot het CSP-abonnement voor de gebruiker. Partner maakt een nieuwe gebruiker of Service-Principal in de klanten Directory. Partner voegt de gebruiker toe aan een groep en geeft toegang tot het CSP-abonnement op de groep.|De partner moet de MPN-ID koppelen aan de gebruiker of Service-Principal in de Tenant van de klant. Voor meer informatie- [koppeling partner-id](/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Controleer of u toegang hebt tot de beheerder

U hebt beheerders toegang nodig voor het beheren van de services van uw klant en het ontvangen van tegoed. Lees de [tegoeden](partner-earned-credit.md) van de partner voor gedetailleerde informatie over de tegoeden die u hebt ontvangen. U hebt twee manieren om er zeker van te zijn dat u toegang hebt tot de beheerder.

- Het dagelijks gebruiks bestand controleren: dit kan worden bepaald door de prijs per eenheid en de werkelijke eenheid van het dagelijks gebruik te controleren en te controleren of er korting wordt toegepast. Als u de korting van de beheerder ontvangt.

- Een Azure monitor-waarschuwing maken: u kunt een [waarschuwing](/azure/azure-monitor/platform/alerts-activity-log) voor een Azure monitor-activiteiten logboek maken om op de hoogte te worden gesteld wanneer uw RBAC-toegang wordt verwijderd uit het CSP-abonnement.

### <a name="create-an-azure-monitor-alert"></a>Een Azure monitor-waarschuwing maken

1. Maak een waarschuwing.

   :::image type="content" source="images/azure/azurealert1.png" alt-text="Azure-waarschuwing":::

2. Selecteer het type actie dat door de waarschuwing moet worden uitgevoerd. Als u bijvoorbeeld opgeeft dat u een e-mail bericht wilt ontvangen, ontvangt u een e-mail met de melding dat er een roltoewijzing wordt verwijderd.

   :::image type="content" source="images/azure/azureconfigurealert2.png" alt-text="waarschuwing configureren":::

### <a name="aobo-removal"></a>ADMINISTRATE verwijderen

Klanten kunnen de toegang tot hun abonnementen beheren door te gaan naar **Access Control** op de Azure Portal. Op het tabblad **roltoewijzingen** selecteert u **toegang verwijderen**. Als dit het geval is, kunt u het volgende doen:

- Neem contact op met uw klant om te zien of de beheerders toegang kan worden hersteld.

- Gebruik de toegang die is verschaft via [op rollen gebaseerd toegangs beheer (RBAC)](/azure/role-based-access-control/overview).

- Gebruik toegang via [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

Op rollen gebaseerde toegang verschilt van beheerders toegang. Rollen kunnen nauw keurig worden beperkt wat u wel en niet kunt doen. De toegang tot de beheerder is breder.

Lees de [rollen en machtigingen voor het tegoed van de partner](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2)om de rollen te zien die in aanmerking komen om PEC te verdienen.

## <a name="next-steps"></a>Volgende stappen

- [Beheerders bevoegdheden intrekken en reactiveren voor Azure CSP-abonnementen](revoke-reinstate-csp.md)

- [Creditering van de partner-overzicht](partner-earned-credit.md)

- [Het tegoed van de partner voor beheerde services](partner-earned-credit-explanation.md)
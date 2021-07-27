---
title: Veelgestelde vragen over partnertegoeden
ms.topic: article
ms.date: 07/22/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Vind antwoorden op veelgestelde vragen over partnertegoeden (PEC).
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: e5d6aa77a02a24648828f06fb2c56640abdbfc56
ms.sourcegitcommit: d133c8b923b90ac5518cb989c0ce4dd69713abf4
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/22/2021
ms.locfileid: "114434212"
---
# <a name="frequently-asked-questions-for-partner-earned-credit"></a>Veelgestelde vragen over partnertegoeden

Juiste rollen: Globale | Gebruikersbeheerbeheer | Beheeragent | Factureringsbeheerders | Verkoopagent

Hieronder volgt een lijst met veelgestelde vragen over partnertegoeden.

## <a name="how-much-is-pec"></a>Hoeveel is PEC?

Het bedrag dat partners voor PEC verdienen, varieert (zie [Berekening](partner-earned-credit-explanation.md#calculation)). Het tarief vindt u op de pagina prijslijst in Partner Center.

## <a name="what-azure-services-are-eligible-for-pec"></a>Welke Azure-services komen in aanmerking voor PEC?

PEC komt in aanmerking voor alle services die betrekking hebben op de nieuwe Azure-aanbieding in CSP (Azure-plan), met uitzondering van het volgende: 
- Reserveringen voor nieuwe Azure-aanbieding (Azure-abonnement)
- Producten van derden die zijn geïdentificeerd als derden in de kolom Tags van de lijst met prijzen voor azure-planverbruik
- Producten in de marketplace-prijslijst
- [Azure Spot Virtual Machines](https://partner.microsoft.com/resources/collection/azure-spot-in-csp#/)

## <a name="where-can-i-see-pec"></a>Waar kan ik PEC zien?

Zie [Berekening.](partner-earned-credit-explanation.md#calculation)

## <a name="where-can-i-find-pec-details"></a>Waar vind ik PEC-gegevens?

PEC-gegevens kunnen rechtstreeks door partners worden opgevraagd via API, dagelijks [reconbestand](partner-earned-credit-explanation.md#calculation) en [ACM (Azure Cost Mgmt).](partner-earned-credit-explanation.md#azure-cost-management-and-pec)

## <a name="how-can-i-reconcile-my-pec-information-across-the-two-recon-files"></a>Hoe kan ik mijn PEC-gegevens afstemmen voor de twee recon-bestanden?

Er zijn twee afstemmingsbestanden in Partner Center onder Facturering die kunnen worden gebruikt.

- Dagelijks beoordeeld gebruik afstemmen op recente activiteit (.csv)
- Afstemming-recente activiteit (.csv)

Voor afstemming kan de partner de velden ProductID, SKUID en AvailabilityID uit deze twee bestanden vergelijken voor elke SubscriptionID.

## <a name="for-an-indirect-reseller-working-with-an-indirect-provider-does-an-indirect-provider-need-to-add-the-indirect-resellers-account-as-an-rbac-identity-and-access-management-iam-role-to-the-end-customers-subscription-in-order-to-utilize-acm"></a>Moet een indirecte provider voor een indirecte reseller die met een indirecte provider werkt, het account van de indirecte reseller als een IAM-rol (RBAC Identity and Access Management) toevoegen aan het abonnement van de eindklant om ACM te kunnen gebruiken?

Ja, de CSP Indirect Provider moet [RBAC-toegang](/azure/role-based-access-control/overview) tot de indirecte reseller inschakelen voor het Azure-abonnement.

## <a name="what-happens-if-a-customer-removes-a-partners-rbac-admin-access"></a>Wat gebeurt er als een klant de RBAC-beheerderstoegang van een partner verwijdert?

Een partner zonder de juiste RBAC-toegang in CSP behoudt nog steeds de Azure-factureringsrelatie en verantwoordelijkheid van de klant met Microsoft. Hoewel dit geen invloed heeft op een partner die de vorige Azure-aanbieding in CSP verkoopt, komt de gefactureerde partner voor de nieuwe Azure-aanbieding in CSP niet in aanmerking voor PEC op hun Azure-factuur. Partners kunnen gedeeltelijke beheerderstoegang verkrijgen in CSP door toegang te verkrijgen via een gebruikersaccount via directory-/gasttoegang met behulp van RBAC of via Azure Lighthouse. Zie Beheerdersbevoegdheden voor de Azure CSP van [een klant herstellen voor meer informatie.](revoke-reinstate-csp.md)

## <a name="how-do-i-know-if-im-earning-pec"></a>Hoe kan ik weten of ik PEC verdien?

Er zijn verschillende manieren waarop een partner kan bevestigen dat deze de juiste toegang heeft tot de Azure-resources van een klant.

- Bekijk het dagelijkse gebruiksbestand: als een partner het partnertegoed voor beheerde services ontvangt, heeft deze partner beheerderstoegang. Dit kan worden bepaald door de eenheidsprijs en de effectieve eenheidsprijs in het dagelijkse gebruiksbestand te controleren en te controleren of er korting wordt toegepast.
- Een waarschuwing voor Azure Monitor maken: [](/azure/azure-monitor/platform/alerts-activity-log) u kunt waarschuwingen voor activiteitenlogboek maken met behulp van Azure Monitor om meldingen te ontvangen wanneer uw RBAC-toegang wordt verwijderd uit CSP-abonnementen. Raadpleeg de handleiding partnertegoeden en technische documentatie.

## <a name="why-dont-i-see-pec-on-the-invoice"></a>Waarom zie ik PEC niet op de factuur?

PEC wordt niet expliciet vermeld op de factuur en er is geen afzonderlijk regelitem om PEC weer te geven, maar PEC-inkomsten worden in rekening gebracht in het aangepaste nettokostenbedrag op de factuur. Bekijk de secties berekening en Hoe is PEC betaald voor meer informatie over waar u PEC-details kunt bekijken.

## <a name="next-steps"></a>Volgende stappen

- [Prijslijst voor de nieuwe commerce-ervaring voor Azure in CSP](azure-plan-price-list.md)
- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)
- [Nieuwe Commerce-ervaring in CSP - Azure-facturering](azure-plan-billing.md)
- [Beheerdersbevoegdheden voor Azure CSP-abonnementen opnieuw instellen](revoke-reinstate-csp.md)
- [Partnertegoed - overzicht](partner-earned-credit.md)
- [Rollen, machtigingen voor partnertegoed](azure-roles-perms-pec.md)
- [Inzicht in partnertegoed (handleiding)](https://partner.microsoft.com/resources/detail/understanding-partner-earned-credit-pdf) (aanmelding vereist)

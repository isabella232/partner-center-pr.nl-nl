---
title: Beginnen met de overstap naar het Azure-plan
description: Ontdek wat u en uw klanten moeten weten over het gebruik van het Azure-abonnement voor betalen per gebruik, inclusief de eerste stappen, voorzorgsmaatregelen en hoe u aan de slag kunt gaan.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: ca7b72e653af37307d3a2985ac57783b050ff408204a14d977ec7a5ec29dab77
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691222"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Beginnen met betalen per gebruik-tarieven met het Azure-plan

**Juiste rollen:** beheeragent | Verkoopagent


Microsoft heeft een nieuwe commerce-ervaring in Partner Center.  Met deze nieuwe commerce-ervaring krijgen partners toegang tot Azure-services tegen tarieven voor betalen per gebruik voor klanten onder de Microsoft-klantovereenkomst.

Dit plan vereenvoudigt de aankoopervaring: u kunt meerdere Azure-abonnementen in een Azure-abonnement hebben. U hoeft geen afzonderlijke order meer per Azure-abonnement in te dienen. En in deze nieuwe commerce-ervaring voor Azure zijn we afgestemd op één globaal prijsprincipe waarmee CSP-partners Azure tegen de gepubliceerde prijzen kunnen aanbieden.

Voor de digitale transformatiebehoeften van onze klanten zijn nieuwe vaardigheden van partners vereist. Veel klanten zoeken partners om services te bieden die zich boven en buiten de transactie kunnen ontwikkelen om hun cloudtraject soepeler te laten verlopen en azure-services efficiënt te gebruiken. Microsoft-partners spelen een cruciale rol in alle fasen van de levenscyclus van de klant. Dit soort partnerservices zijn van nature en omvatten Azure Estate Monitoring, beleid en beheer van governance, het instellen en configureren van afstemming, technische ondersteuning en tal van andere services. Ze vereisen dat een partner nauw vertrouwd is met de Azure-omgeving van de klant en continue en juiste governance en controle heeft over de onderliggende resources die ze beheren. Factureringspartners die 24 x 7 cloudbewerkingen beheren, komen in aanmerking voor partnertegoed voor **services die** voor dat werk worden beheerd.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Zorg ervoor dat uw klanten de Microsoft-klantovereenkomst

Sinds 1 oktober 2019 is de Microsoft-klantovereenkomst een doorlopende overeenkomst beschikbaar die de aankoopervaring van klanten vereenvoudigt en stroomlijnt met een volledig digitaal proces. Alle klanten die willen profiteren van de nieuwe commerce-ervaring in CSP voor Azure, moeten de Microsoft-klantovereenkomst.

Partners die het nieuwe Azure-plan willen uitvoeren en een nieuwe order willen plaatsen, moeten de klantacceptatie van de Microsoft-klantovereenkomst bevestigen met behulp van het Partner Center-dashboard en de API in productie.

Vanaf 1 februari 2020 wordt de bestaande Microsoft Cloud-overeenkomst verwijderd uit het CSP-programma. Vanaf dat moment is partnerbevestiging (attestation) van de acceptatie van de klant voor de nieuwe Microsoft-klantovereenkomst vereist voor alle andere aanbiedingen, waaronder Microsoft 365, Dynamics 365 en bestaande Azure. Partners in de CSP kunnen geen nieuwe bestelling voor de klant maken zonder attestation van de Microsoft-klantovereenkomst.

Lees Acceptatie van [klantacceptatie van de Microsoft-klantovereenkomst](confirm-customer-agreement.md) voor meer Microsoft-klantovereenkomst

## <a name="security-and-access-control-practices"></a>Beveiligings- en toegangsbeheerprocedures

Ter bescherming van partners en klanten introduceren we een aantal verplichte beveiligingsvereisten voor adviseurs, Configuratiescherm-leveranciers en partners die deelnemen aan het Cloud Solution Provider-programma.

Partners die de verplichte beveiligingsvereisten niet implementeren, kunnen het Cloud Solution Provider-programma niet uitvoeren of tenants van klanten beheren die gebruikmaken van gedelegeerde beheerdersrechten zodra deze vereisten worden afgedwongen. Er wordt een technische afdwingingsdatum voor de vereisten gemaakt en partners worden op de hoogte gesteld van de datum met gedetailleerde informatie.

## <a name="actions-to-take-to-implement-mfa"></a>Acties die moeten worden ondernomen om MFA te implementeren

Gezien de zeer bevoegde aard van een partner moeten we ervoor zorgen dat elke gebruiker een MFA-uitdaging heeft voor elke afzonderlijke verificatie. Dit kan op een van de volgende manieren worden bereikt:

- Implementatie van Azure AD Premium en ervoor zorgen dat meervoudige verificatie (MFA) wordt afgedwongen voor elke gebruiker
- De standaardinstellingen voor [Azure AD-beveiliging implementeren](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Een oplossing van derden implementeren en ervoor zorgen dat MFA wordt afgedwongen voor elke gebruiker

Vanaf 1 augustus 2019 moeten alle partners meervoudige verificatie afdwingen voor alle gebruikers, inclusief serviceaccounts, in hun partner-tenant. Gedetailleerde informatie over deze beveiligingsvereisten vindt u in [Beveiligingsvereisten van partners.](partner-security-requirements.md)

Microsoft raadt partners aan om zorgvuldig gebruik te maken van RBAC, volgens best practices die zijn ingeschakeld via [Azure Active Directory Privileged Identity Management resources.](/azure/active-directory/privileged-identity-management/pim-configure)

## <a name="read-more-about-the-azure-plan"></a>Meer informatie over het Azure-plan

- [Het Azure-abonnement kopen](purchase-azure-plan.md)

- [Azure-aanbiedingen vergelijken](compare-azure-offers.md)

- [Partnertegoed - overzicht](partner-earned-credit.md)

- De partnertegoedberekeningen (PEC) en de rollen en machtigingen die in aanmerking komen om partnertegoeden te verdienen, zijn beschikbaar in de prijslijst van uw Partner Center Dashboard (aanmelden vereist).

## <a name="next-steps"></a>Volgende stappen 

- [Hoe het partnertegoed wordt bepaald - details](partner-earned-credit-explanation.md)
- [Prijslijst voor Azure-abonnement uitgelegd](azure-plan-price-list.md)
- [Transition your customer to Azure plan](azure-plan-transition.md) (Uw klanten laten overstappen naar een Azure-plan)
- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)
- [De volledige lijst met landen/regio's waar het Azure-plan beschikbaar is](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)
---
title: Begin met uw overstap naar het Azure-abonnement
description: Meer informatie over wat u en uw klanten moeten weten over het gebruik van het Azure betalen per gebruik-abonnement, met inbegrip van de eerste stappen, beveiligings maatregelen en hoe u aan de slag gaat.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 5ad7bd7c99d7caa044877c98aac6dc5e3ce69420
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528598"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Beginnen met betalen naar gebruik-tarieven met het Azure-abonnement

Micro soft heeft een nieuwe Commerce ervaring geïntroduceerd in Partner Center.  Met deze nieuwe Commerce-ervaring krijgen partners toegang tot Azure-Services tegen betalen per gebruik-tarieven voor klanten onder de klant overeenkomst van micro soft.

Dit plan vereenvoudigt de koop ervaring: u kunt meerdere Azure-abonnementen in een Azure-abonnement hebben. U hoeft niet langer een afzonderlijke order per Azure-abonnement in te dienen. En in deze nieuwe Commerce-ervaring voor Azure zijn we afgestemd op één wereld wijd prijs beginsel waardoor CSP-partners Azure kunnen aanbieden tegen de gepubliceerde prijzen.

De digitale trans formatie behoeften van onze klanten vereisen nieuwe vaardig heden van partners. Veel klanten kijken naar partners voor het leveren van services boven en buiten de trans actie om hun Cloud reis soepeler te maken en Azure-Services efficiënt te gebruiken. Micro soft-partners spelen een cruciale rol in alle fasen van de levens cyclus van de klant. Dit soort partner Services is aan het volgen van zaken en omvat de bewaking, het beleid en het beheer van Azure-instellingen, het instellen en configureren van fijnafstelling, technische ondersteuning en diverse andere services. Ze hebben een partner nodig om bekend te zijn met de Azure-omgeving van de klant en voortdurend en passend governance en controle te hebben van de onderliggende resources die ze beheren. Facturerings partners die dit 24 X 7 Cloud-Operations-beheer leveren, komen in aanmerking voor een partner die een tegoed heeft ontvangen **voor services** die worden beheerd voor die werkzaamheden.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Zorg ervoor dat uw klanten de micro soft-klant overeenkomst hebben ondertekend

Sinds 1 oktober 2019 is de micro soft-klant overeenkomst een permanente overeenkomst waarmee de klant aankoop ervaring met een volledig digitaal proces wordt vereenvoudigd en gestroomlijnd. Alle klanten die willen profiteren van de nieuwe Commerce ervaring in CSP voor Azure, moeten de micro soft-klant overeenkomst ondertekenen.

Partners die willen handelen onder het nieuwe Azure-plan en een nieuwe order moeten maken, moeten de acceptatie van klanten bevestigen van de micro soft-klant overeenkomst met behulp van het dash board en de API voor de productie van het partner centrum.

Vanaf 1 februari 2020 wordt de bestaande Microsoft Cloud overeenkomst verwijderd uit het CSP-programma. Vanaf dat moment is partner bevestiging (Attestation) van de acceptatie van de klant voor de nieuwe micro soft-klant overeenkomst vereist voor alle andere aanbiedingen, waaronder Microsoft 365, Dynamics 365 en bestaande Azure. Partners in de CSP kunnen geen nieuwe order voor de klant maken zonder dat de micro soft-klant overeenkomst is attest.

Lees voor meer informatie [klant acceptatie van de micro soft-klant overeenkomst bevestigen](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Procedures voor beveiliging en toegangs beheer

Om partners en klanten te helpen beschermen, introduceren we een reeks verplichte beveiligings vereisten voor Advisor, leveranciers van het configuratie scherm en partners die deel nemen aan het programma voor Cloud solution provider.

Partners die de verplichte beveiligings vereisten niet implementeren, kunnen geen trans acties uitvoeren in het Cloud Solution Provider-programma of de tenants van klanten beheren die gebruikmaken van gedelegeerde beheerders rechten, zodra deze vereisten worden afgedwongen. We zijn bezig met het opstellen van een technische afdwingings datum voor de vereisten en zullen de partners van de datum op de hoogte stellen met gedetailleerde informatie.

## <a name="actions-to-take-to-implement-mfa"></a>Acties die moeten worden uitgevoerd om MFA te implementeren

Gezien de zeer beschermde aard van een partner moeten we ervoor zorgen dat elke gebruiker een MFA-uitdaging voor elke afzonderlijke verificatie heeft. U kunt dit op een van de volgende manieren doen:

- Azure AD Premium implementeren en ervoor zorgen dat multi-factor Authentication (MFA) wordt afgedwongen voor elke gebruiker
- Implementatie van de [standaard instellingen voor Azure AD-beveiliging](/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementatie van een oplossing van derden en ervoor zorgen dat MFA wordt afgedwongen voor elke gebruiker

Vanaf 1 augustus 2019 zijn alle partners vereist voor het afdwingen van multi-factor Authentication voor alle gebruikers, inclusief service accounts, in hun partner Tenant. Meer informatie over deze beveiligings vereisten vindt u op [beveiligings vereisten van partners](partner-security-requirements.md).

Micro soft raadt partners aan om met behulp van de best practices die via [Azure Active Directory privileged Identity Management resources](/azure/active-directory/privileged-identity-management/pim-configure)zijn ingeschakeld, gebruik te maken van RBAC.

## <a name="read-more-about-the-azure-plan"></a>Meer informatie over het Azure-abonnement

- [Het Azure-abonnement kopen](purchase-azure-plan.md)

- [Azure-aanbiedingen vergelijken](compare-azure-offers.md)

- [Creditering van de partner-overzicht](partner-earned-credit.md)

- De berekening van de door de partner gehaalde credit (PEC) en de rollen en machtigingen die in aanmerking komen voor het verdienen van de aangekeerde tegoeden van de partner zijn beschikbaar via de prijs lijst van uw partner Center-dash board (aanmelden is vereist).

## <a name="next-steps"></a>Volgende stappen 

- [Hoe het tegoed van de partner wordt bepaald: Details](partner-earned-credit-explanation.md)
- [Uitleg prijzen lijst voor Azure plan](azure-plan-price-list.md)
- [Transition your customer to Azure plan](azure-plan-transition.md) (Uw klanten laten overstappen naar een Azure-plan)
- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)
- [De volledige lijst met landen/regio's waar het Azure-abonnement beschikbaar is](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)
---
title: Software en oplossingen kopen vanuit Azure Marketplace
description: Meer informatie over hulpprogram ma's voor het vereenvoudigen en stroom lijnen van software-aankopen en-beheer in azure Marketplace.
ms.prod: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 01/18/2021
ms.openlocfilehash: de58fad7af7dd2cd6b8c98e5763557d54cc776a2
ms.sourcegitcommit: c46658f4d70004596e758fe4cd8671b6e9dadeab
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/20/2021
ms.locfileid: "98584208"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace-aankopen

Azure Marketplace heeft talloze hulpprogram ma's en functies waarmee het proces van het kopen, factureren en beheren van inkoop beleid wordt vereenvoudigd en gestroomlijnd.

## <a name="simplified-procurement"></a>Vereenvoudigde aanschaf

Met Azure Marketplace kunt u het aankoopproces vereenvoudigen via verschillende aankoopopties. Als u producten koopt met een credit card die is gekoppeld aan uw Azure-account, worden alle aankopen geconsolideerd op één factuur en gefactureerd met de keuze van de credit card. Als u een grote klant bent, kunt u kopen via een Enterprise Agreement. Met een EA worden software aankopen automatisch opgenomen in uw Azure-factuur. Uw factuur bevat eerst de gebruikskosten voor Azure, gevolgd door de kosten voor Azure Marketplace.

Wanneer u via Azure Marketplace koopt, elimineert u de complexiteit van het beheer van afzonderlijke leveranciers relaties en-facturen. U krijgt één geconsolideerde maandelijkse factuur van micro soft waarin zowel uw Azure Marketplace-aankopen als uw Azure-kosten zijn opgenomen.

## <a name="permission-to-purchase"></a>Machtiging voor aankoop

Nadat u de juiste software toepassing hebt gevonden, is het volt ooien van de aankoop eenvoudig. U hebt echter wel de juiste machtigingen nodig in het Azure-abonnement. Omdat Azure wordt uitgevoerd op een [op rol gebaseerd Access Control](/azure/role-based-access-control/overview) model (RBAC), hebben uw account de eigenaar van het **abonnement** of de machtiging **Inzender** nodig om een aankoop te doen.

Voordat u een aankoop voltooit, controleert u of de gebruiker de juiste configuratie heeft in de Azure-Tenant. Dit helpt bij het voor komen van fouten tijdens de aankoop.

Zoek in de Azure Marketplace-ervaring in het Azure Portal naar de toepassing die u wilt kopen en selecteer **maken** of **instellen en abonneren**. U wordt gevraagd om informatie te volt ooien voordat u uw nieuwe oplossing kunt gebruiken.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="De knop voor het maken van de aanbieding.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="De knop instellen en abonneren.":::

Als u een oplossing wilt implementeren vanuit de online winkel voor Azure Marketplace, selecteert u **nu downloaden** op de pagina product beschrijving en meldt u zich aan met de referenties van uw Azure-account.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Het dialoog venster Aanmelden bij Azure Marketplace.":::

Zodra u zich hebt aangemeld, wordt u omgeleid naar het product in de Azure Portal om uw aankoop te volt ooien.

## <a name="purchase-policy-management"></a>Aankoop beleids beheer

Micro soft biedt u de mogelijkheid om gebruikers aankopen via uw facturerings profiel te beheren als de beheerder van het Azure-abonnement. U kunt kiezen uit drie opties:

- **Gratis + betaald** : Hiermee kunnen gebruikers een Azure Marketplace-software toepassing verkrijgen.
- **Gratis** : Hiermee kunnen gebruikers alleen gratis software van Azure Marketplace implementeren.
- **Nee** : hiermee voor komt u dat gebruikers software van Azure Marketplace implementeren.

Deze instellingen zijn van toepassing op alle gebruikers met toegang tot uw Azure-abonnement. Dit biedt u de mogelijkheid om de IT-aankopen via de Azure Portal te beheren.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="IT-aankopen beheren via de Azure Portal":::

## <a name="cost-management"></a>Kostenbeheer

Wanneer u producten aanschaft vanuit Azure Marketplace, wilt u inzichten krijgen die u helpen bij het beheren van de kosten. Azure Cost Management is een gratis hulp programma voor het weer geven van informatie over de producten die u hebt aangeschaft. U kunt Cost Management gebruiken om details te bekijken van de services die u in de loop van de tijd wilt best Eden en hoe deze kosten volgen op de budgetten die u hebt ingesteld. Naast het instellen van budgetten kunt u ook rapporten plannen en abonnements kosten analyseren. Meer informatie over Azure Cost Management door het volt ooien van de Microsoft Learn module voor het [analyseren van kosten en het maken van budgetten met Azure Cost Management](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

U kunt de kosten en facturen van uw Azure Marketplace bekijken via het hulpprogramma kostenanalyse onder Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Gebruik Azure Cost Management om inzicht te krijgen in uw gekochte producten.":::

## <a name="purchase-validation-checks"></a>Validatie controles voor aankoop

Het kopen van een aanbieding via Azure Marketplace kan om verschillende redenen mislukken. Het gebruik van de opdracht regel interface (CLI) voor een aankoop heeft waarschijnlijk veel problemen als gevolg van het aanschaffen van een aanbieding die niet beschikbaar of zichtbaar is in azure Marketplace. Hieronder ziet u de controles die ertoe kunnen leiden dat een aankoop mislukt:

1. Het abonnement hoort bij een Enterprise Agreement (EA) en de EA-beheerder uitgeschakeld Azure Marketplace-aankopen.
1. De EA-beheerder heeft aankopen alleen voor gratis aanbiedingen ingeschakeld en de aanbieding is een betaalde aanbieding.
1. De aanbieding is niet gevonden in de Marketplace.
1. De Independent Software Vendor (ISV) is gestopt met het verkopen van de aanbieding, ten minste in uw regio.
1. Het abonnement dat u gebruikt, behoort tot een facturerings account in een regio waarin de aanbieding niet beschikbaar is.
1. Het abonnement/facturerings account is niet gekoppeld aan een geldig betalings middel (zoals een geldige credit card).
1. Het abonnement behoort tot een Cloud Solution Provider (CSP) en de ISV heeft geweigerd om via een CSP te verkopen.
1. Privé Marketplace is ingeschakeld voor het abonnement en de aanbieding bevindt zich niet in de lijst met toegestane aanbiedingen.
1. De aanbieding is privé/Preview voor specifieke klanten en het abonnement bevindt zich niet in de lijst met toegestane klanten.

## <a name="next-steps"></a>Volgende stappen

- [Facturering](billing-invoicing.md)
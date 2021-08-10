---
title: Software en oplossingen van Azure Marketplace
description: Meer informatie over hulpprogramma's die software-aankopen en -beheer vereenvoudigen en stroomlijnen in Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 06/22/2021
ms.openlocfilehash: 029d68f2d33453f760e353bb0eb7a0f59df82fb887ef49d57c0b6c8f4bbe9d9a
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115689049"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace aanschaffen

Azure Marketplace beschikt over talloze hulpprogramma's en functies die het aankoopproces, de facturering en het beheer van het aankoopbeleid vereenvoudigen en stroomlijnen.

## <a name="simplified-procurement"></a>Vereenvoudigde inkoop

Met Azure Marketplace kunt u het aankoopproces vereenvoudigen via verschillende aankoopopties. Als u producten koopt met een creditcard die is gekoppeld aan uw Azure-account, worden alle aankopen geconsolideerd op één factuur en gefactureerd op de creditcard van uw keuze. Als u een grote klant bent, kunt u kopen met behulp van een Enterprise Agreement. Met een EA worden software-aankopen automatisch opgenomen in uw Azure-factuur. Uw factuur bevat eerst de gebruikskosten voor Azure, gevolgd door de kosten voor Azure Marketplace.

Wanneer u aanschaft via Azure Marketplace, elimineert u de complexiteit van het beheren van relaties en facturen van afzonderlijke leveranciers. U krijgt één geconsolideerde maandelijkse factuur van Microsoft die zowel uw Azure Marketplace als uw Azure-kosten omvat.

## <a name="permission-to-purchase"></a>Machtiging om aan te schaffen

Nadat u de juiste softwaretoepassing hebt gevonden, is het voltooien van de aankoop eenvoudig. U hebt echter geschikte machtigingen nodig binnen het Azure-abonnement. Omdat Azure werkt met een op rollen gebaseerd [Access Control](/azure/role-based-access-control/overview) (RBAC) model, heeft uw account machtigingen van de eigenaar van het abonnement of inzender nodig om een aankoop te doen.  

Voordat u een aankoop voltooit, moet u ervoor zorgen dat de gebruiker de juiste configuratie heeft in de Azure-tenant. Dit helpt bij het voorkomen van fouten tijdens de aankoop.

Zoek in Azure Marketplace in de Azure Portal de toepassing die u wilt kopen  en selecteer Maken of **Instellen en abonneren.** U wordt gevraagd om wat informatie in te vullen voordat u uw nieuwe oplossing kunt gebruiken.

> [!CAUTION]
> Goedkeuring in Private Marketplace duidt niet op de aanschaf van een oplossing.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="De knop Maken van aanbieding.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="De knop Instellen en abonneren.":::

Als u een oplossing wilt implementeren vanuit de Azure Marketplace  Online Store, selecteert u Nu downloaden op de pagina productbeschrijving en meld u vervolgens aan met de referenties van uw Azure-account.

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="Het Azure Marketplace aanmeldingsvenster.":::

Nadat u zich hebt aanmelden, wordt u omgeleid naar het product in de Azure Portal om uw aankoop te voltooien.

## <a name="purchase-policy-management"></a>Beheer van aankoopbeleid

Met Microsoft kunt u gebruikersaankopen beheren via uw factureringsprofiel als de beheerder van het Azure-abonnement. Kies uit drie opties:

- **Gratis en betaald:** hiermee kunnen gebruikers alle Azure Marketplace verkrijgen.
- **Gratis:** hiermee kunnen gebruikers alleen gratis software van Azure Marketplace.
- **Nee:** hiermee voorkomt u dat gebruikers software implementeren vanuit Azure Marketplace.

Deze instellingen zijn van toepassing op alle gebruikers met toegang tot uw Azure-abonnement, zodat u de it-aanschaf kunt beheren via de Azure Portal.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="It-inkoop beheren via de Azure Portal.":::

## <a name="cost-management"></a>Kostenbeheer

Wanneer u producten van Azure Marketplace, wilt u inzichten krijgen die u helpen kosten te beheren. Azure Cost Management is een gratis hulpprogramma voor het weergeven van informatie over de producten die u hebt aangeschaft. U kunt Cost Management om details te bekijken van de services waar u in de afgelopen tijd geld aan uit geeft en hoe deze kosten worden afgenomen ten opzichte van de budgetten die u hebt ingesteld. Naast het instellen van budgetten kunt u rapporten plannen en abonnementskosten analyseren. Meer informatie over Azure Cost Management door de module Microsoft Learn kosten analyseren en [budgetten maken](/learn/modules/analyze-costs-create-budgets-azure-cost-management/)met Azure Cost Management.

U kunt de kosten en facturen van uw Azure Marketplace bekijken via het hulpprogramma kostenanalyse onder Azure Cost Management.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Gebruik Azure Cost Management om inzicht te krijgen in uw aangeschafte producten.":::

## <a name="purchase-validation-checks"></a>Validatiecontroles voor aankopen

Het aanschaffen van een aanbieding via Azure Marketplace kan om verschillende redenen mislukken. Het gebruik van de opdrachtregelinterface (CLI) voor een aankoop veroorzaakt waarschijnlijk meer fouten, omdat u mogelijk probeert een aanbieding aan te schaffen die niet beschikbaar is of zichtbaar is in Azure Marketplace. Hieronder vindt u de controles die ertoe kunnen leiden dat een aankoop mislukt:

1. Het abonnement behoort tot een Enterprise Agreement (EA) en de EA-beheerder heeft Azure Marketplace uitgeschakeld.
1. De EA-beheerder heeft aankopen alleen ingeschakeld voor gratis aanbiedingen en de aanbieding is een betaalde aanbieding.
1. De aanbieding is niet gevonden in de marketplace.
1. De Onafhankelijke softwareleverancier (ISV) is gestopt met het verkopen van de aanbieding, ten minste in uw regio.
1. Het abonnement dat u gebruikt, behoort tot een factureringsaccount in een regio waarin de aanbieding niet beschikbaar is.
1. Het abonnement/de factureringsrekening is niet gekoppeld aan een geldig betaalmiddel (zoals een geldige creditcard).
1. Het abonnement behoort tot een Cloud Solution Provider (CSP) en de ISV heeft geweigerd om te verkopen via een CSP.
1. Private Marketplace is ingeschakeld voor het abonnement en de aanbieding staat niet in de lijst met toegestane aanbiedingen.
1. De aanbieding is Privé/Preview voor specifieke klanten en het abonnement staat niet in de lijst met toegestane klanten.

> [!NOTE]
> Het kopen van Marketplace-aanbiedingen kan mislukken als er een conflict is Azure Policy door de Azure-beheerder in uw organisatie is gedefinieerd. U kunt bijvoorbeeld Geen Microsoft.SaaS aanschaffen als deze niet in de lijst met toegestane toepassingen van **uw organisatie** staat. Zie de Azure Policy [voor meer informatie.](/azure/governance/policy/)

## <a name="next-steps"></a>Volgende stappen

- [Facturering](billing-invoicing.md)
---
title: Levenscyclusbeheer van SaaS-abonnementen (Software as a Service)
description: Levenscyclusbeheer van SaaS-abonnementen (Software as a Service) in Azure Marketplace.
ms.service: marketplace
ms.subservice: partnercenter-marketplace-publisher
ms.topic: conceptual
ms.date: 08/20/2021
ms.author: yonits
author: yonits
ms.openlocfilehash: e0cd29d9fe36d4f81307594f7fd8ab948d56adf7
ms.sourcegitcommit: 38afe7e35e3dce4f35cf7352cc98e3d53e979a62
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/23/2021
ms.locfileid: "122752703"
---
# <a name="saas-subscription-lifecycle-management"></a>Levenscyclusbeheer voor SaaS-abonnementen

In dit artikel wordt beschreven hoe u een SaaS-resource detecteert, wat de verschillen zijn tussen SaaS en het klassieke SaaS-resourcebeheer en saaS-resourcebeheer in Azure Portal.

## <a name="find-a-saas-resource"></a>Een SaaS-resource zoeken

Wanneer u een SaaS-aanbieding aanschaft bij Azure Marketplace, wordt er een SaaS-abonnement (Software as a Service) gemaakt in de Azure Portal (zie [Een SaaS-aanbieding](purchase-saas-offer-in-azure-portal.md)kopen in Azure Portal). Een SaaS-resource zoeken in de portal:

- **Algemeen zoekvenster** (boven) : zoek uw SaaS-abonnement op naam.
- **SaaS:** geeft al uw SaaS-abonnementen weer. Er zijn twee typen SaaS-lijsten: zie de volgende sectie.
- **Abonnementen:** geeft een lijst weer van alle Azure-abonnementen tot wie u toegang hebt als onderdeel van uw tenant. Als u een specifiek abonnement wilt zoeken, gebruikt u het filter- of zoekvenster.
- **Alle resources:** geeft een lijst weer van alle resources die zijn gemaakt onder alle abonnementen tot wie u toegang hebt. Als u een specifiek abonnement wilt zoeken, gebruikt u het filter (Type > SaaS) of zoekt u in de lijst.

## <a name="differences-between-saas-and-saas-classic-lists-of-resources-in-the-azure-portal"></a>Verschillen tussen de klassieke SaaS- en SaaS-lijsten met resources in de Azure Portal

Het verschil tussen deze twee typen is dat u met de klassieke SaaS-abonnementen de SaaS-abonnementen kunt vinden die zijn gemaakt onder uw tenant en niet onder een resourcegroep.
Als u vóór februari 2021 een SaaS-abonnement hebt aangeschaft in de Azure Portal, is het onder uw tenant gemaakt en kunt u het vinden onder De klassieke SaaS-versie. Alle aankopen die in Microsoft AppSource worden gedaan, staan in deze lijst.

Als u vóór februari 2021 een SaaS-abonnement hebt aangeschaft in de Azure Portal en u dit wilt verplaatsen van onder de tenant naar een resourcegroep (aanbevolen), gaat u naar het SaaS-abonnement in de klassieke **SaaS-sectie** en selecteert u Verplaatsen **naar resourcegroep**. U kunt alleen abonnementen met de status In **behandeling** **of Actief** verplaatsen. Na de overstap wordt het SaaS-abonnement nu weergegeven in de **SaaS-weergave,** niet in **de klassieke SaaS-versie.** U kunt een SaaS-abonnement niet verplaatsen naar een resourcegroep als het is gekocht in AppSource.

Deze overstap biedt de volgende voordelen:

- Verbeterde toegang tot en beheer van uw SaaS-resource met overgenomen beleidsregels en machtigingen van het Azure-abonnement en resourcegroepen (volledig RBAC-beheer)
- De levenscyclus van SaaS is gekoppeld aan de levenscyclus van het Azure-abonnement voor acties zoals overdrachten en verwijderingen
- Eenvoudiger vindbaarheid, met SaaS-resources die zijn gevonden met algemene zoekopdracht
- Gebruik van Azure Cost Management: uitgaven voor SaaS-resources bewaken
- Resources op abonnementsniveau hebben resourcesgebeurtenissen in activiteitenlogboek

## <a name="manage-your-saas-service"></a>Uw SaaS-service beheren

Er zijn meerdere manieren om uw SaaS-abonnementen te beheren

* Voor SaaS-abonnementen die in de Azure Portal, moet u deze daar beheren.
* Voor SaaS-abonnementen die zijn aangeschaft in AppSource, beheert u deze in het Azure Portal en [het Microsoft 365-beheer Center;](https://admin.microsoft.com/Adminportal/Home?#/subscriptions) Zie [App-abonnementen](/microsoft-365/commerce/manage-saas-apps?view=o365-worldwide)van derden beheren voor uw organisatie voor meer informatie over het gebruik van het Microsoft 365-beheer Center.
* Met sommige uitgevers kunt u SaaS-abonnementen rechtstreeks in hun platform beheren. Ga naar de site van de uitgever via een koppeling op de pagina SaaS-abonnement in de Azure Portal.

Er zijn verschillende acties die u na uw aankoop kunt uitvoeren; Voor sommige zijn de machtigingen Eigenaar of Inzender vereist:

### <a name="change-plans"></a>Plannen wijzigen

Wijzigingen die u aan een abonnement maakt en op wie u bent geabonneerd, worden onmiddellijk van kracht. De facturering wordt naar eigen goed gefactureerd op basis van de factureringsperiode van het huidige abonnement. Voor het wijzigen van abonnementen **zijn eigenaars-** of **inzendermachtigingen** vereist.

> [!NOTE]
> De uitgever kan weigeren de wijziging goed te keuren als de wijzigingen die u selecteert, niet haalbaar zijn binnen de service. In dit geval mislukt de wijziging.

Er zijn enkele gevallen waarin **een wijzigingsplan** mogelijk niet werkt:

- Als uw abonnement onder het  tenantniveau met leesmachtigingen valt, kunt u het plan niet wijzigen. Vraag in dit geval machtigingen aan bij de persoon die de rol **Eigenaar** heeft voor het abonnement.
- Als er geen betaalmiddel (PI) is gekoppeld aan het Azure-abonnement, kunt u uw gratis abonnement niet wijzigen in een betaald abonnement. U kunt echter een ander Azure-abonnement selecteren en vervolgens een betaald abonnement kiezen of een PI toevoegen aan het geselecteerde Azure-abonnement.
- Als het abonnement dat u hebt geselecteerd, een minimale/maximale gebruikersbeperking heeft die niet het huidige aantal gebruikers omvat, selecteert u een ander abonnement met hetzelfde aantal gebruikers dat is opgenomen in het oorspronkelijke abonnement dat u hebt aangeschaft of neemt u contact op met de uitgever.
- Als de uitgever niet aan de aanvraag kan voldoen, kunt u rechtstreeks contact met de uitgever opnemen.

### <a name="change-number-of-users"></a>Aantal gebruikers wijzigen

Voor op seat gebaseerde abonnementen kunt u het aantal gebruikers dat u tijdens het aankoopproces hebt gedefinieerd, toevoegen of verminderen. Het wijzigen van het aantal gebruikers op wie u bent geabonneerd, wordt onmiddellijk van kracht en de facturering wordt pro factureren op basis van de factureringsperiode van het huidige abonnement. Wijzigingen in seats zijn alleen mogelijk binnen het bereik van de minimum- en maximum seats, zoals gedefinieerd door de uitgever. In sommige gevallen moet u een plan wijzigen voordat u van seats wisselt, en vice versa.

- Als uw abonnement onder het tenantniveau met leesmachtigingen valt, kunt u het aantal gebruikers niet wijzigen. Vraag in plaats daarvan inzendermachtigingen aan van de persoon die de rol Eigenaar heeft voor het abonnement.
- Als de uitgever niet aan de aanvraag kan voldoen, kunt u rechtstreeks contact met de uitgever opnemen.

> [!NOTE]
> De uitgever kan weigeren om de wijziging goed te keuren als dit niet haalbaar is binnen de service. In dit geval mislukt de wijziging.

### <a name="edit-recurring-billing"></a>Terugkerende facturering bewerken

Met terugkerende facturering kunt u de verlenging van uw SaaS-abonnement beheren. Wanneer terugkerende facturering is uitgeschakeld, worden het SaaS-abonnement en de service beëindigd op de verlengingsdatum. U kunt de optie voor verlenging alleen wijzigen wanneer het abonnement actief is. Een beëindigd en/of geannuleerd SaaS-abonnement kan niet opnieuw worden geactiveerd; Er moet een nieuw SaaS-abonnement worden gemaakt.

### <a name="view-billing"></a>Facturering weergeven

Bekijk facturen voor uw Azure-abonnement en Azure Marketplace producten die zijn aangeschaft met dit abonnement. Voor SaaS die u hebt aangeschaft in de portal, raadpleegt  u de factureringspagina op de pagina SaaS-abonnement in de sectie Facturering. U wordt dan omgeleid **naar Cost Management**.

Cost Management helpt u inzicht te krijgen in uw factuur uitsplitsing, uw factureringsrekening en abonnementen te beheren, Azure-uitgaven te bewaken/beheren en het resourcegebruik te optimaliseren. Hiermee kunt u kosten analyseren, budgetten maken en beheren, en meer. Hiermee kunt u bijvoorbeeld uw aangepaste metergebruik bijhouden (voor SaaS-abonnementen die zijn gemaakt na februari 2021 of verplaatst naar een resourcegroep). Meer informatie over kostenbeheer kunt u [vinden Azure Cost Management + Billing documentatie](/azure/cost-management-billing/).

Als uw aankoop is gedaan via Microsoft AppSource, kunt u uw facturen weergeven in het Microsoft-beheercentrum onder **Facturen & betalingen.**

### <a name="cancel-subscription"></a>Abonnement annuleren

Als u annuleert, wordt uw toegang tot de software die u hebt aangeschaft als onderdeel van dit SaaS-abonnement verwijderd. Restituties worden verwerkt volgens het restitutiebeleid; Zie Restitutiebeleid voor Microsoft AppSource en Azure Marketplace voor [meer Azure Marketplace.](refund-policies.md)

Als uw abonnement onder het  tenantniveau met leesmachtigingen valt, kunt u een abonnement niet annuleren. Neem in plaats daarvan contact op met de persoon **met eigenaarsmachtigingen.**

Als u meer dan 24 uur een maandelijks SaaS-abonnement hebt of meer dan 14 dagen een jaarlijks of meer jaar-abonnement hebt, wordt er geen restitutie gebruikt voor de huidige termijn van het abonnement (zie annuleringsbeleid). Facturering op basis van verbruik nadat een SaaS-account is geconfigureerd, komt ook niet in aanmerking voor restitutie.

### <a name="delete-subscription"></a>Abonnement verwijderen

Deze actie lijkt op annuleren, met toevoeging van het verwijderen van de SaaS-resource uit uw lijst met SaaS-abonnementen. Nadat u een abonnement hebt verwijderd, hebt u geen toegang meer vanaf de Azure Portal.

Als uw abonnement onder het  tenantniveau met leesmachtigingen valt, kunt u een abonnement niet verwijderen. Neem in plaats daarvan contact op met de persoon **met eigenaarsmachtigingen.**

### <a name="change-azure-subscription-andor-resource-group"></a>Azure-abonnement en/of resourcegroep wijzigen

Als u een abonnement of resourcegroep wilt wijzigen die is gekoppeld aan een aanbieding die is aangeschaft in de Azure Portal:

1. Ga naar de **sectie SaaS.**
2. Selecteer het abonnement dat u wilt wijzigen.
3. Selecteer **onder Facturering** de optie **Gefactureerd abonnement wijzigen.**
4. Selecteer het gewenste abonnement of de gewenste resourcegroep of maak een nieuwe resourcegroep om de SaaS-resource naar te verplaatsen.
5. Selecteer **Wijzigen onderaan** om het proces te voltooien.

Er zijn enkele gevallen waarin de wijziging mogelijk niet werkt:

- Als uw SaaS-abonnement niet de status Geabonneerd heeft, controleert u de status van uw abonnement in de sectie SaaS of op de pagina van uw **SaaS-abonnement.**
- Als het SaaS-abonnement een resource op tenantniveau is:
    - U moet *eigenaars-/inzendermachtigingen* hebben voor het Azure-doelabonnement.
- Als het SaaS-abonnement een resource op abonnementsniveau is:
    - U hebt *de machtiging Lezen* of *Eigenaar/Inzender* nodig voor het Azure-doelabonnement.
    - U hebt *eigenaars-/inzendermachtigingen* nodig voor de doelresourcegroep.
    - Als er al een SaaS-abonnement met dezelfde naam bestaat in de doelresourcegroep, selecteert u een andere doelresourcegroep.
- Het Azure-doelabonnement en het resourceabonnement ondergaan alle controles die tijdens de aankoop worden uitgevoerd. Zie de sectie [SaaS-abonnement](purchase-saas-offer-in-azure-portal.md#saas-subscription-and-configuration) en -configuratie in Een **SaaS-aanbieding** kopen in de sectie Azure Portal.

## <a name="next-steps"></a>Volgende stappen

- Als u al een aanbieding hebt aangeschaft in marketplace, gaat u naar [Facturering en facturering](billing-invoicing.md)
- Meer informatie over opties [voor privé-plannen](private-offers.md)

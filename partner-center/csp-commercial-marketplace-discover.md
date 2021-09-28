---
title: Aanbiedingen ontdekken - commerciële marketplace
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over hoe CSP-partners Partner Center marketplace kunnen bekijken of doorzoeken op SaaS-aanbiedingen of prijzen van ISV's (Independent Software Vendors).
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b4914fa41c58ce9f36fc3ed95f4dc20fae4c769b
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089892"
---
# <a name="discover-offers-and-pricing-in-partner-center-commercial-marketplace"></a>Aanbiedingen en prijzen ontdekken in Partner Center commerciële marketplace

**Juiste rollen:** Globale | Beheeragent

Wanneer onafhankelijke softwareleveranciers (ISV's) ervoor kiezen om een aanbieding te publiceren in de commerciële marketplace, kunnen ze ook bepalen of ze willen dat de aanbieding beschikbaar wordt gesteld in het CSP-programma. Als ze ervoor kiezen om de aanbieding te verkopen via het CSP-programma, moeten CSP-partners de aanbieding zien in Partner Center Marketplace.

Als een ISV-aanbieding niet wordt weergegeven zoals u verwacht in Partner Center, kan dit het volgende zijn:

- De ISV heeft besloten de aanbieding niet te verkopen via het CSP-programma. Sommige ISV-producten zijn bijvoorbeeld beschikbaar gesteld in andere gebieden van de commerciële marketplace (zoals in [Microsoft AppSource](https://appsource.microsoft.com/) en [Azure Marketplace),](https://azuremarketplace.microsoft.com/)maar worden mogelijk niet weergegeven voor partners in het CSP-programma in Partner Center Marketplace.

- De ISV heeft besloten om de aanbieding alleen exclusief te maken voor een select aantal CSP-partners. Zie verder in dit Help-onderwerp voor meer informatie over exclusieve aanbiedingen.

- Het aanbiedingstype kan mogelijk niet worden Partner Center of Azure Portal (bijvoorbeeld containers of sommige aanbiedingen op basis van gebruik).

- Het factureringsland van uw gekoppelde klanten wordt mogelijk niet ondersteund voor deze ISV-aanbieding.

## <a name="view-marketplace-offers-in-partner-center"></a>Marketplace-aanbiedingen weergeven in Partner Center

Beschikbare commerciële marketplace-aanbiedingen in het CSP-programma weergeven:

> [!NOTE]
> Zie Getting around Partner Center voor meer informatie over [de werkruimte-interface.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Werkruimteweergave](#tab/workspaces-view)

1. Meld u aan Partner Center [dashboard en](https://partner.microsoft.com/dashboard) selecteer de **tegel** Prijzen.

2. Selecteer **Marketplace.** Standaard ziet u producten van alle typen en categorieën.

3. Selecteer een filter op type of categorie. U kunt Search ook **gebruiken om** specifieke trefwoorden, namen van aanbiedingsaanbiedingen of de namen van ISV-uitgevers te vinden.

4. Selecteer een specifieke productaanbieding in de lijst. Hiermee gaat u naar een tabblad Overzicht van het product, waar u meer informatie over de aanbieding kunt vinden. Informatie op dit tabblad kan het volgende omvatten:

    - Een beschrijving van het product of de aanbieding

    - Meer informatie over de ISV-uitgever

    - Koppelingen naar documentatie of marketingmateriaal dat is geüpload door de ISV-uitgever

    - Andere mogelijke ISV-contactpersonen voor klantondersteuning, engineering of een contactpersoon voor het CSP-programma

5. Selecteer het tabblad Abonnementen en prijzen voor meer informatie over de beschikbare abonnementen, SKU's of prijzen **van een** aanbieding. Op dit tabblad ziet u het volgende:

    - De markten waar deze aanbieding voor u beschikbaar is

    - Een lijst met SKU's of abonnementen die beschikbaar zijn voor de aanbieding

    - Prijzen voor elke beschikbare SKU of abonnement

#### <a name="current-view"></a>[Huidige weergave](#tab/current-view)

1. Meld u Partner Center [dashboard aan](https://partner.microsoft.com/dashboard)en selecteer **CSP** in het navigatiemenu aan de linkerkant.

2. Selecteer **Verkopen,** gevolgd door **Marketplace.** Standaard ziet u producten van alle typen en categorieën.

3. Selecteer een filter op type of categorie. U kunt Search ook **gebruiken om** specifieke trefwoorden, namen van aanbiedingsaanbiedingen of de namen van ISV-uitgevers te vinden.

4. Selecteer een specifieke productaanbieding in de lijst. Hiermee gaat u naar een tabblad Overzicht van het product, waar u meer informatie over de aanbieding kunt vinden. Informatie op dit tabblad kan het volgende omvatten:

    - Een beschrijving van het product of de aanbieding

    - Meer informatie over de ISV-uitgever

    - Koppelingen naar documentatie of marketingmateriaal dat is geüpload door de ISV-uitgever

    - Andere mogelijke ISV-contactpersonen voor klantondersteuning, engineering of een contactpersoon voor het CSP-programma

5. Selecteer het tabblad Abonnementen en prijzen voor meer informatie over de beschikbare abonnementen, SKU's of prijzen **van een** aanbieding. Op dit tabblad ziet u het volgende:

    - De markten waar deze aanbieding voor u beschikbaar is

    - Een lijst met SKU's of abonnementen die beschikbaar zijn voor de aanbieding

    - Prijzen voor elke beschikbare SKU of abonnement

* * *

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Marketplace-aanbiedingen weergeven via Partner Center API's

CSP-programmapartners kunnen ook API's gebruiken om een lijst met in aanmerking komende aanbiedingen te retourneren. In aanmerking komende aanbiedingen zijn alleen die SaaS ISV-aanbiedingen die de partner kan verkopen via Partner Center marketplace. Voor partners die API's gebruiken om aanbiedingen in de catalogus te identificeren, raadpleegt u de richtlijnen voor het verkrijgen van een lijst [met aanbiedingen voor een markt.](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Bekijk de meest recente prijzen voor Marketplace-Partner Center

Volg deze stappen voor de meest recente prijsinformatie die is gekoppeld aan een aanbieding:

> [!NOTE]
> Zie Getting around Partner Center voor meer informatie over [de werkruimte-interface.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Werkruimteweergave](#tab/workspaces-view)

1. Meld u aan Partner Center [dashboard en](https://partner.microsoft.com/dashboard) selecteer de **tegel** Prijzen.

2. Selecteer **Marketplace.** Standaard ziet u producten van alle typen en categorieën.

3. Schuif omlaag naar de **sectie Marketplace,** selecteer een locatie en download **Marketplace-prijzen.** Hiermee wordt een spreadsheet gegenereerd met de meest recente prijsgegevens voor SaaS, aanbiedingen op basis van licenties en aanbiedingen naar gebruik die beschikbaar zijn voor ISV-uitgevers. Sommige prijzen voor Azure-toepassingen kunnen hier ook worden weergegeven. Deze informatie wordt dagelijks bijgewerkt, zodat u deze zo vaak als u kiest kunt controleren op de huidige prijzen.

4. Als een ISV-product een gratis proefperiode bevat, worden in het werkblad twee rijen voor dat product weergegeven:

    - Eén rij toont de prijs van de gratis proefversie van nul. Dit betekent dat er een gratis proefperiode beschikbaar is.

    - In de andere rij ziet u de prijs en voorwaarden die van toepassing zijn nadat de gratis proefperiode is afgelopen.

Als CSP-programmapartner komt u mogelijk in aanmerking voor andere incentives die zijn gekoppeld aan bepaalde aanbiedingen op de commerciële marketplace. Zie de [CSP Incentive Guide (CSP-aanmeldgegevens](https://aka.ms/partnerincentives) vereist) voor meer informatie over andere incentives.

#### <a name="current-view"></a>[Huidige weergave](#tab/current-view)

1. Meld u Partner Center [dashboard aan](https://partner.microsoft.com/dashboard)en selecteer **CSP** in het navigatiemenu aan de linkerkant.

2. Selecteer **Verkopen,** gevolgd door **Prijzen en aanbiedingen.**

3. Schuif omlaag naar de **sectie Marketplace,** selecteer een locatie en download **Marketplace-prijzen.** Hiermee wordt een spreadsheet gegenereerd met de meest recente prijsgegevens voor SaaS, aanbiedingen op basis van licenties en aanbiedingen naar gebruik die beschikbaar zijn voor ISV-uitgevers. Sommige prijzen voor Azure-toepassingen kunnen hier ook worden weergegeven. Deze informatie wordt dagelijks bijgewerkt, zodat u deze zo vaak als u kiest kunt controleren op de huidige prijzen.

4. Als een ISV-product een gratis proefperiode bevat, worden in het werkblad twee rijen voor dat product weergegeven:

    - Eén rij toont de prijs van de gratis proefversie van nul. Dit betekent dat er een gratis proefperiode beschikbaar is.

    - In de andere rij ziet u de prijs en voorwaarden die van toepassing zijn nadat de gratis proefperiode is afgelopen.

Als CSP-programmapartner komt u mogelijk in aanmerking voor andere incentives die zijn gekoppeld aan bepaalde aanbiedingen op de commerciële marketplace. Zie de [CSP Incentive Guide (CSP-aanmeldgegevens](https://aka.ms/partnerincentives) vereist) voor meer informatie over andere incentives.

* * *

## <a name="learn-about-marketplace-exclusive-offers"></a>Meer informatie over exclusieve Marketplace-aanbiedingen

ISV's hebben de mogelijkheid om hun aanbiedingen alleen beschikbaar te maken voor specifieke partners in het CSP-programma. Dit staat bekend als een exclusieve aanbieding. Alle partners in het CSP-programma kunnen nog steeds alle ISV-aanbiedingen weergeven in Partner Center commerciële marketplace, met inbegrip van de aanbiedingen die zijn gemarkeerd als Exclusief.

Als een aanbieding **niet** is gemarkeerd als Exclusief, kunnen alle partners die aanbieding kopen (ervan uitgaande dat het factureringsland van de geselecteerde klant overeenkomt met de landbeschikbaarheid van de ISV-aanbieding).

Voor elke aanbieding die als Exclusief is gemarkeerd, kunnen echter alleen de partners die door de ISV zijn geselecteerd, die aanbieding kopen.

> [!NOTE]
> Als u een aanbieding ziet met de naam Exclusief die u aan uw klanten wilt verkopen, neemt u rechtstreeks contact op met de ISV en vraagt u toestemming om de exclusieve aanbieding te verkopen. Wanneer u de details van een exclusieve aanbieding bekijkt, ziet u mogelijk een koppeling Contact opnemen met **ISV** die u kunt selecteren.

Lees Cloud Solution Providers voor meer informatie over de ISV-ervaring in de commerciële [marketplace.](/azure/marketplace/cloud-solution-providers)

Lees Overzicht van commerciële marketplace voor meer informatie over de CSP-ervaring in [de marketplace.](csp-commercial-marketplace-overview.md)

## <a name="next-steps"></a>Volgende stappen

- [Aanbiedingen voor de commerciële marketplace kopen](csp-commercial-marketplace-purchase.md)
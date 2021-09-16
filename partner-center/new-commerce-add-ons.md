---
title: Nieuwe commerce-invoegtoepassingen
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over nieuwe commerce-ervaringen voor het kopen van invoegtoepassingen.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 01644e5d2dd2fe2057d223b62f1f4e9d6f9cd101
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/16/2021
ms.locfileid: "127894044"
---
# <a name="introduction-new-commerce-add-ons"></a>Inleiding: Nieuwe commerce-invoegtoepassingen

**Juiste rollen**

- Beheeragent
- Verkoopagent
- Globale beheerder

> [!Note] 
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technische preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Partners kunnen invoegtoepassingen aanschaffen in nieuwe commerce om andere services in te stellen die een aanvulling zijn op een eerder gekocht product. Enkele voorbeelden hiervan zijn aanroepplannen, meer schijfruimte of andere functies die kunnen worden toegevoegd als de klant de basisservices heeft.



## <a name="add-ons-in-new-commerce"></a>Invoegtoepassingen in nieuwe handel ## 

Nieuwe commerce-invoegtoepassingen bevatten vergelijkbare concepten als traditionele invoegtoepassingen op basis van licenties. Nieuwe commerce-invoegtoepassingen, zoals traditionele licenties, bevatten het concept van vereisten. Dit zijn product-SKU's die de klant moet hebben om de invoegfunctie correct te laten functioneren. De vereisten voor een invoeggebruiker vindt u in de catalogus-API's voor een bepaalde SKU en in Partner Center catalogusgebruikerservaring. Voor het kopen van invoegtoepassingen moeten een of meer van de vereisten bestaan in de tenant van de klant.
 
Het belangrijkste verschil in de aankoop van invoegtoepassingen tussen traditionele licenties en nieuwe handel zit *hem* in de manier waarop ze worden gekocht. In een traditionele licentie past de partner de invoeg-on toe op een bestaand abonnement op de basisaanbieding. In nieuwe commerce kopen partners de invoegtoepassingen uit de catalogus zelf, zonder dat ze een gefabriceerde aankoopervaring meer hebben voor basisaanbiedingen en invoegtoepassingen, alles staat in de catalogus in nieuwe handel.

Veel van de concepten over de manier waarop invoegtoepassingen werken, blijven waar voor traditionele en nieuwe handel. De invoegservice registreren en inrichten. Er is niets anders over de manier waarop het inrichten gebeurt. Bovendien kunnen de services van één invoegservice een aanvulling zijn op meer dan één basisproduct-SKU waar de invoegservice mee kan werken.

## <a name="identifying-add-ons"></a>Invoegtoepassingen identificeren ##

Partners kunnen invoegtoepassingen identificeren en lijsten met vereisten verkrijgen door de SKU-details te controleren bij het verkrijgen van SKU's via de API. Invoegtoepassingen worden ook geïdentificeerd in de nieuwe prijslijst op basis van commercelicenties in de kolom Tags. De aanbiedingsmatrix bevat de lijst met vereisten voor elke product-SKU voor een invoegsel.

## <a name="purchasing-add-ons"></a>Invoegtoepassingen kopen ##

Er bestaan invoegtoepassingen voor zowel traditionele als nieuwe commerce-ervaringen op basis van licenties. Het belangrijkste verschil is dat nieuwe handel detecteerbaarheid en aankoop mogelijk maakt vanuit de catalogus, op dezelfde plaats als de basisaanbiedingen of vereisten. Traditionele invoegtoepassingen op basis van licenties kunnen alleen worden ontdekt en aangeschaft door naar de pagina met abonnementsgegevens van de basisaanbieding te gaan. Nadat daar een invoeg-on wordt vermeld, past de partner de gewenste invoeg-on toe.


Invoegtoepassingen voor de nieuwe commerce-ervaring worden ontdekt en aangeschaft in de catalogus zelf. Partners kunnen filteren op nieuwe commerce-invoegtoepassingen door de vervolgkeuzepagina producttype te selecteren. Invoegproducten zijn ook gemakkelijk te zien omdat er een informatiepictogram naast staat. Hier wordt de status en betekenis van de invoeg-app uitgelegd.


Partners kunnen meer informatie krijgen over de vereiste producten  voor een invoegabonnement door te klikken op Compatibele basisproductabonnementen weergeven om een lijst weer te geven met product-SKU's die voor de partner moeten bestaan om een bepaalde invoegcode te kunnen kopen.


## <a name="add-on-enforcement"></a>Afdwinging van invoegverzoeken ##

Partners krijgen fouten te zien bij het kopen van een nieuw commerce-invoegselproduct waarbij de klant geen van de vereisten heeft. Partners kunnen controleren of een klant voldoet aan de vereisten door de validateAddon-API aan te roepen in het partnercentrum.

## <a name="important-details-when-purchasing-add-ons"></a>Belangrijke details bij het kopen van invoegtoepassingen ##

Invoegtoepassingen worden aangeschaft als afzonderlijke product-SKU's als de klant aan de vereisten voldoet. Invoegabonnementen hebben hun eigen uitlijning van afzonderlijke termijnen. Partners die invoegtoepassingen aanschaffen, merken dat de termijn en de bijbehorende einddatum mogelijk niet hetzelfde zijn als de vereiste. Zolang beide abonnementen automatisch worden verlengd naar nieuwe voorwaarden, werken de vereiste en invoegtoepassingen prima. Als de partner besluit de termijn van de vereiste te beëindigen door niet automatisch te verlengen, moet de invoegsel ook worden bijgewerkt om aan het einde van de invoegtermijn niet automatisch te vernieuwen als de partner besluit dat deze niet meer nodig is.  Partners converteren een product-SKU naar een hogere SKU die al de invoegservice heeft, kunnen een serviceaanvraag indienen met ondersteuning om een invoeg-invoeging uit te schakelen.

Van partners wordt verwacht dat ze de einddatums van de termijn beheren voor invoegtoepassingen die ze verkrijgen, om ervoor te zorgen dat er naar behoefte is afgestemd op de basisaanbiedingen.


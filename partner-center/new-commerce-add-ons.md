---
title: Nieuwe commerce-invoegtoepassingen
ms.topic: article
ms.date: 08/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over nieuwe commerce-ervaringen voor het kopen van invoegtoepassingen.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 539aa939d980f7b40abc44789a08d153a8abdfaa
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957758"
---
# <a name="introduction-new-commerce-add-ons"></a>Inleiding: Nieuwe commerce-invoegtoepassingen

**Juiste rollen**

- Beheeragent
- Verkoopagent
- Globale beheerder

> [!Note] 
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van Microsoft 365/Dynamics 365 New Commerce Experience Technical Preview.

Partners kunnen invoegtoepassingen aanschaffen in nieuwe commerce om andere services mogelijk te maken die een aanvulling zijn op een eerder gekocht product. Enkele voorbeelden hiervan zijn het aanroepen van plannen, meer schijfruimte of andere functies die kunnen worden toegevoegd als de klant de basisservices heeft.



## <a name="add-ons-in-new-commerce"></a>Invoegtoepassingen in nieuwe commerce ## 

Nieuwe commerce-invoegtoepassingen bevatten vergelijkbare concepten als traditionele invoegtoepassingen op basis van licenties. Nieuwe commerce-invoegtoepassingen, zoals traditionele licenties, bevatten het concept van vereisten. Dit zijn product-SKU's die de klant moet hebben om de invoegfunctie correct te laten functioneren. De vereisten voor een invoeggebruiker vindt u in de catalogus-API's voor een bepaalde SKU en in Partner Center catalogusgebruikerservaring. Voor het kopen van invoegtoepassingen moeten een of meer van de vereisten aanwezig zijn in de tenant van de klant.
 
Het belangrijkste verschil in de aankoop van invoegtoepassingen tussen traditionele licenties en nieuwe handel zit *hem* in de manier waarop ze worden gekocht. In een traditionele licentie past de partner de invoeg-on toe op een bestaand abonnement op de basisaanbieding. In nieuwe commerce kopen partners de invoegtoepassingen van de catalogus zelf, en hebben ze niet langer een gefabriceerde aankoopervaring voor basisaanbiedingen en invoegtoepassingen, alles staat in de catalogus in nieuwe commerce.

Veel van de concepten over de manier waarop invoegtoepassingen werken, blijven waar in traditionele en nieuwe handel. De invoegservice registreren en inrichten, er is niets anders over de manier waarop de inrichting wordt gedaan. Bovendien kunnen de services van één invoeg-on een aanvulling zijn op meer dan één basisproduct-SKU waar de invoeg-invoegservice mee kan werken.

## <a name="identifying-add-ons"></a>Invoegtoepassingen identificeren ##

Partners kunnen invoegtoepassingen identificeren en lijsten met vereisten verkrijgen door de SKU-details te bekijken bij het verkrijgen van SKU's via de API. Invoegtoepassingen worden ook vermeld in de nieuwe prijslijst op basis van commercelicenties in de kolom Tags. De aanbiedingsmatrix bevat de lijst met vereisten voor elke product-SKU voor invoegabonnementen.

## <a name="purchasing-add-ons"></a>Invoegtoepassingen kopen ##

Invoegtoepassingen bestaan voor zowel traditionele op licenties gebaseerde als nieuwe commerce-ervaringen. Het belangrijkste verschil is dat nieuwe handel detecteerbaarheid en aankopen mogelijk maakt vanuit de catalogus, op dezelfde plaats als de basisaanbiedingen of vereisten. Traditionele invoegtoepassingen op basis van licenties kunnen alleen worden ontdekt en aangeschaft door naar de pagina met abonnementsgegevens van de basisaanbieding te gaan. Nadat daar een invoeg-on wordt vermeld, past de partner de gewenste invoeg-on toe.


Nieuwe commerce-invoegtoepassingen worden ontdekt en aangeschaft in de catalogus zelf. Partners kunnen filteren op nieuwe commerce-invoegtoepassingen door de vervolgkeuzepagina producttype te selecteren. Invoegproducten zijn ook gemakkelijk te zien omdat er een informatiepictogram naast staat. Hier wordt de status en betekenis van de invoeg-app uitgelegd.


Partners kunnen meer informatie krijgen over de vereiste producten  voor een invoegabonnement door te klikken op Compatibele basisproductabonnementen weergeven om een lijst weer te geven met product-SKU's die voor de partner moeten bestaan om een bepaalde invoegcode te kunnen kopen.


## <a name="add-on-enforcement"></a>Afdwinging van invoeginstanties ##

Partners krijgen fouten te zien bij een poging om een nieuw commerce-invoegselproduct te kopen waarbij de klant geen van de vereisten heeft. Partners kunnen controleren of een klant voldoet aan de vereisten door de validateAddon-API aan te roepen in het partnercentrum.

## <a name="important-details-when-purchasing-add-ons"></a>Belangrijke details bij het kopen van invoegtoepassingen ##

Invoegtoepassingen worden aangeschaft als afzonderlijke product-SKU's als de klant aan de vereisten voldoet. Invoegabonnementen hebben hun eigen uitlijning van verschillende termijnen. Partners die invoegtoepassingen aanschaffen, merken dat de termijn en de bijbehorende einddatum mogelijk niet dezelfde zijn als de vereiste. Zolang beide abonnementen automatisch worden verlengd naar nieuwe voorwaarden, werken de vereisten en invoegtoepassingen prima. Als de partner besluit de termijn van de vereiste te beëindigen door niet automatisch te verlengen, moet de invoeg-invoegsel ook worden bijgewerkt om aan het einde van de invoegtermijn niet automatisch te vernieuwen als de partner besluit dat deze niet meer nodig is.  Partners converteren een product-SKU naar een hogere SKU die al de invoegservices heeft, kunnen een serviceaanvraag indienen met ondersteuning voor het uitschakelen van een invoegservice.

Van partners wordt verwacht dat ze de einddatums van de termijn beheren voor invoegtoepassingen die ze verkrijgen om ervoor te zorgen dat er naar behoefte is afgestemd op de basisaanbiedingen.


---
title: Nieuwe commerce-invoegtoepassingen
ms.topic: article
ms.date: 09/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over nieuwe commerce-ervaringen voor het kopen van invoegtoepassingen.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 355c7ae3d4832764f6201613c040eebca998c3b6
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/29/2021
ms.locfileid: "129249329"
---
# <a name="introduction-new-commerce-add-ons"></a>Inleiding: Nieuwe commerce-invoegtoepassingen

**Juiste rollen:** beheeragent | Verkoopagent | Globale beheerder

> [!NOTE]
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van Microsoft 365/Dynamics 365 New Commerce Experience Technical Preview.

Partners kunnen invoegtoepassingen aanschaffen in nieuwe commerce om andere services mogelijk te maken die een aanvulling zijn op een eerder gekocht product. Enkele voorbeelden van invoegtoepassingen zijn het aanroepen van plannen, meer schijfruimte of andere functies die kunnen worden toegevoegd als de klant de basisservices heeft.

## <a name="add-ons-in-new-commerce"></a>Invoegtoepassingen in nieuwe commerce

Nieuwe commerce-invoegtoepassingen bevatten vergelijkbare concepten als traditionele invoegtoepassingen op basis van licenties. Nieuwe commerce-invoegtoepassingen, zoals traditionele licenties, bevatten het concept van vereisten. De vereisten zijn product-SKU's die de klant nodig heeft om de invoeg-service correct te laten functioneren. De vereisten voor een invoeggebruiker vindt u in de catalogus-API's voor een bepaalde SKU en in Partner Center catalogusgebruikerservaring. Voor het kopen van invoegtoepassingen moeten een of meer van de vereisten aanwezig zijn in de tenant van de klant.

Het belangrijkste verschil tussen traditionele en nieuwe commerce-invoegtoepassingen zit **hem** in de manier waarop ze worden gekocht. Partners passen de invoeg-on toe op het basisaanbiedingsabonnement in traditionele scenario's op basis van licenties. Partner purchase new commerce add-ons from the catalog itself. Met deze aankoopervaring wordt de invoegtoepassingen afgestemd op de basisaanbieding, zodat u de invoegtoepassingen gemakkelijker kunt vinden en kopen.

Veel van de concepten over de manier waarop invoegtoepassingen werken, blijven waar voor traditionele en nieuwe handel. Zowel traditionele als nieuwe handelstransacties registreren en inrichten van de invoegservice. In beide gevallen gebeurt het inrichten op dezelfde manier. Bovendien kunnen de services van één invoeg-on een aanvulling zijn op meer dan één basisproduct-SKU waar de invoeg-on mee kan werken.

## <a name="identifying-add-ons"></a>Invoegtoepassingen identificeren

Partners kunnen invoegtoepassingen identificeren en lijsten met vereisten verkrijgen door de SKU-details te bekijken bij het verkrijgen van SKU's via de API. Invoegtoepassingen worden ook vermeld in de nieuwe prijslijst op basis van commercelicenties in de kolom Tags. De aanbiedingsmatrix bevat de lijst met vereisten voor elke invoeg-product-SKU.

## <a name="purchasing-add-ons"></a>Invoegtoepassingen kopen

Invoegtoepassingen bestaan voor zowel traditionele op licenties gebaseerde als nieuwe commerce-ervaringen. Het belangrijkste verschil is hoe de invoegtoepassingen worden ontdekt. Nieuwe commerce-invoegtoepassingen worden ontdekt en kopen in de catalogus, op dezelfde plaats als de basisaanbiedingen of vereisten. Traditionele invoegtoepassingen op basis van licenties kunnen alleen worden ontdekt en toegevoegd door naar de pagina met abonnementsgegevens van de basisaanbieding te gaan. 

Nieuwe commerce-invoegtoepassingen worden ontdekt en aangeschaft in de catalogus zelf. Partners kunnen filteren op nieuwe commerce-invoegtoepassingen door de vervolgkeuzepagina producttype te selecteren. Invoegproducten worden aangeduid met het informatiepictogram naast de product-SKU. Partners kunnen op dit pictogram klikken voor meer informatie over de vereisten voor de invoeg-app.

Partners kunnen meer informatie krijgen over de vereiste producten  voor een invoegabonnement door te klikken op Compatibele basisproductabonnementen weergeven om een lijst weer te geven met product-SKU's die voor de partner moeten bestaan om een bepaalde invoegcode te kunnen kopen.

## <a name="add-on-enforcement"></a>Afdwinging van invoeginstanties

Partners zien nuttige informatie over invoegtoepassingen wanneer ze een nieuw commerce-invoegtoepassingenproduct willen kopen wanneer de klant niet aan de vereisten heeft. Partners kunnen valideren of er vereisten voor een invoeg-on aanwezig zijn in de Partner Center catalogus en de pagina-ervaringen controleren. Als de invoeggebruiker niet aan de ondersteuningsvoorwaarden heeft, wordt in de gebruikersinterface het bericht 'De invoeggebruiker kan niet worden opgevraagd zonder een compatibel basisproduct' weergegeven. Partners die de CreateCart-API gebruiken, krijgen een foutmelding te zien op het regelitem van de winkelwagen als de invoeg-app niet de vereiste product-SKU's heeft. De foutcode wordt 400041 met de beschrijving 'De invoegvoegcode kan niet worden opschatbaar zonder een compatibel basisproduct'.

## <a name="important-details-when-purchasing-add-ons"></a>Belangrijke details bij het kopen van invoegtoepassingen

Invoegtoepassingen worden aangeschaft als afzonderlijke product-SKU's als de klant aan de vereisten voldoet. Invoegabonnementen hebben hun eigen uitlijning van de verschillende termijnen. Partners die invoegtoepassingen aanschaffen, merken dat de termijn en de bijbehorende einddatum mogelijk niet dezelfde zijn als de vereiste. Zolang beide abonnementen automatisch worden verlengd naar nieuwe voorwaarden, blijven de vereisten en invoegtoepassingen correct werken. Als de partner besluit de termijn van de vereiste te beëindigen door niet automatisch te verlengen, moet de invoeg-invoegsel ook worden bijgewerkt om aan het einde van de invoegtermijn niet automatisch te vernieuwen als de partner besluit dat deze niet meer nodig is.  Partners converteren een product-SKU naar een hogere SKU die al de invoegservices heeft, kunnen een serviceaanvraag indienen met ondersteuning voor het uitschakelen van een invoegservice.

Van partners wordt verwacht dat ze de einddatums van de termijn beheren voor invoegtoepassingen die ze verkrijgen om ervoor te zorgen dat er naar behoefte is afgestemd op de basisaanbiedingen.

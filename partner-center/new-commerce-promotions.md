---
title: Nieuwe commerciële promoties
ms.topic: article
ms.date: 08/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over nieuwe commerce-ervaringen voor het detecteren en kopen van promoties.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: abb1bc79bc3a67ccb9f3d067f6eeb8cb22a6b3f5
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/03/2021
ms.locfileid: "123458285"
---
# <a name="introduction-new-commerce-promotions"></a>Inleiding: Nieuwe commerciële promoties

**Juiste rollen**

- Beheeragent
- Verkoopagent
- Globale beheerder

> [!Note] 
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van Microsoft 365/Dynamics 365 New Commerce Experience Technical Preview.

Microsoft biedt ondersteuning voor promoties in nieuwe handel. Deze promoties hebben verschillende kortingsbedragen en duur. 

## <a name="discovering-promotions"></a>Promoties detecteren ##

Partners kunnen promoties ontdekken door de achterstand voor promoties te bezoeken of door de GETPromotions-API aan te roepen. De achterstand bij promoties is een Microsoft-lijst met beschikbare promoties die partners moeten kennen. De lijst wordt maandelijks opeengepdatet en bijgewerkt. 


## <a name="operationalize-promotions"></a>Promoties operationeel maken ##

Partners kunnen de promoties operationeel maken door de getPromotions-API te implementeren. Deze API retourneert alle promoties die bestaan voor een bepaalde markt (het land van de klant) en het segment. De API retourneert de lijst met promoties en belangrijke informatie om de partner te helpen begrijpen welke promoties beschikbaar zijn voor klanten in verschillende landen. 


De getPromotions-API bevat de volgende gegevens voor een bepaalde promotie:

- Duur van de promotie
- Het kortingspercentage voor de promotie
- De producten en SKU's voor welke promotie beschikbaar is

Promoties worden toegepast door het partnercentrum wanneer de partner de product-SKU koopt waarop de promotie beschikbaar is. Partnerpromoties zijn beschikbaar in de gebruikersinterface van de partnercentrumcatalogus in de product-SKU-details. Ze kunnen klikken op De promotiegegevens weergeven voor meer informatie over de promotie. De mogelijkheid om de promotiedetails weer te geven, is toegankelijk via de SKU-details van de cataloguspaginaweergave, de beoordelingspagina vóór het indienen van de aankoop, de bevestiging nadat de order is verzonden en de pagina ordergeschiedenis. 


## <a name="verify-eligibility"></a>Geschiktheid controleren ##

Partners kunnen bekijken of een klantaankoop in aanmerking komt voor een promotie door de informatie op de beoordelingspagina in het partnercentrum te bekijken voordat het product wordt gekocht. Partners kunnen ook de verifyPromotionEligibility-API aanroepen, door de tenant-id van de klant en de promotie-id door te geven. De aanroep retourneert true als de klant in aanmerking komt. Als de klant niet in aanmerking komt, retourneert de API de voorwaarden die niet van toepassing zijn op de promotie. 



## <a name="promotions-and-renewals"></a>Promoties en verlengingen ##

Aanbiedingskortingen wanneer deze worden toegepast, gelden voor de duur van de aankoop. Abonnementen met toegepaste promoties behouden de actieprijs als de verlengingsdatum binnen het datumbereik van de promotieduur valt. Verlengingen buiten het datumbereik van de promotieduur worden verlengd tot de prijs die niet aan promotie is toegevoegd (in de prijslijst). Partners kunnen de verlengingsstatus volgen voor de prijspunten op de pagina met abonnementsgegevens en op de instructies voor het verlengen van de getSubscription-gegevens.


## <a name="promotions-and-upgrades"></a>Promoties en upgrades ##
Partners die upgraden van een abonnement naar een andere SKU laten de promotieprijs achter. Deze actie treedt op omdat de promotie is geconfigureerd voor de SKU die ze verlaten wanneer ze upgraden naar een andere SKU. Partners die upgraden naar een SKU die mogelijk een promotie heeft, krijgen niet automatisch de promotieprijs. Als ze de promotieprijs nodig hebben of willen hebben voor de SKU waar ze naar willen gaan, moeten ze de nieuwe SKU handmatig aanschaffen als een nieuw abonnement. Momenteel worden promoties alleen toegepast op nieuwe abonnementen en verlengingen.




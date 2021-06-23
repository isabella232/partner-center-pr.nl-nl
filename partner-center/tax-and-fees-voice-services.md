---
title: Regionale PSTN-servicebelastingen en -kosten
description: Als Office 365-partner die Microsoft 365 Voice-producten aftransactiet, bent u mogelijk onderworpen aan regionale belastingen, kosten of wettelijke vereisten voor PSTN-services.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 85eefb49cf62c4bcfa5533683abd8ddb0e854463
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/23/2021
ms.locfileid: "112490067"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionale belastingen, voorschriften voor PTSN-services (Public Switched Telephone Network)

**Juiste rollen:** Globale | Gebruikersbeheerders | Beheeragent

PSTN-services (Public Switched Telephone Network) in sommige jurisdicties zijn mogelijk onderworpen aan speciale belasting- en regelgevingsvereisten die van invloed kunnen zijn op de volgorde en facturering van partners. In de Verenigde Staten, met inbegrip van Communication Communication, zijn PSTN-services, waaronder audiovergaderingen, aanroepplannen en communicatietegoeden, onderworpen aan speciale belasting- en regelgevingsvereisten. In de Verenigde Staten enOrteEneEner prijst Microsoft PSTN-services als tax-inclusive.  Unieke PSTN-belastingen en -regelgeving zijn van invloed op Office 365-partners die Microsoft 365 Voice-producten.  Als een partner de prijs van een Microsoft PSTN-service markeert, kan deze verantwoordelijk zijn voor het berekenen en ruiten van PSTN-belastingen en -kosten.

## <a name="partner-recommendations"></a>Aanbevelingen van partners

Neem contact op met uw belasting- en juridische adviseur om inzicht te krijgen in de verantwoordelijkheid van uw organisatie met betrekking tot de regelgeving, belastingen en kosten van PSTN-services en andere potentiële gevolgen.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Factuurpresentatie en partnerafstemmingsbestand

Cloud Solution Provider-facturen (CSP) en CSP-afstemmingsbestanden in de Verenigde Staten, Skype Voor Bedrijven PSTN en Microsoft 365 Voice-services, bieden afzonderlijke regelitems voor de PSTN- en niet-PSTN-onderdelen.

Daarnaast worden op CSP-facturen de volgende voetnoot weergegeven:

* De weergegeven prijs is een bedrag voor audiovergaderingen en het aanroepen van planservices.  Alle toepasselijke transactionele belastingen worden exclusief in rekening gebracht van het weergegeven bedrag, met uitzondering van de verkopen in de Verenigde Staten.  In de Verenigde Staten is de weergegeven prijs inclusief btw, omdat deze kosten bevat voor de oproepende plan- en audiovergaderingservices en kosten voor de belastingen en kosten die we in rekening moeten brengen.  Services voor audiovergaderingen en oproepen van planservices worden verwerkt door de Microsoft-partner die gemachtigd is om deze te leveren.  Zie [Microsoft Volume Licensing](https://go.microsoft.com/fwlink/?LinkId=690247) voor meer informatie.

## <a name="reconciliation-file-example"></a>Voorbeeld van afstemmingsbestand

Office 365 Enterprise E5 wordt in het afstemmingsbestand als twee regelitems met identieke namen en identieke ID's gebruikt, maar elk regelitem heeft een unieke eenheidsprijs (bijvoorbeeld: $ 28,40 en $ 2,00). Hiermee wordt het Skype voor Bedrijven PSTN-conferencing-onderdeel van de Office 365-aanbieding gescheiden, zodat u op de juiste wijze belastingen kunt toepassen.

**Voorbeeld van partnerafstemming #1 (kolommen selecteren):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Cycluskosten   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Cycluskosten   |2,00   |

**Voorbeeld van partnerafstemming #2**

Microsoft 365 Business Voice die beschikbaar is in Canada, bevat aanvullende, met PSTN belaste onderdelen die worden geconsolideerd op CSP-factuur (vergelijkbaar met Office 365 E5, er worden twee regelitems weergegeven, één voor PSTN-onderdelen en de andere voor niet-PSTN-onderdelen).  In het CSP-afstemmingsbestand voor Microsoft 365 Business Voice worden alle belaste PSTN-onderdelen afzonderlijk weergegeven (afzonderlijke PSTN-onderdelen worden niet geconsolideerd in .CSV of API-hulpprogramma).  De som van ordergegevens en gefactureerde bedragen voor klanten die in het afstemmingsbestand zijn gevonden, komt overeen met de CSP-factuur.

## <a name="additional-resources"></a>Aanvullende resources
Ga naar de site Microsoft 365 [voor partners voor meer](https://www.microsoft.com/microsoft-365/partners/) informatie.


---
title: Regionale PSTN-servicebelastingen en -kosten
description: Als Office 365-partner die Microsoft 365 Voice-producten aftakt, bent u mogelijk onderworpen aan regionale belastingen, kosten of wettelijke vereisten voor PSTN-services.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 80cb5503323f483c13c983375559baf70f9d0b6f
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854720"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionale belastingen, voorschriften voor PTSN-services (Public Switched Telephone Network)

**Juiste rollen:** globale | Gebruikersbeheerders | Beheeragent

PsTN-services (Public Switched Telephone Network) in sommige jurisdicties zijn mogelijk onderworpen aan speciale belasting- en regelgevingsvereisten die van invloed kunnen zijn op de volgorde en facturering van partners. In de Verenigde Staten, met inbegrip van Communication Communication, zijn PSTN-services, waaronder audiovergaderingen, oproepplannen en communicatietegoeden, onderworpen aan speciale belasting- en regelgevingsvereisten. In de Verenigde Staten en Verenigde Staten worden PSTN-services door Microsoft als inclusief belasting betaald.  Unieke PSTN-belastingen en -regelgeving zijn van invloed op Office 365-partners die Microsoft 365 Voice-producten.  Als een partner de prijs van een Microsoft PSTN-service markeert, is deze mogelijk verantwoordelijk voor het berekenen en afrekenen van PSTN-belastingen en -kosten.

## <a name="partner-recommendations"></a>Aanbevelingen van partners

Neem contact op met uw belasting- en juridisch adviseur om inzicht te krijgen in de verantwoordelijkheid van uw organisatie met betrekking tot de regelgeving, belastingen en kosten van PSTN-services en andere potentiële verplichtingen.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Factuurpresentatie en partnerafstemmingsbestand

CSP-facturen en CSP-afstemmingsbestanden in de Verenigde Staten, Skype Voor Bedrijven PSTN en Microsoft 365 Voice-services bevatten afzonderlijke regelitems voor de PSTN- en niet-PSTN-onderdelen.

Daarnaast wordt op CSP-facturen de volgende voetnoot weergegeven:

* De weergegeven prijs is een kosten voor audiovergaderingen en het aanroepen van planservices.  Alle toepasselijke transactionele belastingen worden exclusief in rekening gebracht op het weergegeven bedrag, met uitzondering van de verkopen in de Verenigde Staten.  In de Verenigde Staten is de weergegeven prijs inclusief btw, omdat deze kosten bevat voor de oproepende plan- en audiovergaderingservices en kosten voor de belastingen en kosten die we in rekening moeten brengen.  Services voor audiovergaderingen en oproepplannen worden verwerkt door de Microsoft-partner die gemachtigd is om deze te leveren.  Zie [Microsoft Volume Licensing](https://go.microsoft.com/fwlink/?LinkId=690247) voor meer informatie.

## <a name="reconciliation-file-example"></a>Voorbeeld van afstemmingsbestand

Office 365 Enterprise E5 wordt in het afstemmingsbestand als twee regelitems met identieke namen en identieke ID's gebruikt, maar elk regelitem heeft een unieke eenheidsprijs (bijvoorbeeld: $ 28,40 en $ 2,00). Hiermee wordt het Skype voor Bedrijven PSTN-conferencing-onderdeel van de Office 365-aanbieding gescheiden, zodat u op de juiste wijze belastingen kunt toepassen.

**Voorbeeld van partnerafstemming #1 (kolommen selecteren):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Cycluskosten   |28.40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Cycluskosten   |2,00   |

**Voorbeeld van partnerafstemming #2**

Microsoft 365 Business Voice die beschikbaar is in Canada, heeft extra belastbare PSTN-onderdelen die zijn geconsolideerd op CSP-factuur (vergelijkbaar met Office 365 E5, worden twee regelitems weergegeven, één voor PSTN-onderdelen en de andere voor niet-PSTN-onderdelen).  In het CSP-afstemmingsbestand Microsoft 365 Business Voice worden alle belaste PSTN-onderdelen afzonderlijk weergegeven (afzonderlijke PSTN-onderdelen worden niet geconsolideerd in . CSV- of API-hulpprogramma).  De som van ordergegevens en gefactureerde bedragen voor klanten die in het afstemmingsbestand zijn gevonden, komt overeen met de CSP-factuur.

## <a name="additional-resources"></a>Aanvullende resources
Ga naar de site Microsoft 365 [for Partners voor meer](https://www.microsoft.com/microsoft-365/partners/) informatie.


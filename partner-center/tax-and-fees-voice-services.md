---
title: Regionale PSTN-service belastingen en-kosten
description: Als een Office 365-partner die Microsoft 365 Voice-producten transactieert, is het mogelijk dat er regionale belastingen, kosten of wettelijke vereisten gelden voor PSTN-Services.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5817e5bb010cee0ab280c83408167f28915a6237
ms.sourcegitcommit: 9b36128fdbd24e4bfe4597b1e6104bd560583c5c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/15/2020
ms.locfileid: "92528357"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Regionale belastingen, voor schriften voor openbaar geswitcheerde telefoonnet werk (PTSN)

**Van toepassing op**

- Partnercentrum
- Office 365-partners die Microsoft 365 Voice-producten handelen

**Juiste rollen**
-    Globale beheerder
-    Gebruikersbeheerder
-    Beheer agent

Open bare telefoonnet werk Services (PSTN) in sommige jurisdicties zijn mogelijk onderworpen aan speciale belasting-en regelgeving die van invloed kunnen zijn op de partner volgorde en facturering. In de Verenigde Staten, waaronder Puerto Rico, worden PSTN-Services, die audio vergaderingen, oproep plannen en communicatie tegoeden omvatten, onderworpen aan speciale belasting-en regelgeving. In de Verenigde Staten en Puerto Rico, micro soft prijzen PSTN-Services als exclusief BTW.  Unieke PSTN-belastingen en-voor schriften zijn van invloed op de Office 365-partners die worden Microsoft 365 Voice-producten.  Als een partner de prijs van een micro soft PSTN-service markeert, kan hij verantwoordelijk zijn voor het berekenen en remitteren van de PSTN-belastingen en-kosten.

## <a name="partner-recommendations"></a>Partner aanbevelingen

Stel uw belasting en juridisch adviseur in om inzicht te krijgen in de verantwoordelijkheid van uw organisatie met betrekking tot de regelgeving, belastingen en vergoedingen en andere mogelijke verplichtingen.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Factuur presentatie en partner afstemmings bestand

CSP-facturen en CSP-afstemmings bestanden in de Verenigde Staten, Puerto Rico en Canada, waaronder Skype voor bedrijven PSTN en Microsoft 365 Voice Services, bieden afzonderlijke regel items voor de PSTN-en niet-PSTN-onderdelen.

Daarnaast wordt in CSP-facturen de volgende voet noot weer gegeven:

* De weer gegeven prijs is een toeslag voor audio vergaderingen en oproep plan Services.  Eventuele van toepassing zijnde transactionele belastingen worden alleen in rekening gebracht met de hoeveelheid die wordt weer gegeven, behalve voor de verkoop in de Verenigde Staten.  In de V.S. is de prijs die wordt weer gegeven, inclusief de kosten voor het oproep plan en de services voor audio vergaderingen, en worden kosten in rekening gebracht voor de belastingen en kosten die we nodig hebben.  Audio vergaderingen en oproep plan services worden onderhouden door de micro soft-vestiging die is gemachtigd om deze te leveren.  Zie [Microsoft Volume Licensing](https://go.microsoft.com/fwlink/?LinkId=690247) voor meer informatie.

## <a name="reconciliation-file-example"></a>Voor beeld van een afstemmings bestand

Office 365 Enter prise E5 geeft een afstemmings bestand weer als twee regel items met identieke namen en identieke Id's, maar elk regel item heeft een unieke eenheids prijs (bijvoorbeeld: $28,40 en $2,00). Dit is het enige deel van het Skype voor bedrijven PSTN Conferencing-onderdeel van de Office 365-aanbieding, zodat u op de juiste wijze belastingen kunt Toep assen.

**Partner Temmings voorbeeld #1 (kolommen selecteren):**

|**Durable_offer_ID**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Cyclus kosten   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Cyclus kosten   |2,00   |

**Voor beeld van partner afstemming #2**

Microsoft 365 Business Voice beschikbaar in Canada beschikt over extra PSTN-belaste onderdelen die worden geconsolideerd op CSP-factuur (op dezelfde manier als Office 365 E5, worden er twee regel items gepresenteerd, één voor PSTN-onderdelen en de andere voor niet-PSTN-onderdelen).  In het CSP-afstemmings bestand voor Microsoft 365 Business Voice worden alle belaste onderdelen afzonderlijk weer gegeven (afzonderlijke PSTN-onderdelen worden niet geconsolideerd in. CSV-of API-hulp programma).  De som van de Order Details en gefactureerde bedragen voor klanten die zijn gevonden in het afstemmings bestand komen overeen met de CSP-factuur.

## <a name="additional-resources"></a>Aanvullende resources
Ga voor meer informatie naar de site [Microsoft 365 voor partners](https://www.microsoft.com/microsoft-365/partners/) .


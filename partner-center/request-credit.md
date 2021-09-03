---
title: Een tegoed aanvragen bij Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Meer informatie over de voordelen, beperkingen en procedures voor het aanvragen van een SLA-tegoed (Service Level Agreement) bij Microsoft als uw klanten een servicestoring ervaren.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 51c5b896564e7eb915814c43a6931e48f1777ffc
ms.sourcegitcommit: 09d2c10491244775e656b48fce35b5648262ce59
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/03/2021
ms.locfileid: "123457953"
---
# <a name="how-and-when-to-request-a-credit-from-microsoft"></a>Hoe en wanneer u een tegoed kunt aanvragen bij Microsoft

**Juiste rollen:** beheeragent | Globale beheerder

U kunt **sla-tegoeden (Service Level Agreement)** aanvragen bij Microsoft als een service die u aan uw klanten levert, een storing heeft.

## <a name="sla-credit-calculation"></a>SLA-kredietberekening

SLA-tegoeden van Microsoft worden bepaald op basis van welke service(s) zijn beïnvloed. Als uw klant bijvoorbeeld een Office 365-suite heeft maar alleen een SharePoint-storing heeft ondervonden, wordt het SLA-tegoed alleen goedgekeurd voor SharePoint en niet voor het hele plan van de klant.

*Tegoeden worden pro-rated op basis van de betrokken service en de duur van de storing.* Zie het document Online Services Consolidated SLA voor de typen scenario's die in aanmerking komen voor [SLA-tegoed.](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37) Deze informatie geldt ook voor services die via het Cloud Solution Provider (CSP)-programma worden verkocht.


## <a name="request-an-sla-credit"></a>Een SLA-tegoed aanvragen

*De CSP-partner moet de claim en alle vereiste gegevens indienen aan het einde van de kalendermaand na de maand waarin het incident zich heeft voorgedaan.* Als het incident bijvoorbeeld op 15 februari heeft plaatsgevonden, moet Microsoft de claim en alle vereiste informatie voor 31 maart ontvangen. Eindklanten en indirecte resellers kunnen geen SLA-kredietclaims indienen; De indirecte provider of directe factuurpartner moet claims namens hen indienen.

> [!NOTE]
> Adviesincidenten komen doorgaans niet in aanmerking voor SLA-tegoed. Een incident dat op het Service Health Dashboard wordt geplaatst, geeft aan dat een *tenant* mogelijk wordt beïnvloed en vertegenwoordigt de beste informatie die Microsoft op het moment van publicatie heeft. Statuspaginagegevens vertegenwoordigen de algemene beschikbaarheid van een service. De impact, beperking en oplossing van afzonderlijke service kan variëren. U kunt de laatste incidentpost en incidentbeoordeling bekijken voor meer informatie. Zie How to check Microsoft 365 service health (Service [health controleren)](/microsoft-365/enterprise/view-service-health#incidents-and-advisories) voor meer informatie.

### <a name="required-information"></a>Vereiste informatie

De naam van de klant, de tenant-id, het partnerticket# en het datum-/tijdstempel van een ticket dat is gemaakt, zijn niet voldoende om een claim te verwerken.

Voordat u [een SLA-tegoedaanvraag bij](#submit-sla-credit-request) Microsoft indient, moet u **alle** volgende informatie verzamelen om op te nemen in uw ondersteuningsticket:

- De GUID van de tenant van de klant
- De [id van het storingsincident](#outage-incident-identifier)?
- Bewijs dat de klant is beïnvloed door de storing en een SLA-tegoed heeft aangevraagd.
- Zijn de beïnvloede abonnementen aangeschaft via CSP? (*Ja* of *Nee*)

#### <a name="evidence-that-proves-customer-impact"></a>Bewijs dat de impact van de klant aantoont

- Informatie over de tijd en duur van de downtime
- Het aantal en de locatie(en) van de betrokken gebruikers (indien van toepassing)
- Beschrijvingen van uw pogingen om het incident op te lossen op het moment van de gebeurtenis
- Een e-mailbericht van de beïnvloede klant die ondersteuning en vervolgens tegoed aanvraagt
- Het ondersteuningsticketnummer en de details van de contactpersoon van de klant met betrekking tot het oplossen van service-impact


#### <a name="outage-incident-identifier"></a>Incident-id van storing

U vindt de id voor het storingsincident op **Service Health** pagina in de Microsoft 365-beheercentrum. De **incident-id** voor uitval is een getal voorafgegaan door een afkorting van twee letters die de betrokken service aangeeft (bijvoorbeeld *EX25194* voor een Exchange Online storing). In de volgende tabel worden algemene serviceafbrekingen beschreven:

| Afkorting van twee letters | Microsoft-service |
| ----------------------- | ----------------- |
| EX | Exchange Online |
| FO | Exchange Online Protection |
| SB | Skype voor Bedrijven Online (voorheen Lync Online) |
| Besturingssysteem | Office Abonnement |
| PB | Power BI voor Office 365 |
| SP | SharePoint Online |
| YA | Yammer Enterprise |
| MO | Portalfout |

### <a name="submit-sla-credit-request"></a>SLA-tegoedaanvraag indienen

Uw SLA-tegoedaanvraag indienen bij Microsoft via het Partner Center dashboard:

1. Meld u aan bij het dashboard van het Partnercentrum.
2. Kies in het menu aan de linkerkant **Serviceaanvragen** en selecteer vervolgens **Partnerondersteuningsaanvragen.**
3. Kies op **de pagina Partneraanvraag** de optie **Nieuwe aanvraag.**
4. Zoek op **de pagina De aanvraag** starten de sectie **CSP - klanten, orders en abonnementen**. Kies in deze sectie Een **probleemtype selecteren** en selecteer vervolgens **Tegoedaanvragen voor klantenservice.**
5. Kies op **de pagina** Aanbevolen oplossingen onder Hebt u meer **hulp nodig?** de optie **Ja.**
6. Vul op **de** pagina Details de sectie **Probleemdetails** in. Voer in **het** tekstvak Details de vereiste gegevens [in die](#required-information) u eerder hebt verzameld.
7. Kies **Verzenden om** uw SLA-tegoedaanvraag te verzenden.

## <a name="next-steps"></a>Volgende stappen

- [Problemen melden namens uw klant](report-problems-on-behalf-of-a-customer.md)

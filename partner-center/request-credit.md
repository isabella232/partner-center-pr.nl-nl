---
title: Een tegoed aanvragen bij Microsoft
ms.topic: article
ms.date: 03/31/2021
description: Meer informatie over de voordelen, beperkingen en procedures voor het aanvragen van een tegoed bij Microsoft.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 0521c7fde81663b9eb7cd89344ee2432e8a1ea31
ms.sourcegitcommit: eeb81ccb888239a0e8fbe4711de3ce07f3b00358
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/23/2021
ms.locfileid: "128312214"
---
# <a name="how-and-when-to-request-a-credit-from-microsoft"></a>Hoe en wanneer u een tegoed kunt aanvragen bij Microsoft

**Juiste rollen:** beheeragent | Globale beheerder

In dit artikel wordt uitgelegd Cloud Solution Provider directe en indirecte providers (CSP) tegoed kunnen aanvragen voor:

- [Onbedoelde aankopen](#accidental-purchase-credit)

- [Dubbele orders](#duplicate-orders-credit)

- [Service-uitval (problemen met service level agreement)](#service-outages-service-level-agreement-issues)

- Technische problemen

- Onjuiste informatie van Microsoft

## <a name="considerations"></a>Overwegingen

Tegoedaanvragen worden alleen geaccepteerd van directe en indirecte CSP-providers. Aanvragen worden niet geaccepteerd door indirecte resellers.

[Het maken van een serviceaanvraag voor een klant in Microsoft Azure](./report-problems-on-behalf-of-a-customer.md) is een afzonderlijk proces.

## <a name="requesting-a-credit"></a>Een tegoed aanvragen

**Een tegoed aanvragen:**

1. Download en vul de [*aanvraag voor tegoed of restitutieformulier in.*](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3eWCb) (Houd er rekening mee dat als u de voorgaande koppeling selecteert, het formulier rechtstreeks naar uw computer wordt gedownload.)

1. Meld u aan bij het dashboard van het Partnercentrum.

1. Kies help en ondersteuning in het menu **aan de linkerkant.**

1. Selecteer **Nieuwe aanvraag.**

1. Selecteer **Door onderwerpen** bladeren en selecteer **Categorie** = CSP, **Onderwerp** = Facturering en facturering en **Subonderwerp** = Tegoedaanvragen en restituties.

1. Selecteer op **de pagina** Aanbevolen oplossingen onder Hebt u meer **hulp nodig?** de **optie Ja.**

1. Vul op **de** pagina Details de sectie **Probleemdetails** in. Voer in **het** tekstvak Details [](#required-information) de vereiste informatie in die wordt beschreven in het formulier Voor tegoed of restitutie aanvragen.
1. Selecteer **Indienen**.

## <a name="types-of-credits"></a>Typen tegoeden

In deze sectie worden enkele tegoeden beschreven die u kunt aanvragen.

### <a name="accidental-purchase-credit"></a>Onopzettelijk aankooptegoed

Voor tegoedaanvragen voor verouderde aanbiedingen van Microsoft 365 of Microsoft Dynamics 365 (bijvoorbeeld wanneer het aantal licenties per ongeluk is verhoogd of het verkeerde product is gekocht):

- Annuleringen van abonnementen binnen 30 dagen na aankoop worden 100% gerestitueerd zonder dat u een serviceaanvraag hoeft te maken. Het tegoed wordt weergegeven in het factuur-/afstemmingsbestand dat is uitgegeven nadat het abonnement is opgeschort.

- Als u een abonnement in maanden 2 tot en met 12 schort, wordt u naar eigen goedheid gecrediteerd. Als u een volledige restitutie wilt ontvangen vanaf het begin van het abonnement, moet een aanvraag binnen **90** dagen na aankoop worden ingediend, met uitzondering van:

  - Microsoft Power BI Premium P1:A-aanvraag moet binnen **zeven** dagen worden ingediend voor een restitutie van 100%. Na zeven dagen worden vaste kosten in mindering gebracht op het tegoed.

  - Microsoft 365 A1: Het volledige tegoed wordt alleen verstrekt als de aanvraag binnen **30**  dagen na aankoop is ingediend en er geen gebruikers zijn toegewezen aan het abonnement. Er worden geen restituties gegeven na 30 dagen na aankoop.

### <a name="duplicate-orders-credit"></a>Tegoed dubbele orders

Voor tegoedaanvragen voor dubbele licenties (bijvoorbeeld wanneer een klant dubbele licenties heeft na de migratie naar een andere tenant of naar een andere CSP-partner):

- Tegoedaanvragen moeten binnen **120** dagen na de aankoop van het **nieuwe abonnement** worden ingediend.

- Klanten die vrijwillig overstappen tussen partners of tenants verliezen alle aanbiedingen in hun overeenkomsten.

- Eerdere promoties worden niet overgedragen als ze niet meer beschikbaar zijn.

- Nieuwe aanbiedingen worden aangeschaft tegen de huidige prijs.

### <a name="service-outages-service-level-agreement-issues"></a>Service-uitval (problemen met service level agreement)

Voor tegoedaanvragen voor service-uitval:

- SLA-tegoeden van Microsoft worden bepaald op basis van welke service(s) zijn beïnvloed. Als uw klant bijvoorbeeld een Office 365-suite heeft maar alleen een SharePoint-storing heeft ondervonden, wordt het SLA-tegoed alleen goedgekeurd voor SharePoint en niet voor het hele plan van de klant
- Tegoeden worden pro rated op basis van de betrokken service en de duur van de storing. Zie het document Online Services Consolidated SLA voor de typen scenario's die in aanmerking komen voor [SLA-tegoed.](https://www.microsoft.com/licensing/docs/view/Service-Level-Agreements-SLA-for-Online-Services) Deze informatie is ook van toepassing op services die via het Cloud Solution Provider (CSP)-programma worden verkocht.
- Tegoedaanvragen moeten worden ingediend aan het einde van de kalendermaand na de maand waarin het incident heeft plaatsgevonden. Als het incident bijvoorbeeld plaatsvond op 15 februari, moeten we de claim en alle vereiste informatie voor 31 maart ontvangen. (Zie Aanvraag voor tegoed *of restitutieformulier voor meer informatie.*

- U moet bewijzen leveren dat de klant is beïnvloed door de storing en dat de klant een SLA-tegoed heeft aangevraagd. Tenant-id en uitval-id van de klant (van Service Health Dashboard) moeten worden opgegeven. Het e-mailbericht van de klant dat als bewijs is verzonden, moet afkomstig zijn van het domein van de betrokken tenant. (E-mail vanaf een persoonlijk adres is niet toegestaan).

> [!NOTE]
> Adviesincidenten komen doorgaans niet in aanmerking voor SLA-tegoed. Een incident dat op het Service Health Dashboard wordt geplaatst, geeft aan dat een *tenant* mogelijk wordt beïnvloed en vertegenwoordigt de beste informatie die Microsoft op het moment van publicatie heeft. Statuspaginagegevens vertegenwoordigen de algemene beschikbaarheid van een service. De impact, beperking en oplossing van afzonderlijke service kan variëren. U kunt de laatste incidentpost en incidentbeoordeling bekijken voor meer informatie. Zie How to check Microsoft 365 service health (Status van de service controleren) Microsoft 365 service health (Status van [service controleren) voor meer informatie](/microsoft-365/enterprise/view-service-health)over service health.

### <a name="required-information"></a>Vereiste informatie

De naam van de klant, de tenant-id, het partnerticketnummer en het door het ticket gemaakte datum/tijd-zegel zijn niet voldoende om een claim te kunnen verwerken.

Voordat u [een SLA-tegoedaanvraag bij](https://www.microsoft.com/licensing/docs/view/Service-Level-Agreements-SLA-for-Online-Services) Microsoft indient, moet u alle volgende informatie verzamelen om op te nemen in uw ondersteuningsticket:

- De GUID van de tenant van de klant
- De [incident-id van de storing](#outage-incident-identifier)
- Bewijs dat de klant is beïnvloed door de storing en een SLA-tegoed heeft aangevraagd.
- Zijn de beïnvloede abonnementen aangeschaft via CSP? (Ja of nee)

### <a name="evidence-that-proves-customer-impact"></a>Bewijs dat de impact van de klant aantoont

- Informatie over de tijd en duur van de downtime
- Het aantal en de locatie(en) van de betrokken gebruikers (indien van toepassing)
- Beschrijvingen van uw pogingen om het incident op te lossen op het moment van de gebeurtenis
- Een e-mail van de beïnvloede klant die ondersteuning en vervolgens tegoed aanvraagt
- Het ondersteuningsticketnummer en de details van de contactpersoon van de klant met betrekking tot het oplossen van service-impact

### <a name="outage-incident-identifier"></a>Incident-id van storing

U vindt de id voor het storingsincident op Service Health pagina in de Microsoft 365-beheercentrum. De incident-id voor uitval is een getal voorafgegaan door een afkorting van twee letters die de betrokken service aangeeft (bijvoorbeeld EX25194 voor een Exchange Online storing).

In de volgende tabel worden algemene serviceafbrekingen beschreven:

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

## <a name="next-steps"></a>Volgende stappen

- [Problemen melden namens uw klant](report-problems-on-behalf-of-a-customer.md)
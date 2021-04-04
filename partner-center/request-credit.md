---
title: Request an SLA credit from Microsoft (Een SLA-tegoed aanvragen van Microsoft)
ms.topic: article
ms.date: 03/31/2021
description: Meer informatie over de voor delen, beperkingen en procedures voor het aanvragen van een service overeenkomst (SLA) van micro soft als uw klanten een service storing ondervinden.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: d33188510b127873864260199ff92018e1a4d995
ms.sourcegitcommit: 766b2bb46dffd29e532b42106359f83e51b96700
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/31/2021
ms.locfileid: "106103822"
---
# <a name="how-and-when-to-request-a-service-level-agreement-sla-credit-from-microsoft"></a>Hoe en wanneer een Service-Level Agreement (SLA)-tegoed van micro soft wordt aangevraagd

U kunt **tegoeden van de service overeenkomst (Sla)** aanvragen bij micro soft als een service die u voor uw klanten levert een storing heeft.

## <a name="sla-credit-calculation"></a>SLA-credit berekening

SLA-credits van micro soft worden bepaald op basis van de betrokken service (s). Als uw klant bijvoorbeeld een Office 365-pakket heeft, maar alleen een share point-onderbreking heeft gehad, wordt het SLA-tegoed alleen goedgekeurd voor share point en niet voor het hele abonnement van de klant.

*De verantwoording wordt pro rata berekend op basis van de betrokken service en de duur van de storing.* Zie het [geconsolideerde Sla-document voor Online Services](http://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=37)voor een overzicht van de scenario's die in aanmerking komen voor sla-credits. Deze informatie is ook van toepassing op Services die via het Cloud Solution Provider-programma worden verkocht.


## <a name="request-an-sla-credit"></a>Een SLA-tegoed aanvragen

*De provider van de Cloud Solution Provider (CSP) moet de claim en alle vereiste gegevens aan het einde van de kalender maand indienen, volgend op de maand waarin het incident heeft plaatsgevonden.* Als het incident bijvoorbeeld op 15 februari heeft plaatsgevonden, moet micro soft de claim en alle vereiste informatie op 31 maart ontvangen. Eind klanten en indirecte wederverkopers kunnen geen SLA-krediet claims verzenden; de indirect provider of de direct factuur partner moet namens hen claims indienen.

>[!NOTE]
>Advies incidenten (de[controle van Microsoft 365 service status](https://docs.microsoft.com/microsoft-365/enterprise/view-service-health?&preserve-view=trueo365-worldwide#incidents-and-advisories)) komen niet in aanmerking voor sla-credits.

### <a name="required-information"></a>Vereiste informatie

De naam van de klant, de Tenant-id, het partner ticket # en de aanmaak datum/tijds tempel van het ticket zijn niet voldoende om een claim te verwerken.

Voordat u [een sla-krediet aanvraag](#submit-sla-credit-request) naar micro soft verzendt, moet u de volgende **informatie verzamelen die** u in uw ondersteunings ticket kunt gebruiken:

- De GUID van de klant Tenant
- De [id van het storings incident](#outage-incident-identifier)?
- Bewijs dat de klant gevolgen heeft gehad voor de storing en een SLA-tegoed heeft aangevraagd.
- Waren de betrokken abonnementen die zijn aangeschaft via CSP? (*Ja* of *Nee*)

#### <a name="evidence-that-proves-customer-impact"></a>Bewijs dat de gevolgen van de klant bewijst

- Informatie over de tijd en duur van de downtime
- Het aantal en de locatie (s) van de betrokken gebruikers (indien van toepassing)
- Beschrijvingen van de pogingen om het incident op het moment van de gebeurtenis op te lossen
- Een e-mail van de betrokken klant die ondersteuning vraagt en vervolgens een tegoed
- Het nummer van de ondersteunings ticket en Details van de contact persoon van de klant met betrekking tot het oplossen van de service-impact


#### <a name="outage-incident-identifier"></a>Id van uitval incident

U kunt de id voor het uitval incident vinden op de pagina **service Health** in het Microsoft 365 beheer centrum. De **id van het onderbrekings incident** is een getal voorafgegaan door een afkorting van twee letters die de betrokken service aanduidt (bijvoorbeeld *EX25194* voor een Exchange Online-onderbreking). In de volgende tabel worden veelvoorkomende afkortingen van services beschreven:

| Afkorting van twee letters | Micro soft-service |
| ----------------------- | ----------------- |
| KADE | Exchange Online |
| FO | Exchange Online-beveiliging |
| SB | Skype voor bedrijven online (voorheen Lync online) |
| Besturingssysteem | Office-abonnement |
| PB | Power BI voor Office 365 |
| SP | SharePoint Online |
| YA | Yammer Enter prise |
| MO | Portal fout |

### <a name="submit-sla-credit-request"></a>SLA-krediet aanvraag indienen

Uw SLA-krediet aanvraag naar micro soft verzenden via het dash board van de partner centrum:

1. Meld u aan bij het dashboard van het Partnercentrum.
2. Kies in het menu links **service aanvragen** en selecteer vervolgens **partner-ondersteunings aanvragen**.
3. Kies op de pagina **partner aanvraag** de optie **nieuwe aanvraag**.
4. Zoek op de pagina **de aanvraag starten** naar de sectie **CSP-klanten, orders en abonnementen**. In deze sectie kiest **u een probleem type selecteren** en selecteert u vervolgens **aanvragen voor tegoeden voor klanten services**.
5. Op de pagina **Aanbevolen oplossingen** onder hebt **u meer hulp nodig? klikt u** op **Ja**.
6. Vul op de pagina **Details** de sectie Details van het **probleem** in. In het tekstvak **Details** moet u de [vereiste informatie](#required-information) invoeren die u eerder hebt verzameld.
7. Kies **verzenden** om in uw sla-krediet aanvraag te verzenden.

## <a name="next-steps"></a>Volgende stappen

- [Problemen namens uw klant melden](report-problems-on-behalf-of-a-customer.md)

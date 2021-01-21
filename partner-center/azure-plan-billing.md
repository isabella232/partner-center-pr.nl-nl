---
title: Facturering van Azure-abonnement-factuur & afstemmings bestanden
ms.topic: article
ms.date: 01/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over de bestands structuur van de factuur en reconciliatie die betrekking heeft op facturering voor het Azure-abonnement.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: e230cc0d8ff3afea4bf2cc7b55d3847814696af6
ms.sourcegitcommit: f99424919f0d77bbe4f44293d84f9ea1e3317f13
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/21/2021
ms.locfileid: "98658430"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nieuwe Commerce-ervaring in CSP - Azure-facturering 

**Juiste rollen**

- Beheer agent
- Factureringsbeheerder
- Globale beheerder

In dit artikel wordt uitgelegd hoe u de bestands structuur van de factuur en de reconciliatie voor het Azure-abonnement kunt openen en begrijpen. Facturering onder het Azure-abonnement is een vereenvoudigde facturerings ervaring met behulp van een uitgelijnde enkele facturerings datum en facturerings periode op basis van een kalender maand.

## <a name="summary-of-billing-essentials"></a>Samen vatting van de basis beginselen van facturering

- **Factuur datum**: factuur-en afstemmings bestand is beschikbaar in het dash board van de partner centrum/API door de achtste (middernacht UTC).

- **Facturerings periode factuur**: de facturerings periode van de factuur is uitgelijnd op de kalender maand, bijvoorbeeld 10/1-10/31, 11/1-11/30.

- **Kosten voor service perioden**: kosten worden uitgelijnd op de kalender maand. Als er bijvoorbeeld een gefactureerde partner Azure-Services toevoegt via een Azure-abonnement op 10/15 en de klant begint met het verbruik van Azure-Services op 10/15, ontvangt de factuur dan op basis van het gebruik van facturen/afstemming op 11/8 voor klant verbruik voor de service periode 10/15-10/31. De factuur van de volgende maand die wordt gegenereerd op 12/8 bevat alle kosten voor de service periode 11/1-11/31.

- **Factuur betalings termijn**: netto 60 dagen.

- **Factuur valuta**: partners worden nog steeds gefactureerd in de country's toegewezen valuta van de klant. Als de gefactureerde partner zich bijvoorbeeld in Ierland bevindt met klanten in het Verenigd Konink rijk, Noor wegen en Duitsland, ontvangt de gefactureerde partner een factuur/afstemming van GBP, NOK en EUR.

- **Partner prikkels**: betaalde 45 dagen aan het einde van de factuur maand.

## <a name="access-your-invoices-and-reconciliation-files"></a>Toegang tot uw facturen en reconciliatie bestanden

De globale beheerder of facturerings beheerder van uw bedrijf ontvangt een e-mail wanneer een factuur gereed is om te worden weer gegeven.

Om toegang te krijgen tot de factuur en het afstemmings bestand:

1. Meld u aan bij het [dashboard](https://partner.microsoft.com/dashboard/) van het Partnercentrum.

2. Selecteer **facturering** in het menu van het partner centrum.

3. Selecteer het tabblad voor de **terugkerende** en **eenmalige** en de valuta waarin u bent geïnteresseerd.

   :::image type="content" source="images/azure/billing3.png" alt-text="verrekeningscode":::

4. Selecteer **factuur** of **afstemmings bestand**.  

   Als u historische facturen en afstemmings bestanden wilt weer geven, vouwt u de rij facturerings geschiedenis hieronder uit.

## <a name="understanding-usage-data"></a>Informatie over gebruiks gegevens 

1. Azure-plan is de hoofd container of het hoogste niveau voor gebruik. Al het gebruik is gekoppeld aan één Azure-abonnement.

2. Binnen een plan worden er een of meer Azure-abonnementen. Dit zijn containers die worden gebruikt voor het beheren en implementeren van resources. 

3. Binnen een abonnement voegen resource groepen toe aan groeps resources. Elke resource wordt geïmplementeerd in één resource groep. 

4. Voor beelden van resources zijn virtuele machines en opslag accounts. 

5. Resource-verzend meters: meters zijn metingen van het verbruik van een resource en een resource kan gebruik voor meerdere meters verzenden. Meters worden aangeduid met een ProductId, SKUId en AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hiërarchie van abonnements resource groepen en-meting

**Azure-account (Tenant)**

- Abonnement A
    - ResourceGroup 1
        - Virtuele machine (resource)
            - Reken meter
        - Virtueel netwerk (resource)
            - Geen facturerings meter

    - ResourceGroup 2
        - Virtuele machine (resource)
            - Computer meter
        - Premium-SSD-beheerde schijf (resource)
            - Opslag capaciteits meter
            - Meter voor opslag bewerkingen

- Abonnement B-ResourceGroup 1-Azure SQL (resource)-DTU-meter-VPN Gateway (resource)-VPN-gateway meter

    - ResourceGroup 2
        - Virtual Network-Interface (resource)
            - Geen facturerings meter

## <a name="read-the-invoice"></a>De factuur lezen

1. Factuur is niet later beschikbaar dan de achtste van elke maand.

2. Partners hebben 60 dagen de betaling te betalen.

3. De facturerings periode geldt voor een bepaalde kalender maand, bijvoorbeeld 10/1-10/31.

4. Kosten zijn netto-aanpassingen (de hoeveelheid is net of het tegoed van de partner voor beheerde services).

5. Bekijk het factuur afstemmings bestand en het dagelijks geclassificeerde gebruiks bestand voor aanvullende facturerings gegevens.

   :::image type="content" source="images/azure/invoice1.png" alt-text="betalen":::

## <a name="read-the-invoice-reconciliation-file"></a>Het afstemmings bestand van de factuur lezen

1. Elk Azure-abonnement en elke combi natie van meters kunnen Maxi maal twee facturerings regels bevatten voor het afstemmings bestand.

2. Als de meter die wordt gebruikt voor elk type korting of tegoed (zoals gelaagde kortingen of de partner die is gefactureerd voor services die worden beheerd) in de hele kalender maand voor komt, bevat het afstemmings bestand slechts één facturerings regel. In de kolom **PriceAdjusmentDescription** wordt verwezen naar de korting of het tegoed.

3. Als er geen resources zijn voor een bepaalde meter die is gekwalificeerd voor de korting of het tegoed van een partner, dan bevat het afstemmings bestand slechts één facturerings regel en de werkelijke eenheids prijs is de prijs van de goed keuring (de prijs per eenheid).

4. Als de meter of resources die deze meter uitbrengen, gekwalificeerd zijn voor een partner die wordt **beheerd** voor een deel van de maand, bevat het afstemmings bestand twee facturerings regels. Eén regel staat voor de dagen waarin de meting is gekwalificeerd en de tweede regel geeft de dagen aan die de meter niet in aanmerking komt.

## <a name="read-the-daily-usage-file"></a>Het dagelijks gebruiks bestand lezen

- Abonnements meters onder een Azure-abonnement worden beoordeeld en worden op dagelijkse basis gecumuleerd.

- Het **tegoed van de partner voor beheerde services** wordt dagelijks bepaald en toegepast.

- Elke abonnements meter heeft een rij voor elke dag van de maand waarin het verbruik is.

- In het voorbeeld hieronder:

  - De ingangs prijs voor de partner die wordt **beheerd** via 7/1-7/3 (Houd rekening met de prijzen van de werkelijke eenheid is de prijs van de verkoop op het tegoed van de partner.

  - De meter is niet gekwalificeerd voor het tegoed van de **partner voor services** die worden beheerd via 7/4-7/7 (de werkelijke eenheids prijs is de verkoop prijs).

  - Meting die geschikt is voor de partner die wordt beheerd via 7/8-7/31 (de werkelijke prijs van een eenheid is de prijs van de **onderneming** , het tegoed van de partner.

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2":::

## <a name="invoice-in-customer-currency"></a>Factuur in klant valuta

Voor Azure-Services via een Azure-abonnement geldt een prijs in USD en gefactureerd in de toegewezen valuta van het klant land. Als de facturerings valuta niet-USD is, wordt de gebruikte FX-tarief op de laatste pagina van de factuur weer gegeven. De FX-tarieven worden maandelijks bepaald en toegepast op de volgende factuur. Bekijk de [nieuwe Commerce-Beschik baarheid voor landen en de matrix voor klant](https://go.microsoft.com/fwlink/?linkid=2112354)valuta's voor een volledige lijst met landen valuta's.

Micro soft volgt de Londen aandelen beurs voor conversie. We gebruiken de wissel koers, die gelijk is aan de wissel koers die is vastgelegd op de laatste seconde van de laatste werkdag van de maand op de beurs in Londen. De FX-tarieven worden vernieuwd en beschikbaar op de dag vóór de eerste van de maand waarop ze van toepassing zijn.

## <a name="azure-reservations"></a>Azure-reserveringen


Als u [Azure-reserve ringen](azure-reservations.md) aanschaft via een Azure-abonnement, kunt u kiezen voor eenmalige of maandelijkse facturering.


## <a name="azure-spending"></a>Uitgaven voor Azure

De bestaande Azure-bestedings ervaring is bijgewerkt ter ondersteuning van de nieuwe Azure plan-facturering in Partner Center. Hierdoor kunnen partners:

- Waarschuwingen voor budget sets op klant niveau weer geven, beheren en ontvangen 

- Totale geschatte uitgaven voor een Azure-abonnement weer geven (gesplitst op resource-en meter niveau)

Omdat het facturerings model voor Azure-Services via een Azure-abonnement post-pay-verbruik is, om een grotere factuur te voor komen dan verwacht, kunnen partners een maandelijks budget Toep assen en het percentage van het gebruik bijhouden. Een budget kan worden toegepast op één klant of meerdere klanten tegelijk. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Uitgaven voor Azure":::

## <a name="next-steps"></a>Volgende stappen

- Bekijk hoe het tegoed van de partner (PEC) wordt berekend. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard/) van het partner centrum en zoek de prijs lijst die beschikbaar is.

- Meer informatie over [het aanschaffen van het Azure-abonnement](purchase-azure-plan.md)

- Zie de [prijs lijst voor de nieuwe Commerce-ervaring in CSP](azure-plan-price-list.md)

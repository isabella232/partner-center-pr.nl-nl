---
title: Facturering van Azure-plan - &-bestanden
ms.topic: article
ms.date: 05/19/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Meer informatie over het openen en begrijpen van de factuur- en afstemmingsbestandsstructuur met betrekking tot facturering voor het Azure-plan.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7e2abdc7536521e72265d99369f165eb7c13d7ae8c258e5db6f84fd774877c19
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115691274"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nieuwe Commerce-ervaring in CSP - Azure-facturering 

**Juiste rollen:** beheeragent | Factureringsbeheerder | Globale beheerder

In dit artikel wordt uitgelegd hoe u de factuur- en afstemmingsbestandsstructuur met betrekking tot facturering voor het Azure-plan kunt openen en begrijpen. Facturering onder het Azure-plan is een vereenvoudigde factureringservaring met behulp van een uitgelijnde factureringsdatum en factureringsperiode op basis van een kalendermaand.

## <a name="summary-of-billing-essentials"></a>Samenvatting van de belangrijkste factureringsgegevens

- **Factuurdatum:** Het factuur- en afstemmingsbestand is op de 8e (middernacht UTC) beschikbaar in Partner Center dashboard/API.

- Factuurfactureringsperiode: de factuurfactureringsperiode is afgestemd op de kalendermaand, bijvoorbeeld 10/1-10/31, 11/1-11/30.

- **Serviceperioden voor** kosten: de kosten worden afgestemd op de kalendermaand. Als de gefactureerde partner bijvoorbeeld Azure-services toevoegt via een Azure-plan op 15-10-2015 en de klant het verbruik van Azure-services op 10/15 begint, ontvangt de gefactureerde partner factuur/recon op 11/8 voor klantverbruik voor de serviceperiode 10/15 - 10/31. De factuur van de volgende maand die wordt gegenereerd op 12/8 bevat alle kosten voor de serviceperiode 11/1- 11/31.

- **Betalingstermijn factuur:** netto 60 dagen.

- Factuurvaluta: vanaf 28 januari 2021 worden partners in de regio EU/EFTA en het VERENIGD Koninkrijk die nieuwe klanten hebben en bestaande CSP-klanten die voor het eerst nieuwe commerceaanbiedingen aanschaffen waarvan de tenants zijn gemaakt vóór 11 mei 2020, gefactureerd voor deze aankopen in partnerlocatievaluta. Partners die zich buiten de regio EU/EFTA en het VK bevinden, worden nog steeds gefactureerd in partnerlocatievaluta.

- **Incentives voor partners:** betaalde 45 dagen vanaf het einde van de factuurmaand.

## <a name="access-your-invoices-and-reconciliation-files"></a>Toegang tot uw facturen en afstemmingsbestanden

De globale beheerder of factureringsbeheerder voor uw bedrijf ontvangt een e-mail wanneer een factuur gereed is om te worden bekeken.

Voor toegang tot het factuur- en afstemmingsbestand:

1. Meld u aan bij het [dashboard](https://partner.microsoft.com/dashboard/) van het Partnercentrum.

2. Selecteer in Partner Center menu **Facturering.**

3. Selecteer het tabblad **Terugkerend en** **Eenmalige** en de valuta waarin u geïnteresseerd bent.

   :::image type="content" source="images/azure/billing3.png" alt-text="Facturering.":::

4. Selecteer **Factuur-** **of afstemmingsbestand.**  

   Als u historische facturen en recon-bestanden wilt weergeven, vouwt u de onderstaande rij Factureringsgeschiedenis uit.

## <a name="understanding-usage-data"></a>Inzicht in gebruiksgegevens 

1. Azure-plan is de hoofdcontainer of container op het hoogste niveau voor gebruik. Al het gebruik is gekoppeld aan één Azure-plan.

2. Binnen een abonnement zijn er een of meer Azure-abonnementen. Dit zijn containers die worden gebruikt voor resourcebeheer en implementatie. 

3. Binnen een abonnement voegen resourcegroepen toe aan groepsresources. Elke resource wordt geïmplementeerd in één resourcegroep. 

4. Voorbeelden van resources zijn virtuele machines en opslagaccounts. 

5. Bronmeters: Meters zijn metingen van het verbruik van een resource en één resource kan het gebruik voor meerdere meters gebruiken. Meters worden geïdentificeerd door een ProductId, SKUId en AvailabilityId. 

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hiërarchie van abonnementsresourcegroepen en meting

**Azure-account (tenant)**

- Abonnement A
    - ResourceGroup 1
        - Virtuele machine (resource)
            - Rekenmeter
        - Virtueel netwerk (resource)
            - Geen factureringsmeter

    - ResourceGroup 2
        - Virtuele machine (resource)
            - Computermeter
        - Premium Ssd-beheerde schijf (resource)
            - Storage capaciteitsmeter
            - Storage operations meter

- Abonnement B -ResourceGroup 1 - Azure SQL (resource) - DTU-meter - VPN Gateway (resource) - VPN-gatewaymeter

    - ResourceGroup 2
        - Virtual Network Interface (resource)
            - Geen factureringsmeter

## <a name="read-the-invoice"></a>De factuur lezen

1. Factuur is niet later dan de acht dagen van elke maand beschikbaar.

2. Partners hebben 60 dagen de tijd om de betaling door te geven.

3. De factureringsperiode heeft betrekking op een bepaalde kalendermaand, bijvoorbeeld 10/1-10/31.

4. Kosten zijn netto correcties (bedrag is netto van 'Partnertegoed voor beheerde services').

5. Controleer het factuur recon-bestand en het bestand met dagelijks beoordeeld gebruik voor aanvullende factureringsgegevens.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Factuur.":::

## <a name="read-the-invoice-reconciliation-file"></a>Het factuurafstemmingsbestand lezen

1. Elke combinatie van Azure-plan en -meter kan maximaal twee factureringslijnen in het reconbestand hebben.

2. Als de meter is gekwalificeerd voor elk type korting of tegoed (zoals gelaagde kortingen of het partnertegoed voor beheerde services) gedurende de hele kalendermaand, bevat het reconbestand slechts één factureringsregel. De kolom **PriceAdjusmentDescription verwijst** naar de korting of het verdiend tegoed.

3. Als er geen resources zijn voor een bepaalde meter die geschikt zijn voor korting of partnertegoed, bevat het reconbestand slechts één factureringsregel en is de effectieve eenheidsprijs de detailhandelprijs (de eenheidsprijs).

4. Als de meter of resources die die meter uitzenden, gekwalificeerd zijn voor partnertegoed voor **services** die een deel van de maand worden beheerd, bevat het reconbestand twee factureringslijnen. Eén regel vertegenwoordigt de dagen dat de meter gekwalificeerd is en de tweede regel de dagen dat de meter niet in aanmerking komt.

>[!NOTE]
>U kunt uw Azure-verbruik afstemmen in uw een-keer-aankoop recon-bestand. Als u dit wilt doen, gaat u naar uw dagelijks beoordeelde reconbestand voor gebruik en zoekt u naar uw SubscriptionID. Hiermee worden alle kosten weergegeven die zijn gekoppeld aan uw Azure-plan-id. Uw Azure SubscriptionID wordt weergegeven als de EntitlementID.

## <a name="read-the-daily-usage-file"></a>Het dagelijkse gebruiksbestand lezen

- Abonnementsmeters onder een Azure-plan worden dagelijks beoordeeld en gecumuleerd.

- **Partnertegoed voor beheerde services** wordt dagelijks bepaald en toegepast.

- Elke abonnementsmeter heeft een rij voor elke dag van de maand waarin het verbruik is geweest.

- In het voorbeeld hieronder:

  - Meter die is gekwalificeerd **voor partnertegoed** voor services die worden beheerd van 7/1 - 7/3 (let op: de effectieve eenheidsprijs is de handelsprijs die minder partnertegoed is.

  - Meter komt niet in aanmerking voor **partnertegoed** voor services die worden beheerd van 7-4-7-7-2017 (de effectieve eenheidsprijs is de detailhandelsprijs).

  - Meter die is gekwalificeerd **voor partnertegoed** voor services die worden beheerd van 7/8 - 7/31 (let op: de effectieve eenheidsprijs is de detailhandelsprijs die minder partnertegoed is).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-customer-currency"></a>Factuur in klantvaluta

Azure-services via een Azure-plan worden in USD geprijsd en gefactureerd in de door de klant toegewezen valuta in het land van de klant. Als de factureringsvaluta niet usd is, wordt het gebruikte valutatarief (Foreign Exchange) weergegeven op de laatste pagina van de factuur. FX-tarieven worden maandelijks bepaald en toegepast op de volgende factuur. Voor een volledige lijst met landvaluta bekijkt u de nieuwe commerceaanbiedingen voor de beschikbaarheid van landen en [de valutamatrix van klanten.](https://go.microsoft.com/fwlink/?linkid=2112354)

Microsoft past een vooraf bepaalde wisselkoers toe op basisprijzen van USD om te komen tot de totale kosten voor Azure-services die elke kalendermaand zijn gekocht of verbruikt. De maandelijkse wisselkoers is het tussentijdse tarief dat is gepubliceerd door Den Haags (meestal) twee werkdagen vóór de voorgaande maand om 16:00 GMT. 

**Bijvoorbeeld:** De wisselkoers van Microsoft in december zou voor een bepaalde valuta het middentarief van Den Haags zijn op of rond 29 november. Dit tarief wordt toegepast op alle aankopen in die valuta van 1 december tot en met 31 december. 

## <a name="azure-reservations"></a>Azure-reserveringen


Als u [Azure-reserveringen aanschaft](azure-reservations.md) via een Azure-abonnement, kunt u kiezen voor een een-keer- of maandelijkse facturering.


## <a name="azure-spending"></a>Uitgaven voor Azure

De bestaande Azure-bestedingservaring wordt bijgewerkt ter ondersteuning van de nieuwe facturering van Azure-plannen in Partner Center. Hierdoor kunnen partners:

- Waarschuwingen weergeven, beheren en ontvangen voor budgetten die zijn ingesteld op klantniveau 

- Totale geschatte uitgaven voor een Azure-plan weergeven (onderverdeeld op resource- en meterniveau)

Omdat het factureringsmodel voor Azure-services via een Azure-plan gebruik na betaling is, kunnen partners een maandelijks budget toepassen en het gebruikspercentage bijhouden om een hogere factuur te voorkomen dan verwacht. Een budget kan worden toegepast op één klant of meerdere klanten tegelijk. 

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-uitgaven.":::

## <a name="next-steps"></a>Volgende stappen

- Zie hoe het partnertegoed (PEC) wordt berekend. Meld u aan Partner Center [dashboard en](https://partner.microsoft.com/dashboard/) zoek de prijslijst die beschikbaar is.

- Meer informatie over [het kopen van het Azure-abonnement](purchase-azure-plan.md)

- Zie de [prijslijst voor de nieuwe commerce-ervaring in CSP](azure-plan-price-list.md)

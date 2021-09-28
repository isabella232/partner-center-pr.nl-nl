---
title: Azure-planfacturering - &-bestanden
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Meer informatie over het openen en begrijpen van de factuur- en afstemmingsbestandsstructuur met betrekking tot facturering voor het Azure-plan.
author: khpavan
ms.author: sakhanda
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: ad04b7af67bb4cf664b2a552c94fc96fa25e5349
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089263"
---
# <a name="new-commerce-experience-in-csp---azure-billing"></a>Nieuwe Commerce-ervaring in CSP - Azure-facturering

**Juiste rollen:** beheeragent | Factureringsbeheerders | Globale beheerder

In dit artikel wordt uitgelegd hoe u de factuur- en afstemmingsbestandsstructuur met betrekking tot facturering voor het Azure-plan kunt openen en begrijpen. Facturering onder het Azure-plan is een vereenvoudigde factureringservaring met behulp van een uitgelijnde factureringsdatum en factureringsperiode op basis van een kalendermaand.

## <a name="summary-of-billing-essentials"></a>Samenvatting van de belangrijkste factureringsgegevens

- **Factuurdatum:** Het factuur- en afstemmingsbestand is vanaf de 8e (middernacht UTC) beschikbaar in Partner Center dashboard/API.

- Factuurfactureringsperiode: de factureringsperiode van de factuur wordt afgestemd op de kalendermaand, bijvoorbeeld 10-1-10/31, 11-1-11/30.

- **Serviceperioden voor kosten:** de kosten worden afgestemd op de kalendermaand. Als de gefactureerde partner bijvoorbeeld Azure-services toevoegt via een Azure-abonnement op 15-10-2015 en de klant het verbruik van Azure-services op 15/15 begint, ontvangt de gefactureerde partner factuur/recon voor klantverbruik op 11/8 voor de serviceperiode 10/15 - 10/31. De factuur van de volgende maand die wordt gegenereerd op 12/8 bevat alle kosten voor de serviceperiode 11/1- 11/31.

- **Betalingstermijn factuur:** netto 60 dagen.

- **Factuurvaluta:** vanaf augustus 2021 worden alle partners gefactureerd in de partnerlocatievaluta, ongeacht de locatie van de klant aan wie u de producten hebt verkocht.

- **Incentives voor partners:** betaalde 45 dagen vanaf het einde van de factuurmaand.

## <a name="access-your-invoices-and-reconciliation-files"></a>Toegang tot uw facturen en afstemmingsbestanden

De globale beheerder of factureringsbeheerder voor uw bedrijf ontvangt een e-mail wanneer een factuur gereed is om te worden bekeken.

Voor toegang tot het factuur- en afstemmingsbestand:

> [!NOTE]
> Zie Getting around Partner Center voor meer informatie over [de werkruimte-interface.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Werkruimteweergave](#tab/workspaces-view)

1. Selecteer in [Partner Center dashboard](https://partner.microsoft.com/dashboard/)de **tegel Facturering.**

2. Selecteer het tabblad **Terugkerend en** **Eenmalige** en de valuta waarin u bent geïnteresseerd.

   :::image type="content" source="images/azure/billing-workspace-1.png" alt-text="Schermopname van de factureringsgeschiedenis.":::

3. Selecteer **Factuur-** **of afstemmingsbestand.**

   Als u historische facturen en afstemmingsbestanden wilt weergeven, vouwt u de onderstaande rij Factureringsgeschiedenis uit.

#### <a name="current-view"></a>[Huidige weergave](#tab/current-view)

1. Selecteer in [Partner Center dashboard](https://partner.microsoft.com/dashboard/) **facturering.**

2. Selecteer het tabblad **Terugkerend en** **Eenmalige** en de valuta waarin u bent geïnteresseerd.

   :::image type="content" source="images/azure/billing3.png" alt-text="Facturering.":::

3. Selecteer **Factuur-** **of afstemmingsbestand.**

   Als u historische facturen en afstemmingsbestanden wilt weergeven, vouwt u de onderstaande rij Factureringsgeschiedenis uit.

* * *

## <a name="about-usage-data"></a>Over gebruiksgegevens

- Azure-plan is de hoofdcontainer of container op het hoogste niveau voor gebruik. Al het gebruik is gekoppeld aan één Azure-plan.

- Binnen een abonnement zijn er een of meer Azure-abonnementen. Dit zijn containers die worden gebruikt voor resourcebeheer en implementatie.

- Binnen een abonnement voegen resourcegroepen toe aan groepsresources. Elke resource wordt geïmplementeerd in één resourcegroep.

- Voorbeelden van resources zijn virtuele machines en opslagaccounts.

- Meter voor het gebruik van resources: Meters zijn metingen van het verbruik van een resource en één resource kan gebruik voor meerdere meters gebruiken. Meters worden geïdentificeerd door een ProductId, SKUId en AvailabilityId.

### <a name="hierarchy-of-subscription-resource-groups-and-metering"></a>Hiërarchie van abonnementsresourcegroepen en -meting

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

## <a name="about-your-invoice"></a>Over uw factuur

- Factuur is niet later dan de acht dagen van elke maand beschikbaar.

- Partners hebben 60 dagen de tijd om de betaling te betalen.

- De factureringsperiode heeft betrekking op een bepaalde kalendermaand, bijvoorbeeld 10-1-10/31.

- Kosten zijn netto aanpassingen (bedrag is netto van 'Partnertegoed voor beheerde services').

- Controleer het recon-bestand van de factuur en het bestand met dagelijks beoordeeld gebruik voor aanvullende factureringsgegevens.

   :::image type="content" source="images/azure/invoice1.png" alt-text="Factuur.":::

## <a name="about-your-invoice-reconciliation-file"></a>Over uw factuurafstemmingsbestand

- Elke combinatie van Azure-plan en -meter kan maximaal twee factureringslijnen in het afstemmingsbestand (recon) hebben.

- Als de meter is gekwalificeerd voor elk type korting of tegoed (zoals gelaagde kortingen of het partnertegoed voor beheerde services) gedurende de hele kalendermaand, bevat het reconsgetal slechts één factureringsregel. De kolom **PriceAdjusmentDescription verwijst** naar de korting of het verdiend tegoed.

- Als er geen resources zijn voor een bepaalde meter die in aanmerking komen voor korting of partnertegoed, bevat het recon-bestand slechts één factureringsregel en is de effectieve eenheidsprijs de detailhandelprijs (de eenheidsprijs).

- Als de meter, of resources die die meter uitzenden, is gekwalificeerd voor partnertegoed voor **services** die een deel van de maand worden beheerd, bevat het recon-bestand twee factureringsregels. Eén regel vertegenwoordigt de dagen dat de meter is gekwalificeerd en de tweede regel de dagen dat de meter niet in aanmerking komt.

> [!NOTE]
> U kunt uw Azure-verbruik afstemmen in uw een-time recon-bestand voor aankopen. Als u dit wilt doen, gaat u naar het reconbestand met dagelijks beoordeelde gebruiksgegevens en zoekt u naar uw SubscriptionID. Hiermee worden alle kosten weergegeven die zijn gekoppeld aan uw Azure-plan-id. Uw Azure SubscriptionID wordt weergegeven als de EntitlementID.

## <a name="read-the-daily-usage-file"></a>Het dagelijkse gebruiksbestand lezen

- Abonnementsmeters onder een Azure-abonnement worden dagelijks beoordeeld en gecumuleerd.

- **Partnertegoed voor beheerde services** wordt dagelijks bepaald en toegepast.

- Elke abonnementsmeter heeft een rij voor elke dag van de maand waarin het verbruik is geweest.

- In het voorbeeld hieronder:

  - Meter die is gekwalificeerd voor **partnertegoed** voor services die worden beheerd van 7/1 - 7/3 (let op: de effectieve eenheidsprijs is de detailhandelprijs minder partnertegoed.

  - Meter komt niet in aanmerking voor **partnertegoed** voor services die worden beheerd op 7-7-7-2017 (de effectieve eenheidsprijs is de detailhandelsprijs).

  - Meter die is gekwalificeerd voor **partnertegoed** voor services die worden beheerd van 7-7-31-2031 (de effectieve eenheidsprijs is de detailhandelprijs minder partnertegoed).

   :::image type="content" source="images/azure/pecfinal.png" alt-text="recon2.":::

## <a name="invoice-in-partner-location-currency"></a>Factuur in partnerlocatievaluta

Azure-services via een Azure-plan worden in USD gefactureerd en gefactureerd in de toegewezen valuta van het partnerland. Als de factureringsvaluta niet usd is, wordt het gebruikte valutatarief (FX) weergegeven op de laatste pagina van de factuur. FX-tarieven worden maandelijks bepaald en toegepast op de volgende factuur. Bekijk voor een volledige lijst met valuta's per land de nieuwe commerceaanbiedingen voor de beschikbaarheid van landen en [de partnervalutamatrix.](https://go.microsoft.com/fwlink/?linkid=2112354)

Microsoft past een vooraf bepaalde wisselkoers toe op basisprijzen van USD om te komen tot de totale kosten voor Azure-services die elke kalendermaand zijn gekocht of verbruikt. De maandelijkse wisselkoers is het middentarief dat is gepubliceerd door Deen (meestal) twee werkdagen vóór de voorgaande maand om 16:00 GMT.

**Bijvoorbeeld:** De wisselkoers van Microsoft in december zou voor een bepaalde valuta het middentarief van Den Middelingen zijn op of rond 29 november. Dit tarief wordt toegepast op alle aankopen in die valuta van 1 december tot en met 31 december.

## <a name="azure-reservations"></a>Azure-reserveringen

Als u [Azure-reserveringen aanschaft](azure-reservations.md) via een Azure-abonnement, kunt u een een time- of maandelijkse facturering kiezen.

## <a name="azure-spending"></a>Uitgaven voor Azure

De bestaande Azure-bestedingservaring wordt bijgewerkt ter ondersteuning van de nieuwe facturering van Azure-plannen in Partner Center. Hierdoor kunnen partners:

- Waarschuwingen weergeven, beheren en ontvangen voor budgetten die zijn ingesteld op klantniveau

- Totale geschatte uitgaven voor een Azure-plan weergeven (onderverdeeld op resource- en meterniveau)

Omdat het factureringsmodel voor Azure-services via een Azure-abonnement gebruik na betaling is, kunnen partners een maandelijks budget toepassen en het gebruikspercentage bijhouden om een hogere factuur te voorkomen dan verwacht. Een budget kan worden toegepast op één klant of meerdere klanten tegelijk.

:::image type="content" source="images/azure/azurespend.png" alt-text="Azure-uitgaven.":::

## <a name="next-steps"></a>Volgende stappen

- Zie hoe het partnertegoed (PEC) wordt berekend. Meld u aan bij [Partner Center dashboard en](https://partner.microsoft.com/dashboard/) selecteer de **tegel Prijzen** om de beschikbare prijslijsten te vinden.

- Meer informatie over [het kopen van het Azure-abonnement](purchase-azure-plan.md)

- Bekijk de [prijslijst voor de nieuwe commerce-ervaring in CSP](azure-plan-price-list.md)

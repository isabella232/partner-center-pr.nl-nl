---
title: Inzicht in uw factuur- en afstemmingsbestand
ms.topic: article
ms.date: 09/27/2021
description: Meer informatie over uw factuur- & afstemmingsbestanden. Uw factuur toont Partner Center kosten voor het programma, de producten en klanten voor die maandelijkse periode.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: df1e7f4aa34c44f0fcb030cda3df1d6f9cb241f9
ms.sourcegitcommit: e1da62b36420d78bf44e3962358d0af65ebc3402
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129089518"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Inzicht in uw factuur- en afstemmingsbestand - informatie over hoe u deze kunt vinden in Partner Center

**Juiste rollen:** globale | Factureringsbeheerders | Beheeragent

Uw factuur is een overzicht van al uw Partner Center kosten voor het programma, alle producten en alle klanten.

## <a name="find-your-bill-and-reconciliation-file"></a>Uw factuur- en afstemmingsbestand zoeken

U vindt uw factuur op de pagina Facturering van het dashboard in Partner Center. Op deze pagina vindt u ook uw factureringsgeschiedenis, bestedingstrends en afstemmingsbestanden.

> [!NOTE]
> Zie Voor meer informatie over de werkruimte-interface [Getting around Partner Center](get-around-partner-center.md#turn-workspaces-on-and-off).

#### <a name="workspaces-view"></a>[Werkruimtenweergave](#tab/workspaces-view)

1. Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/home).

2. Selecteer de **tegel** Facturering.

3. Selecteer een factuur- of afstemmingsbestand om gedetailleerdere informatie weer te geven.

Boven aan de pagina vindt u een koppeling naar uw meest recente factuur onder Rekeningsaldo vanaf de laatste factuurdatum.

Vorige facturen vindt u in de sectie Factureringsgeschiedenis. Kies het juiste jaar en selecteer vervolgens de vervolgkeuzepijl naast de juiste factureringsperiode. Selecteer de koppeling naast Facturen (.pdf) om de factuur van die periode te downloaden.

#### <a name="current-view"></a>[Huidige weergave](#tab/current-view)

1. Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/home).

2. Selecteer facturering in het menu aan de **linkerkant.**

3. Selecteer op de pagina met de factuurstatus een factuur of afstemmingsbestand om gedetailleerdere informatie weer te geven.

Boven aan de pagina vindt u een koppeling naar uw meest recente factuur onder Rekeningsaldo vanaf de laatste factuurdatum.

Vorige facturen vindt u in de sectie Factureringsgeschiedenis. Kies het juiste jaar en selecteer vervolgens de vervolgkeuzepijl naast de juiste factureringsperiode. Selecteer de koppeling naast Facturen (.pdf) om de factuur van die periode te downloaden.

* * *

## <a name="invoice-types"></a>Factuurtypen

Microsoft geeft één factuur uit voor kosten op basis van licenties (zoals Office 365) en kosten op basis van gebruik (zoals Azure) en een afzonderlijke factuur voor een een time-kosten (zoals Azure RI, Marketplace of Azure-plan).

Bijvoorbeeld:  

**Scenario 1 [enkele valuta]**: Partner heeft aankopen voor 145P-aanbieding en Office 365 licenties,  

- Partner ontvangt één PDF-factuur en twee afstemmingsbestanden voor de kosten voor zowel Office 365 als Azure (145p).  

**Scenario 2 [enkele valuta]**: De partner heeft aankopen voor Azure RI, Marketplace en/of een Azure-abonnement, samen met 145p-aankopen.

- Partner ontvangt één PDF-factuur en één afstemmingsbestand voor de kosten voor Azure (145p). 

- De partner ontvangt een ander PDF-factuurbestand en één afstemmingsbestand met de kosten voor gereserveerde Azure-instanties (RI), Marketplace, Azure-plan. 

**Scenario 3 [meerdere valuta's]**: De partner heeft aankopen voor Azure RI in DKK en een Azure-plan in EURO, samen met 145p-aankopen in EURO.

- De partner ontvangt één PDF-factuur en één afstemmingsbestand voor de kosten voor Azure RI in DKK. 

- De partner ontvangt één PDF-factuur en één afstemmingsbestand voor de kosten voor het Azure-plan in DEN. 

- Partner ontvangt een ander PDF-factuurbestand en één afstemmingsbestand voor de kosten voor 145p-aanbieding in EURO (of partnerfactureringsvaluta). 

## <a name="understanding-invoice-pdf"></a>Informatie over factuur-PDF 

**Facturen voor kosten** op basis van gebruik en licenties: facturen voor kosten voor services zoals Office 365 en Azure zijn beschikbaar binnen twee (2) dagen na de geselecteerde factureringsdatum [UTC].  

**Facturen voor eenmalige en** terugkerende kosten: Facturen voor kosten voor services zoals Azure RI, Azure-plan en Marketplace zijn niet later dan de acht dagen van elke maand beschikbaar.  

Hieronder vindt u enkele van de belangrijkste velden in het PDF-document voor facturen:

**Factuurnummer:** de unieke id voor het factuurdocument dat is gegenereerd voor de respectieve factureringsperiode. 

**Factureringsperiode:** dit is de periode waarin u gebruiks- en licentieservices hebt. 

**Factuurdatum:** de factureringsdatum of jubileumdatum waarop uw factuur elke maand wordt gegenereerd. 

**Einddatum van betaling:** de datum waarop uw betaling moet worden ontvangen. 

**Kosten:** het verschuldigde bedrag in uw factureringsvaluta voor de respectieve factureringsperiode. 

**Tegoeden:** tegoed (zoals sla (Service Level Agreement) of aanpassingen voor wijzigingen in abonnementen (bijvoorbeeld toename of afname van licenties). 

**Betalingsinstructies:** beschrijving van het betalen van uw factuur, op basis van uw regio. Zorg er altijd voor dat u uw factuurnummer bij het doen van een betaling op uw factuur vermeldt. 

Zie Velden voor factuurbestand voor een gedetailleerde beschrijving van alle velden in uw factuurbestand (inclusief velden voor een [een time-charges).](invoice-file.md) 

## <a name="understand-reconciliation-files"></a>Afstemmingsbestanden begrijpen

 Afstemmingsbestanden, die een inzoom-/gespecificeerde details van uw kosten bieden, kunnen samen met de pdf-factuur worden gedownload. De afstemmingsbestanden bevatten klant-id's en abonnements-id's die u kunt gebruiken om klantfacturen te maken. Zie De afstemmingsbestanden gebruiken voor meer informatie [over afstemmingsbestanden.](use-the-reconciliation-files.md) 

## <a name="next-steps"></a>Volgende stappen

- [De afstemmingsbestanden gebruiken](use-the-reconciliation-files.md)
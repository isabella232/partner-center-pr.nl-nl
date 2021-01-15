---
title: Uw factuur & afstemmings bestand lezen
ms.topic: article
ms.date: 06/05/2020
description: Meer informatie over uw factuur & reconciliatie bestanden. Uw factuur toont de kosten voor het partner centrum in het programma, producten en klanten voor die maandelijkse periode.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 43c2605d750d35bc2e0095b1fed413ed91a1a28e
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215812"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Meer informatie over uw factuur-en afstemmings bestand-lees hoe u deze kunt vinden in Partner Center


**Juiste rollen**

- Globale beheerder
- Factureringsbeheerder
- Beheer agent


Uw **factuur** is een **samen vatting van de kosten van uw partner centrum** (in het programma, alle producten en alle klanten). 

## <a name="invoice-types"></a>Factuur typen

Micro soft verleent één factuur voor eventuele kosten op basis van licenties (zoals Office 365) en kosten op basis van gebruik (zoals Azure) en een afzonderlijke factuur voor eenmalige kosten (zoals Azure RI, Marketplace of Azure-abonnement).

Bijvoorbeeld:  

**Scenario 1 [enkele valuta]**: de partner heeft aankopen voor de 145P-aanbieding en O365-licenties.  

- Partner ontvangt één factuur-PDF en 2 afstemmings bestanden voor de kosten voor O365 en Azure (145p).  

**Scenario 2 [enkele valuta]**: de partner heeft aankopen gedaan voor Azure RI, Marketplace en/of Azure, samen met 145p-aankopen.

- Partner ontvangt één factuur-PDF en een afstemmings bestand met de kosten voor Azure (145p). 

- De partner ontvangt een andere factuur-PDF en een afstemmings bestand met de kosten voor Azure RI, Marketplace, Azure-abonnement. 

**Scenario 3 [Multi-Currency]**: partner heeft aankopen voor Azure ri in DKK en Azure-abonnement in EUR samen met 145p-aankopen in EUR.

- Partner ontvangt één factuur-PDF en een afstemmings bestand met de kosten voor Azure RI in DKK. 

- Partner ontvangt één factuur-PDF en een afstemmings bestand met de kosten voor Azure-plan in EUR. 

- De partner ontvangt een andere factuur-PDF en een afstemmings bestand met de kosten voor de 145p-aanbieding in EUR (of de facturerings valuta van de partner). 

## <a name="find-your-bill"></a>Uw factuur zoeken 

U kunt uw factuur vinden op de facturerings pagina van het dash board in Partner Center. U kunt ook uw facturerings geschiedenis, bestedings trends en afstemmings bestanden op deze pagina vinden. 

1. Meld u aan bij het [dashboard](https://partner.microsoft.com/dashboard/home) van het Partnercentrum. 

2. Selecteer **facturering** in het menu aan de linkerkant. 

3. Selecteer op de pagina facturering de factuur die u wilt downloaden. 

U vindt een koppeling naar uw laatste factuur boven aan de pagina onder account saldo vanaf de laatste factuur datum. 

U kunt de vorige facturen vinden in de sectie facturerings geschiedenis. Kies het juiste jaar en selecteer vervolgens de vervolg keuze pijl naast de juiste facturerings periode. Selecteer de koppeling naast facturen (. PDF) om de factuur van die periode te downloaden. 

## <a name="understanding-invoice-pdf"></a>Factuur PDF 

**Facturen voor gebruik en kosten op basis van licenties**: facturen voor de kosten voor services, zoals Office 365 en Azure, zijn binnen twee (2) dagen na de geselecteerde facturerings datum [UTC] beschikbaar.  

**Facturen voor eenmalige en terugkerende kosten**: facturen voor de kosten voor services zoals Azure RI, Azure-abonnement en Marketplace zijn niet later dan achtste van elke maand beschikbaar.  

Hieronder ziet u enkele van de belangrijkste velden in het factuur PDF-document –

**Factuur nummer**: de unieke id voor het factuur document dat voor de desbetreffende facturerings periode is gegenereerd. 

**Facturerings periode**: dit is de periode waarin u gebruik hebt en services op basis van licenties. 

**Factuur datum**: de factuur datum of jubileum datum waarop uw factuur per maand wordt gegenereerd. 

**Verval datum betaling**: de datum waarop uw betaling moet worden ontvangen. 

**Kosten**: het verschuldigde bedrag in uw facturerings valuta voor de desbetreffende facturerings periode. 

**Tegoeden**: tegoed (zoals sla) of aanpassingen voor wijzigingen in abonnementen (bijvoorbeeld licentie verhogen of afname). 

**Betalings instructies**: hier wordt beschreven hoe u uw factuur kunt betalen op basis van uw regio. Zorg er altijd voor dat u uw factuur nummer opgeeft wanneer u een betaling doet. 

Zie [factuur bestands velden](invoice-file.md)voor een gedetailleerde beschrijving van alle velden in uw factuur bestand (inclusief velden voor eenmalige kosten). 

## <a name="understand-reconciliation-files"></a>Informatie over afstemmings bestanden

 Reconciliatie bestanden, die een inzoomen/gedetailleerde Details van uw kosten bieden, zijn beschikbaar om samen met de factuur-PDF te worden gedownload. De afstemmings bestanden bevatten klant-id's en abonnements-id's die u kunt gebruiken om klant facturen te maken. Raadpleeg  [How to use the reconciliatie files](use-the-reconciliation-files.md) voor meer informatie over de afstemmings bestanden. 

## <a name="next-steps"></a>Volgende stappen

- [De reconciliatie bestanden gebruiken](use-the-reconciliation-files.md)
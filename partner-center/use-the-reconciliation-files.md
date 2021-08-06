---
title: Uw afstemmingsbestanden gebruiken
ms.topic: article
ms.date: 03/26/2021
description: Meer informatie over afstemmingsbestanden in Partner Center en hoe u de gedetailleerde weergaven van de kosten voor een bepaalde factureringscyclus kunt interpreteren.
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2b14379f7e7750b3423d03be4addaca4e4a6a94834709b9f0b6e5891a185bb0c
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681192"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Informatie over het lezen van de regelitems in uw Partner Center afstemmingsbestanden

**Juiste rollen:** Factureringsbeheerders | Globale beheerder

U kunt uw afstemmingsbestanden downloaden Partner Center voor een gedetailleerde weergave van alle kosten in een factureringscyclus. Details van regelitem omvatten kosten voor de abonnementen van elke klant en gedetailleerde gebeurtenissen (zoals het op de korte termijn toevoegen van licenties aan een abonnement).

Zie Uw factuur lezen voor **meer informatie** over het lezen van [uw factuur.](read-your-bill.md)

## <a name="understand-reconciliation-file-fields"></a>Velden voor afstemmingsbestand begrijpen

- [Velden voor afstemmingsbestand op basis van licentie](license-based-recon-files.md)
- [Velden voor afstemmingsbestand op basis van gebruik](usage-based-recon-files.md)
- [Velden voor afstemmingsbestand over dagelijks gebruik](daily-rated-usage-recon-files.md)
- [Velden voor CSP-afstemmingsbestand voor een een time-aankoop](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Inzicht in kostentypen in afstemmingsbestanden

Zie Kostentypen voor afstemmingsbestand voor meer [](recon-file-charge-types.md)informatie over de typen kosten in afstemmingsbestanden (de kolom **ChargeType).**

## <a name="fix-formatting-issues"></a>Opmaakproblemen oplossen

Af en toe kan een afstemmingsbestand opmaakproblemen bevatten. Dit probleem kan bijvoorbeeld optreden als de en-US-locale niet wordt gebruikt.

Volg deze stappen om eventuele opmaakproblemen in uw afstemmingsbestanden op te lossen:

1. Open het afstemmingsbestand (in .csv indeling) in Microsoft Excel.
2. Selecteer de eerste kolom in het bestand.
3. Open de **wizard Tekst converteren naar kolommen.** Selecteer op het lint **Gegevens** en selecteer vervolgens Tekst **naar kolommen.**
4. Selecteer in de wizard **Bestandstype met scheidingstekens.** Selecteer vervolgens **Volgende**.
5. Selecteer in **het veld Scheidingstekens** de optie **Komma**. (Als **Tab** al is geselecteerd, kunt u deze optie ingeschakeld laten.) Selecteer vervolgens **Volgende.**
6. Selecteer **datum:MDY** **in** het veld Kolomgegevensindeling. Selecteer vervolgens **Volgende**.
7. Selecteer in **het veld Kolomgegevensindeling** de optie **Tekst** voor alle hoeveelheid kolommen. Selecteer vervolgens **Voltooien**.

## <a name="download-reconciliation-files-programmatically"></a>Afstemmingsbestanden programmatisch downloaden

Afstemmingsbestanden kunnen erg groot zijn en zijn soms moeilijk te downloaden. Zie Factuurregelitems downloaden om afstemmingsbestanden programmatisch [te downloaden.](/partner-center/develop/get-invoiceline-items)

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Als uw bestand de rijlimiet in de Excel

Als u een afstemmingsbestand kunt downloaden maar niet kunt openen in Microsoft Excel, betekent dit waarschijnlijk dat het bestand meer rijen bevat dan Excel toestaat. Als dit gebeurt, kunt u een van de onderstaande procedures gebruiken om het bestand te openen.

### <a name="open-a-recon-file-in-power-bi"></a>Open een reconbestand in Power BI

1. Download het afstemmingsbestand zoals u dat normaal zou doen.
2. Download, installeer en open een exemplaar van Microsoft Power BI.
3. Selecteer op Power BI **tabblad Start** de optie **Gegevens verzamelen.**
4. Selecteer **Tekst/CSV** **in** de lijst met algemene gegevensbronnen.
5. Wanneer u hier om wordt gevraagd, opent u het recon-bestand.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Een reconbestand openen in een Excel draaitabel

1. Download het afstemmingsbestand zoals u dat normaal zou doen.
2. Open een nieuw bestand in Microsoft Excel.
3. Selecteer op **het** tabblad Gegevens de optie **Gegevens downloaden,** selecteer **Uit bestand** en selecteer vervolgens **Tekst/CSV.**
4. Wanneer u hier om wordt gevraagd, opent u het recon-bestand. Uw gegevens worden weergegeven.
5. Selecteer in **de** vervolgkeuzelijst Laden de optie **Laden naar** en selecteer vervolgens **OK.**
6. Selecteer in **het dialoogvenster Gegevens** importeren de optie **Draaitabelrapport om** het bestand te openen.

## <a name="negative-amount-displayed"></a>Negatief bedrag weergegeven

Mogelijk ziet u een negatief bedrag in uw afstemmingsbestand. Dit wordt mogelijk veroorzaakt door een van de volgende zaken:

- U hebt het aantal licenties onlangs geannuleerd of verlaagd
- U hebt tegoed ontvangen voor een servicelicentieovereenkomst (SLA) of voor Azure-verbruik

Voor meer informatie over deze transactie raadpleegt u de bijbehorende kostentype-eigenschap in uw afstemmingsbestand.

## <a name="map-taxes-or-vat"></a>Btw of btw in kaart brengen

Belastingen of btw-waarde (BTW) aan uw factuur toe te voegen:

- Som de **kolom Belasting** op uit het op licenties gebaseerde bestand.
- Som de **kolom TaxAmount** op uit het bestand op basis van gebruik.

## <a name="itemize-reconciliation-files-by-partner"></a>Afstemmingsbestanden itemeren per partner

Partners in het **indirecte model kunnen** deze aanvullende velden gebruiken in zowel op licenties gebaseerde als op gebruik gebaseerde afstemmingsbestanden om de bestanden per reseller te itemeren.

| MPN-id | Description |
| ------ | ----------- |
| MPN-id | De Microsoft Partner Network (MPN)-id van de Cloud Solution Provider (CSP)-partner (direct of indirect). |
| [MPN-id van reseller](#reseller-mpn-id) | De [MPN-id van de reseller van de record voor het abonnement](#reseller-mpn-id). Dit veld komt overeen met de reseller-id die wordt vermeld voor het specifieke abonnement in Partner Center. Wordt alleen weergegeven in afstemmingsbestanden voor partners in het indirecte model. |

### <a name="reseller-mpn-id"></a>MPN-id voor reseller

Als een CSP-partner het abonnement rechtstreeks aan de klant heeft verkocht, wordt de **MPN-id** twee keer vermeld, zowel als de **MPN-id** van de reseller en de **MPN-id** van de reseller.

Als een CSP-partner een reseller zonder **MPN-id** heeft, wordt deze waarde in plaats daarvan ingesteld op de **MPN-id van de partner.**

Als de CSP-partner een **MPN-id** voor resellers verwijdert, wordt deze waarde ingesteld *op -1.*

Als u de MPN-id van **de reseller wilt weergeven of bijwerken:**

1. Meld u aan bij Partnercentrum.
2. Selecteer in Partner Center menu **Klanten.**
3. Kies de klant in de lijst.
4. Selecteer Abonnementen in het menu **van de klant.**
5. Kies het abonnement in de lijst.
6. Selecteer **Update om** de Reseller **(MPN-id) te wijzigen.**

## <a name="next-steps"></a>Volgende stappen

- [Uw factuur lezen & recon-bestand](read-your-bill.md) 
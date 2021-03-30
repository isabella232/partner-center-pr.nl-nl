---
title: Uw afstemmings bestanden gebruiken
ms.topic: article
ms.date: 03/26/2021
description: Meer informatie over reconciliatie bestanden in het partner centrum en het interpreteren van gedetailleerde weer gaven van het regel item van kosten voor een bepaalde facturerings cyclus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aefd5258c778fd8a7b92bfe49f245bf818497fb8
ms.sourcegitcommit: dd51744a4af3797493a5ebbfc766dab86ff00477
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/29/2021
ms.locfileid: "105730076"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Meer informatie over het lezen van regel items in uw partner centrum-afstemmings bestanden

**Juiste rollen**

- Factureringsbeheerder
- Globale beheerder

U kunt uw afstemmings bestanden downloaden van het partner centrum voor een gedetailleerde weer gave van regel items van elke kosten in een facturerings cyclus. Details van regel items zijn kosten voor abonnementen van elke klant en gedetailleerde gebeurtenissen (zoals een middel grote aanvulling van licenties voor een abonnement).

Zie [uw factuur lezen](read-your-bill.md)voor meer informatie over het lezen van uw **facturen**.

## <a name="understand-reconciliation-file-fields"></a>Informatie over afstemmings bestand velden

- [Velden voor afstemmingsbestand op basis van licentie](license-based-recon-files.md)
- [Velden voor afstemmingsbestand op basis van gebruik](usage-based-recon-files.md)
- [Velden voor afstemmingsbestand over dagelijks gebruik](daily-rated-usage-recon-files.md)
- [Eenmalige inkopen CSP-afstemmings bestand velden](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Meer informatie over kosten typen in afstemmings bestanden

Zie [reconciliatie bestands toeslag typen](recon-file-charge-types.md)voor meer informatie over de typen kosten in reconciliatie bestanden (de kolom **ChargeType** ).

## <a name="fix-formatting-issues"></a>Opmaak problemen oplossen

Af en toe kan een afstemmings bestand opmaak problemen bevatten. Dit probleem kan bijvoorbeeld optreden als de land instelling en niet wordt gebruikt.

Volg deze stappen voor het oplossen van problemen met de opmaak in uw afstemmings bestanden:

1. Open het afstemmings bestand (in CSV-indeling) in micro soft Excel.
2. Selecteer de eerste kolom in het bestand.
3. Open de **wizard tekst naar kolommen converteren**. Selecteer op het lint de optie **gegevens** en selecteer vervolgens **tekst naar kolommen**.
4. Selecteer in de wizard **gescheiden bestands type**. Selecteer vervolgens **Volgende**.
5. Selecteer **komma** in het veld scheidings **tekens** . (Als **tabblad** al is geselecteerd, kunt u deze optie ingeschakeld laten.) Selecteer vervolgens **volgende**.
6. Selecteer in het veld **kolom gegevens indeling** de optie **datum: MDJ**. Selecteer vervolgens **Volgende**.
7. Selecteer in het veld **kolom gegevens indeling** de **tekst** voor alle bedragkolommen. Selecteer vervolgens **Voltooien**.

## <a name="download-reconciliation-files-programmatically"></a>Afstemmings bestanden programmatisch downloaden

Afstemmings bestanden kunnen erg groot zijn en soms moeilijk te downloaden. Zie [factuur regel items ophalen](/partner-center/develop/get-invoiceline-items)om de afstemmings bestanden via een programma te downloaden.

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Als uw bestand de rijlimiet in Excel overschrijdt

Als u een afstemmings bestand kunt downloaden, maar niet in micro soft Excel wilt openen, betekent dit waarschijnlijk dat het bestand meer rijen bevat dan Excel toestaat. Als dit het geval is, kunt u een van de onderstaande procedures gebruiken om het bestand te openen.

### <a name="open-a-recon-file-in-power-bi"></a>Een afstemmings bestand openen in Power BI

1. Down load het afstemmings bestand zoals u dat gewend bent.
2. Down load, installeer en open een exemplaar van Power BI.
3. Selecteer op het tabblad Power BI **Start** de optie **gegevens ophalen**.
4. Selecteer in de lijst met **algemene gegevens bronnen** de optie **tekst/CSV**.
5. Open uw afstemmings bestand wanneer u hierom wordt gevraagd.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Een afstemmings bestand openen in een Excel-draai tabel

1. Down load het afstemmings bestand zoals u dat gewend bent.
2. Open een nieuw bestand in micro soft Excel.
3. Op het tabblad **gegevens** selecteert u **gegevens ophalen**, selecteert u **uit bestand** en selecteert u vervolgens **tekst/CSV**.
4. Open uw afstemmings bestand wanneer u hierom wordt gevraagd. Uw gegevens worden weer gegeven.
5. Selecteer in de vervolg keuzelijst **laden** de optie **laden naar** en klik vervolgens op **OK**.
6. Selecteer in het dialoog venster **gegevens importeren** het **draai tabel rapport** om het bestand te openen.

## <a name="negative-amount-displayed"></a>Weer gegeven negatief bedrag

Mogelijk wordt er een negatief bedrag in het afstemmings bestand weer geven. Dit wordt waarschijnlijk veroorzaakt door een van de volgende dingen:

- U hebt uw aantal licenties onlangs geannuleerd of gereduceerd
- U hebt een tegoed ontvangen voor een service licentieovereenkomst (SLA) of voor Azure-verbruik

Als u meer informatie wilt over deze trans actie, controleert u het kenmerk van het type kosten in het afstemmings bestand.

## <a name="map-taxes-or-vat"></a>Belastingen of BTW toewijzen

BTW of belasting toegevoegde waarde (BTW) toewijzen aan uw factuur:

- Som van de **belasting** kolom van het bestand op basis van licentie.
- Som van de kolom **TaxAmount** van het bestand op basis van gebruik.

## <a name="itemize-reconciliation-files-by-partner"></a>Afstemmings bestanden specificeren op partner

Partners in het **indirecte model** kunnen deze extra velden gebruiken in zowel op licenties gebaseerde afstemmings bestanden als voor het specificeren van de bestanden op reseller.

| MPN-id | Beschrijving |
| ------ | ----------- |
| MPN-id | De Microsoft Partner Network-ID (MPN) van de Cloud Solution Provider (CSP)-partner (direct of indirect). |
| [Reseller MPN-ID](#reseller-mpn-id) | De [MPN-id van de dealer van de record voor het abonnement](#reseller-mpn-id). Dit veld komt overeen met de wederverkoper-ID die wordt vermeld voor het specifieke abonnement in partner centrum. Wordt alleen weer gegeven voor reconciliatie bestanden voor partners in het indirecte model. |

### <a name="reseller-mpn-id"></a>Reseller MPN-ID

Als een CSP-partner het abonnement rechtstreeks aan de klant heeft verkocht, wordt hun **MPN-id** twee keer vermeld, zowel de **MPN-id** als de **wederverkoper MPN-id**.

Als een CSP-partner een wederverkoper heeft zonder **MPN-id**, wordt deze waarde in plaats daarvan ingesteld op de **MPN-id** van de partner.

Als de CSP-partner een **wederverkoper MPN-id** verwijdert, wordt deze waarde ingesteld op *-1*.

De **wederverkoper MPN-id** weer geven of bijwerken:

1. Meld u aan bij Partnercentrum.
2. Selecteer **klanten** in het menu van het partner centrum.
3. Kies de klant in de lijst.
4. Selecteer in het menu klant de optie **abonnementen**.
5. Kies het abonnement in de lijst.
6. Selecteer **bijwerken** om de wederverkoper te wijzigen **(MPN-id)**.

## <a name="next-steps"></a>Volgende stappen

- [Uw factuur & afstemmings bestand lezen](read-your-bill.md) 
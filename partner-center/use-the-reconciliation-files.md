---
title: Uw afstemmings bestanden gebruiken
ms.topic: article
ms.date: 06/08/2020
description: Meer informatie over reconciliatie bestanden in het partner centrum en het interpreteren van gedetailleerde weer gaven van het regel item van kosten voor een bepaalde facturerings cyclus.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d927b138c32b3e5f6f5d906db898e17f89a85aae
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101755781"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Meer informatie over het lezen van regel items in uw partner centrum-afstemmings bestanden

Van toepassing op:

- Partnercentrum
- Partnercentrum voor Microsoft Cloud for US Government

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
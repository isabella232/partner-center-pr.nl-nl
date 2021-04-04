---
title: Factuur facturen van partner Center begrijpen
ms.topic: article
ms.date: 05/18/2020
description: Inzicht in de velden in het factuur bestand voor het factureren van het partner centrum. Opgenomen zijn velden en definities voor alle factuur velden en velden met eenmalige kosten.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 44bda5256b14722f143a5bf937e73b2533b8c9f5
ms.sourcegitcommit: 6498c57e75aa097861523b206dc142f789deeb36
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/02/2021
ms.locfileid: "106178898"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Informatie over de facturerings factuur velden van partner Center

**Juiste rollen**

- Globale beheerder
- Beheerder van gebruikers beheer
- Factureringsbeheerder
- Helpdesk medewerker

U kunt de volgende tabellen gebruiken om inzicht te krijgen in de velden in de factuur bestanden van partner Center.

## <a name="invoice-file-fields"></a>Factuur bestands velden

De volgende velden worden op uw factuur bestanden weer gegeven.

| Veld | Definitie |
| ----- | ---------- |
| VS-FEIN | Uw Federal werkgevers id-nummer (FEIN). Dit is uw Verenigde Staten id-nummer van de federale belasting. |
| Klant nummer | Uw klant nummer. |
| Factureren aan | Het adres waarnaar we uw factuur verzenden. U kunt de naam en het adres van uw bedrijf wijzigen in het facturerings Profiel van uw partner centrum. |
| Kosten op basis van licenties | De vaste maandelijkse of jaarlijkse kosten voor uw gekochte op gebruik gebaseerde licenties, vóór de service gefactureerd. Dit aantal is de som van alle kosten in de kolom **Subtotaal** (kolom **T**) in het afstemmings bestand op basis van licenties. |
| Kosten op basis van gebruik | Uw Azure-gebruik. Dit geldt ook voor nieuwe services of toepassingen die tijdens de facturerings periode zijn ingeschakeld en gebruikt. Dit aantal is de som van alle kosten in de kolom **PretaxCharges** (kolom **Z**) in het afstemmings bestand op basis van gebruik. |
| Kortingen | De korting die de klant ontvangt van de normale prijs van het abonnement. Dit aantal wordt weer gegeven als een *vaste hoeveelheid*, niet als een prijs per eenheid of licentie. |
| Tegoeden | Tegoeden of aanpassingen voor wijzigingen in abonnementen (bijvoorbeeld licentie verhogen of afname). |
| Subtotaal | Totaal vóór belastingen en kosten en tegoed. |
| Btw | De totale belastingen voor uw huidige kosten, zoals deze worden opgeteld in het gedeelte met **Details** , beginnend op pagina 2 van uw factuur. Dit aantal is de som van alle kosten in de kolom **TaxAmount** (kolom **AA**) in uw afstemmings bestand op basis van gebruik en de kolom **belasting** (kolom **U**) in het afstemmings bestand op basis van licenties. |
| Overige tegoeden | Tegoed-exclusieve bedragen. |
| Totale huidige kosten | Het verschuldigde bedrag in uw facturerings valuta voor de facturerings periode. Deze kosten moeten worden betaald door de verval datum van de betaling. |
| Betalingsinstructies | Beschrijving van hoe u uw factuur kunt betalen op basis van uw regio. *Zorg er altijd voor dat u uw factuur nummer opgeeft wanneer u een betaling doet.* |
| Factuur nummer | Het nummer van uw factuur. |
| Factureringsperiode | De maandelijkse periode tot en met de factuur datum. Dit is de periode waarin op gebruik gebaseerde services worden verbruikt en op licenties gebaseerde services worden afgestemd op eventuele krediet aanpassingen of wijzigingen in het aantal licenties. |
| Factuurdatum | De factuur datum of jubileum datum waarop uw factuur per maand wordt gegenereerd. |
| Betalingsvoorwaarden | De betalings termijn. Voor eenmalige aankopen is dit altijd 60 dagen. |
| Verval datum betaling | De datum waarop uw betaling moet worden ontvangen. |
| IO van klant | De volg orde van uw aankoop nummer. |
| Klantenservice | Het website adres waar u toegang hebt tot de klanten service. |
| Ontvanger van service | Het adres waar de service wordt gebruikt. (Dit is het juridische bedrijfs adres dat is gekoppeld aan het bedrijf hebben.) |

## <a name="one-time-charges-fields"></a>Velden met eenmalige kosten

De volgende velden zijn alleen van toepassing op **eenmalige kosten** in Partner Center:

| Veld | Definitie |
| ----- | ---------- |
| Date | Aankoop datum. |
| Beschrijving | Product naam. |
| Aantal | Het aantal producten (zoals reserve ringen) dat is gekocht. |
| Eenheidsprijs | Prijs per product (zoals een reserve ring). |
| Kortingen | Alle toepasselijke kortingen. |
| Bedrag vóór belastingen | Subtotaal van de aankopen vóór belastingen. |
| Omzet belasting | Belasting bedrag. |
| Totaal | Het totale bedrag dat moet worden betaald. |

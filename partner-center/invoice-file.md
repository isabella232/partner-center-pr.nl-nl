---
title: Inzicht in Partner Center factureringsfacturen
ms.topic: article
ms.date: 05/18/2020
description: Informatie over de velden in uw factuurbestand voor Partner Center facturering. Opgenomen zijn velden en definities voor alle factuurvelden en velden met een eenkostendefinities voor één keer.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c741caa6993a5da415d3a94d541bf10c21470889
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957514"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Inzicht in Partner Center velden voor factureringsfacturering

**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Factureringsbeheerder | Helpdeskagent

U kunt de volgende tabellen gebruiken om inzicht te krijgen in de velden in Partner Center factuurbestanden.

## <a name="invoice-file-fields"></a>Velden voor factuurbestand

De volgende velden worden weergegeven in uw factuurbestanden.

| Veld | Definitie |
| ----- | ---------- |
| US FEIN | Uw federale werkgeveridentificatienummer (FEIN). Dit is uw Verenigde Staten federal tax identifier-nummer. |
| Klantnummer | Uw klantnummer. |
| Factureren aan | Het adres waar we uw factuur verzenden. U kunt uw bedrijfsnaam en -adres wijzigen in uw Partner Center factureringsprofiel. |
| Kosten op basis van licenties | De vaste maandelijkse of jaarlijkse kosten voor uw aangeschafte licenties op basis van gebruik, die worden gefactureerd voor de service. Dit getal is de som van alle kosten in de **kolom Subtotaal (kolom** **T**) in uw afstemmingsbestand op basis van licenties. |
| Kosten op basis van gebruik | Uw Azure-gebruik. Dit omvat nieuwe services of toepassingen die tijdens de factureringsperiode zijn ingeschakeld en gebruikt. Dit getal is de som van alle kosten in de kolom **PretaxCharges** (kolom **Z**) in uw afstemmingsbestand op basis van gebruik. |
| Kortingen | De korting die de klant ontvangt van de normale prijs van het abonnement. Dit getal wordt weergegeven als een *vast bedrag,* niet als een prijs per eenheid of licentie. |
| Tegoeden | Tegoeden of aanpassingen voor wijzigingen in abonnementen (bijvoorbeeld toename of afname van licenties). |
| Subtotaal | Totaal vóór belastingen en exclusief btw-kosten en tegoed. |
| Btw | De totale belasting voor uw huidige kosten, zoals wordt weergegeven in de **sectie Details** die begint op pagina 2 van uw factuur. Dit getal is de som van alle kosten in de **kolom TaxAmount** (kolom  **AA**) in uw op gebruik gebaseerde afstemmingsbestand en de kolom Belasting (kolom **U**) in uw afstemmingsbestand op basis van licenties. |
| Overige tegoeden | Exclusief belastingtegoed. |
| Totale huidige kosten | Het verschuldigde bedrag in uw factureringsvaluta voor de factureringsperiode. Deze kosten zijn verschuldigd op de einddatum van de betaling. |
| Betalingsinstructies | Beschrijving van hoe u uw factuur betaalt, op basis van uw regio. *Zorg er altijd voor dat u uw factuurnummer bij het doen van een betaling op uw factuur vermeldt.* |
| Factuur nee | Het nummer van uw factuur. |
| Factureringsperiode | De maandelijkse periode voorafgaand aan de factuurdatum. Dit is de periode waarin services op basis van gebruik worden gebruikt en op licenties gebaseerde services worden afgestemd op eventuele tegoedcorrecties of wijzigingen in het aantal licenties. |
| Factuurdatum | De factureringsdatum of jubileumdatum waarop uw factuur elke maand wordt gegenereerd. |
| Betalingsvoorwaarden | De betalingstermijn. Voor een eendaagse aankopen is dit altijd 60 dagen. |
| Einddatum van betaling | De datum waarop uw betaling moet worden ontvangen. |
| Klant-PO | Uw inkoopnummerorder. |
| Klantenservice | Het websiteadres waar u toegang hebt tot de klantenservice. |
| Ontvanger van de service | Het adres waar de service wordt gebruikt. (Dit is het adres van het juridische bedrijf dat is gekoppeld aan de bedrijfsde doorlichting.) |

## <a name="one-time-charges-fields"></a>Velden voor eenkosten voor een keer

De volgende velden zijn alleen van toepassing **op een een time-kosten** in Partner Center:

| Veld | Definitie |
| ----- | ---------- |
| Date | Aankoopdatum. |
| Description | Productnaam. |
| Aantal | Het aantal aangeschafte producten (zoals reserveringen). |
| Eenheidsprijs | Prijs per product (zoals een reservering). |
| Kortingen | Eventuele toepasselijke kortingen. |
| Bedrag vóór belasting | Subtotaal van de aankopen vóór belastingen. |
| Btw | Btw-bedrag. |
| Totaal | Het totale bedrag dat moet worden betaald. |

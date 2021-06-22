---
title: Afstemmingsbestanden op basis van gebruik
ms.topic: article
ms.date: 06/08/2020
description: Meer informatie over alle items in uw op gebruik gebaseerde afstemmingsbestand in Partner Center. Bevat enkele voorbeelden.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6c486d4866b0a2a912801d2648a1822418687078
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431706"
---
# <a name="understand-usage-based-reconciliation-files-and-their-specific-fields-in-partner-center"></a>Informatie over op gebruik gebaseerde afstemmingsbestanden en hun specifieke velden in Partner Center

**Juiste rollen:** Accountbeheerder | Factureringsbeheerder

Als u uw kosten wilt afstemmen op het gebruik van een klant, vergelijkt  u **resellerID,** **ResellerName** en  **ResellerBillableAccount** uit het afstemmingsbestand met de naam van de klant en de abonnements-id van Partner Center.

## <a name="fields-in-usage-based-reconciliation-files"></a>Velden in op gebruik gebaseerde afstemmingsbestanden

In de volgende velden wordt uitgelegd welke services zijn gebruikt en wat de snelheid is.

| Kolom | Beschrijving | Voorbeeldwaarde(n) |
| ------ | ----------- | ------------ |
| PartnerId | Partner-id, in GUID-indeling. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| PartnerName | Naam van de partner. | *Contoso Ltd.* |
| PartnerBillableAccountId | Partneraccount-id. | *1010578050* |
| CustomerCompanyName | De organisatienaam van de klant, zoals vermeld in Partner Center. *Dit is heel belangrijk voor het afstemmen van de factuur met uw systeemgegevens.* | *Testklant* |
| MpnId | Microsoft Partner Network (MPN)-id van de Cloud Solution Provider (CSP)-partner. | *4390934* |
| ResellerMpnId | MPN-id van de wederverkoper van record voor het abonnement.  |
| InvoiceNumber | Factuurnummer waar de opgegeven transactie wordt weergegeven. | *D020001IVK* |
| ChargeStartDate | Begindatum van factureringscyclus, behalve bij het presenteren van datums van eerder niet-in rekening gebrachte latente gebruiksgegevens (van de vorige factuurcyclus). De tijd is altijd het begin van de dag, 0:00. | *2/1/2019 0:00* |
| ChargeEndDate | Einddatum van factureringscyclus, behalve bij het presenteren van datums van eerder niet-in rekening gebrachte latente gebruiksgegevens (van de vorige factuurcyclus). De tijd is altijd het einde van de dag, 23:59. | *2/28/2019 23:59* |
| SubscriptionId | Unieke id voor een abonnement in het Microsoft-factureringsplatform. Kan handig zijn om het abonnement te identificeren wanneer u contact op met de ondersteuning opzegt. Niet gebruikt voor afstemming. *Dit is niet hetzelfde als de **abonnements-id** in de beheerconsole van de partner.* | *usCBMgAAAAAAAAIA* |
| SubscriptionName | Bijnaam voor de serviceaanbieding. | *Microsoft Azure* |
| SubscriptionDescription | Line-Of-Business van de serviceaanbieding. | *Microsoft Azure* |
| OrderID | Unieke id voor een bestelling in het Microsoft-factureringsplatform. Kan handig zijn om het abonnement te identificeren wanneer u contact op met de ondersteuning opzegt. Niet gebruikt voor afstemming. | *566890604832738111* |
| ServiceName | De naam van de azure-service in kwestie. | *VIRTUELE MACHINES* |
| ServiceType | Het specifieke type Azure-service. | *Service Bus: individueel of pack,* *SQL Azure-database – Business of Web Edition* |
| ResourceGuid | Specifieke unieke id voor alle servicegegevens en prijsstructuur. | *DA41BC5F-C52D-4464-8A8D-8C8DCC43503B* |
| ResourceName | De naam van de Azure-resource. | *Gegevensoverdracht in (GB),* *gegevensoverdracht uit (GB)* |
| Region | De regio waarop het gebruik van toepassing is. Wordt voornamelijk gebruikt om tarieven toe te wijzen aan gegevensoverdrachten, omdat de tarieven per regio verschillen. | *Azië en Stille Oceaan*, *Europa*, *Latijns-Amerika*, *Noord-Amerika* |
| Sku | Unieke Microsoft-id voor een aanbieding. | *7UD-00001* |
| DetailLineItemId | Een id en hoeveelheid voor het itemeren van verschillende tarieven voor een service of resource in een bepaalde factureringsperiode. Voor gelaagde Azure-prijzen kan er één tarief zijn voor een bepaald aantal factureerbare eenheden en vervolgens een ander tarief na die hoeveelheid. | *1* |
| ConsumedQuantity | De hoeveelheid service die tijdens de rapportageperiode is verbruikt (zoals uren of GB). Omvat ook niet-gebilled gebruik van eerdere rapportageperioden. | *11* |
| IncludedQuantity | Eenheden die zijn opgenomen als onderdeel van de aanbieding. Meestal niet aanwezig in CSP. | *0* |
| OverageQuantity | Eenheden die niet zijn opgenomen als onderdeel van de aanbieding. Deze moeten worden betaald door de partner. Gelijk aan **ConsumedQuantity** min **IncludedQuantity**. | *11* |
| ListPrice | Aanbiedingsprijs van kracht op de begindatum van het abonnement. | *$ 0,0808* |
| PretaxCharges | Gelijk aan **ListPrist** vermenigvuldigd **met OverageQuantity,** afgerond op de dichtstbijzijnde cent. | *$ 0,085* |
| TaxAmount | Belastingbedrag in rekening gebracht. Op basis van de belastingregels en specifieke omstandigheden van uw markt. | *$ 0,08* |
| PostTaxTotal | Totaal na belasting, indien van toepassing. | *$ 0,93* |
| Valuta | Valutatype. Elke factureringsentiteit heeft slechts één valuta. Controleer of deze overeenkomt met uw eerste factuur en vervolgens na belangrijke updates voor het factureringsplatform. | *EUR* |
| PretaxEffectiveRate | Prijs vóór belasting per eenheid. Gelijk aan **PretaxCharges** gedeeld door **OverageQuantity,** afgerond op de dichtstbijzijnde cent. | *$ 0,08* |
| PostTaxEffectiveRate | Prijs na belasting per eenheid. Gelijk aan **PostTaxTotal** gedeeld door **OverageQuantity,** afgerond op de dichtstbijzijnde cent. Of gelijk aan **PretaxEffectiveRate** plus het belastingtarief per eenheidsbedrag, afgerond op de dichtstbijzijnde cent. | *$ 0,08* |
| ChargeType | Het [type kosten of](recon-file-charge-types.md) correctie. | Zie [Kostentypen.](recon-file-charge-types.md) |
| CustomerId | Unieke Microsoft-id voor de klant, in GUID-indeling. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| DomainName | Domeinnaam van de klant. Dit veld kan leeg zijn tot de tweede factureringscyclus. | *example.onmicrosoft.com* |
| BillingCycleType | Tijdsfactureringsfrequentie.| **Maandelijks**  |
| Eenheid | De eenheid van de **resourcenaam**. | *GB of* *UREN* |
| CustomerBillableAccount | Unieke account-id in het Microsoft-factureringsplatform. | *1280018095* |
| UsageDate | Datum van service-implementatie. | *2/1/2019 0:00* |
| MeteredRegion | Hiermee wordt de locatie van een datacenter binnen de regio geïdentificeerd (voor services waar deze waarde van toepassing is en ingevuld). | *Azië - oost*, *South Azië - oost*, *Europa - noord*, *Europa - west*, VS - *noord-centraal*, VS - *zuid-centraal* |
| MeteredService | Identificeert het gebruik van de afzonderlijke Azure-service wanneer deze niet specifiek wordt geïdentificeerd in de **kolom ServiceName.** Gegevensoverdrachten worden bijvoorbeeld gerapporteerd als *Microsoft Azure - Alle services* in de kolom **ServiceName.** | *AccessControl,* *CDN,* *Compute,* *Database,* *ServiceBus,* *Storage* |
| MeteredServiceType | Subkoping voor **het veld MeteredService** met aanvullende uitleg over het gebruik van de Azure-service. | *Externe* |
| Project | Door de klant gedefinieerde naam voor het service-exemplaar. | *ORDDC52E52FDEF405786F0642DD0108BE4* |
| ServiceInfo | Het aantal Azure Service Bus verbindingen dat op een bepaalde dag is ingericht en gebruikt. | *1.00000 verbindingen /30* dagen (als u een afzonderlijk inrichtende verbinding hebt gedurende een maand van 30 dagen), *25 verbindingen /30 dagen – gebruikt: 1,000000* (als u 25 Service Bus-verbindingen hebt ingericht en die dag 1 hebt gebruikt) |

## <a name="next-steps"></a>Volgende stappen

- [Inzicht in de velden in Partner Center op licenties gebaseerde afstemmingsbestanden](license-based-recon-files.md)
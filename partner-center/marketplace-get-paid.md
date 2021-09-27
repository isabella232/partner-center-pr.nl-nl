---
title: Betaald krijgen in Partner Center
description: Meer informatie over het ontvangen van betalingen voor inkomsten als Een Microsoft-partner, zoals via aanbiedingen op de commerciële marketplace, incentive-programma's en het Cloud Solution Provider programma. Omvat uitbetalingsbeleid, uitbetalingsstatus en uitbetalingsverklaringen.
ms.service: partner-dashboard
ms.subservice: partnercenter-payouts
ms.topic: conceptual
ms.date: 09/21/2021
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: 5a98a4ef3c1064a64dd2af46ce3a83a0a73589d6
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075261"
---
# <a name="getting-paid-in-partner-center"></a>Betaald krijgen in Partner Center

**Juiste rollen:** Accountbeheerder | Globale beheerder

Dit artikel bevat belangrijke informatie over het ontvangen van betaling voor uw aanbiedingen, invoegtoepassingen en advertentie-inkomsten. Het bevat een overzicht van het uitbetalingsbeleid, de stappen die vereist zijn voordat u betaald krijgt, en een overzicht van het uitbetalingsoverzicht.

## <a name="payout-policies-and-agreements"></a>Uitbetalingsbeleid en overeenkomsten

Als u betaald wilt krijgen, moet u zich houden aan de overeenkomsten en het uitbetalingsbeleid.

- [Microsoft Azure Marketplace Publisher overeenkomst:](/legal/marketplace/msft-publisher-agreement)voordat u betaald krijgt, moet u deze uitgeversovereenkomst accepteren. In deze overeenkomst wordt uitgelegd wat de relatie tussen u en Microsoft is wanneer deze betrekking heeft op verkopersaanbiedingen in de commerciële marketplace, met inbegrip van de winkelkosten die Microsoft in rekening brengt voor elke verkoop.
- [Uitbetalingsbeleid toont](payout-policy-details.md) het betalingsbeleid voor uitbetaling, inclusief betalingsplanning en betalingswijzen. In het beleid wordt ook het proces voor niet-betalingen van klanten uitgelegd.
- [In Belastingdetails](tax-details-marketplace.md) wordt de btw-overweging voor prijsselectie en belastingverantwoordelijkheid onder de Microsoft [Publisher-overeenkomst uitgelegd.](/legal/marketplace/msft-publisher-agreement)
- **Winkelkosten worden** officieel aangeboden in [Commerciële Marketplace-kosten.](/azure/marketplace/marketplace-commercial-transaction-capabilities-and-considerations)
- **Betalingen** worden maandelijks uitgevoerd (op voorwaarde dat aan de betalingsdrempelwaarde is voldaan). Normaal gesproken verzenden we elke betaling die in een bepaalde maand op de 15e dag van die maand moet worden betaald. Het duurt over het algemeen 3 tot 10 extra werkdagen om uw uitbetalingsaccount te bereiken. Zie Betalingsdrempels, methoden en [tijdframes voor meer informatie.](payment-thresholds-methods-timeframes.md)

## <a name="prerequisite-steps-before-getting-paid"></a>Vereiste stappen voordat u betaald krijgt

Voordat u de eerste keer wordt betaald, moet u uw uitbetalingsaccount instellen en de benodigde bank- en belastingformulieren invullen. In bank- en belastingformulieren geeft u uw voorkeursbetalingsmethoden en de belastingformulieren voor bronbelasting op. Bank- en belastingformulieren zijn vereist voordat we u kunnen betalen. Zie Uw uitbetalingsaccount [en belastingformulieren instellen voor meer informatie.](set-up-your-payout-account.md)

### <a name="payout-hold-status"></a>Wachtstatus uitbetaling

Standaard verzenden we betalingen op maandelijkse basis, zoals hierboven wordt beschreven. U kunt uw uitbetalingen voor een programma echter in de wacht zetten en Microsoft zal uw betalingen niet vrijgeven aan uw account. Als u ervoor kiest om uw uitbetalingen in de wacht te zetten, blijven we eventuele inkomsten opnemen op de **pagina Uitbetalingen.** We sturen echter geen betalingen naar uw account totdat u de wachtstand hebt verwijderd.

Als u uw betalingen in de wacht wilt zetten, selecteert **Instellingen** het tandwielpictogram rechtsboven en vervolgens **Accountinstellingen.** Selecteer **Uitbetaling en belasting** in het  menu links en zoek in de sectie Toewijzing van uitbetalings- en belastingprofiel het programma waarvoor u betalingen wilt houden. Schakel het **selectievakje Mijn betaling in** de wacht houden in om betalingen voor dit programma op te houden. U kunt de status van uw uitbetalings hold op elk moment wijzigen, maar uw beslissing is van invloed op de volgende maandelijkse uitbetaling. Als u bijvoorbeeld de uitbetaling van april wilt behouden, moet u  vóór eind maart de status van uw uitbetalings hold instellen op Aan.

Zodra u uw wachtstatus voor uitbetaling hebt ingesteld op **Aan,** worden alle uitbetalingen voor dit programma in de wacht gezet totdat u het selectievakje uit bij **Uit hebt uitgeschakeld.** Wanneer u dit doet, wordt u opgenomen tijdens de volgende maandelijkse uitbetalingscyclus (mits is voldaan aan de betalingsdrempelwaarde). Als uw uitbetalingen in de wacht staan, maar u een uitbetaling wilt genereren  in juni, wist u het selectievakje uit vóór eind mei.

>[!Note]
> Uw uitbetalingsstatus is afzonderlijk van toepassing op elk programma (Microsoft Store, advertenties, Azure Marketplace, etc.). Als u betalingen voor al uw programma's wilt houden, moet u voor elk programma afzonderlijk betalen.

## <a name="payout-statements"></a>Uitbetalingsinstructies

Het uitbetalingsoverzicht toont uw inkomsten uit de verkoop van uw aanbiedingen en invoegtoepassingen in de transactiegeschiedenis. U kunt ook betalingsgegevens bekijken en rapporten downloaden in tsv- of CSV-indeling. Zie [Uitbetalingsoverzichten](payout-statement.md) voor meer informatie over het openen van het uitbetalingsoverzicht en de details van de transactiegeschiedenis en betalingsrapporten. Daarnaast kunt u de API voor uitbetalingen van partners gebruiken om systematisch de [uitbetalingsrapporten](https://apidocs.microsoft.com/services/partnerpayouts) op te halen.

## <a name="next-steps"></a>Volgende stappen

- [Api voor uitbetalingen van partners](https://apidocs.microsoft.com/services/partnerpayouts)
- [Veelgestelde vragen over uitbetalingen](payout-faq.yml)
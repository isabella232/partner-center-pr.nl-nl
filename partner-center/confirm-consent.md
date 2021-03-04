---
title: Acceptatie door de klant van Microsoft-klantovereenkomst bevestigen
description: Meer informatie over het bevestigen van de acceptatie van de klant door de klant overeenkomst van micro soft. Dit kan nodig zijn om micro soft-producten en-services voor klanten te best Ellen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/02/2021
ms.openlocfilehash: ab2f5be77f6480b4a8b47bef0e0fd5096f7c1776
ms.sourcegitcommit: a7897284b79abb1ceeee79deb3a87b72d59900dc
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "102029913"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Controleer of de klant de Microsoft-klantovereenkomst heeft geaccepteerd


**Juiste rollen**

- Beheer agent
- Verkoop agent

> [!NOTE]
> De bron van de overeenkomst wordt momenteel alleen ondersteund door het partner centrum in de open bare cloud van micro soft. Het is niet van toepassing op:
> * Partner centrum beheerd door 21Vianet
> * Partnercentrum voor Microsoft Cloud Duitsland
> * Partnercentrum voor Microsoft Cloud for US Government


Als partner moet u de acceptatie van de klant van micro soft verkrijgen voordat u micro soft-producten en-services voor die klant kunt best Ellen. Om ervoor te zorgen dat partners voldoen aan nalevings vereisten, vraagt micro soft partners om acceptatie te bevestigen door de volgende gegevens te verstrekken over degene die de overeenkomst heeft geaccepteerd:

- Voornaam

- Achternaam

- E-mailadres

- Telefoon nummer (optioneel)

- Datum van acceptatie

Directe factuur partners en indirecte providers moeten acceptatie van klant bevestigen van de klant overeenkomst van micro soft bij het handelen via partner Center of partner Center-API. Bevestiging is *verplicht*.

>[!NOTE]
>Vanaf 31 januari 2020 moeten alle klanten, bestaande en nieuwe, de nieuwe micro soft-klant overeenkomst ondertekenen. Lees voor meer informatie [klant acceptatie bevestigen van de micro soft-klant overeenkomst](confirm-customer-agreement.md).

Als er geen bevestiging is opgegeven voor een bepaalde klant:

- U kunt geen nieuwe orders maken voor deze klant.

- U kunt het aantal licenties van bestaande abonnementen op licenties voor deze klant niet wijzigen.

Bevestiging van acceptatie van klanten kan worden gedaan via partner centrum of de Partner Center-API. Zie de volgende onderwerpen voor meer informatie over de Partner Center-API:

- [Bevestiging van toestemming van de klant verkrijgen](/partner-center/develop/get-confirmation-of-customer-consent)

- [Meta gegevens van de overeenkomst ophalen](/partner-center/develop/get-agreement-metadata)

- [Toestemming van de klant bevestigen](/partner-center/develop/confirm-customer-consent)

Dit geldt voor productie-en sandbox-omgevingen.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Acceptatie van klant bevestigen voor een nieuwe klant

Gebruik de volgende procedure om de acceptatie van klanten te bevestigen terwijl u een nieuwe klant Tenant maakt in het partner centrum. U moet een beheer agent of verkoop agent zijn om dit te kunnen doen.

1. Selecteer **klanten** en vervolgens **nieuwe klant** en selecteer vervolgens **account gegevens**.

2. Voer de gegevens in van het **bedrijf** en de **primaire contact persoon**.

   :::image type="content" source="images/mca/mca1.png" alt-text="Bedrijfs gegevens":::

3. Onder **micro soft-klant overeenkomst** selecteert u dat de **klant de nieuwste micro soft-klant overeenkomst heeft geaccepteerd**.

4. Voer bij **acceptatie datum** van de overeenkomst de juiste datum in. U kunt dit niet instellen op een datum in de toekomst.

5. Voer de details in van de gebruiker die de acceptatie heeft opgegeven.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Acceptatie datum toevoegen":::

   Standaard worden de gegevens van de primaire contact persoon weer gegeven. Als dat niet het geval is, selecteert u **bijwerken** en voert u vervolgens de **voor naam**, **Achternaam**, **e-mail adres** en het **telefoon nummer* (optioneel) in van de persoon die de overeenkomst heeft geaccepteerd.

6. Selecteer **volgende** om door te gaan met de resterende stappen voor het maken van de Tenant van de klant.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Acceptatie van klant bevestigen voor een bestaande klant

U moet een beheer agent of verkoop agent zijn om dit te kunnen doen.

1. Selecteer **klanten** en zoek en selecteer de klant die u wilt zien.

2. Selecteer **account gegevens**.

3. Selecteer in de **micro soft-klant overeenkomst** **Update**.

   :::image type="content" source="images/mca/mca4.png" alt-text="Bijwerken":::

4. Voer de **voor naam**, **Achternaam**, het **e-mail adres** en het **telefoon nummer** (optioneel) in van de gebruiker die de overeenkomst heeft geaccepteerd.

5. Voer bij **acceptatie datum** van de overeenkomst de juiste datum in. U kunt dit niet instellen op een datum in de toekomst.

6. Selecteer **Opslaan en doorgaan**.

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Acceptatie van klant bevestigen bij het maken van een nieuwe order voor een bestaande klant

Als u probeert een nieuwe bestelling te maken voor een bestaande klant die u nog niet eerder hebt bevestigd, ontvangt u een prompt om de bevestiging te volt ooien. Gebruik de volgende procedure om dit te doen.

1. Voer de **voor naam**, **Achternaam**, het **e-mail adres** en het **telefoon nummer** (optioneel) in van de gebruiker die de overeenkomst heeft geaccepteerd.

2. Voer bij **acceptatie datum** van de overeenkomst de juiste datum in. U kunt dit niet instellen op een datum in de toekomst.

3. Selecteer **Opslaan en doorgaan**.

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Bevestiging van acceptatie van klant voor een bestaande klant ophalen

U kunt de bevestiging van acceptatie van klanten ophalen voor een bestaande klant die u eerder hebt gegeven met behulp van de onderstaande procedure. U moet een beheer agent of verkoop agent zijn om dit te kunnen doen.

1. Selecteer **klanten** en zoek en selecteer de klant die u wilt zien.

2. Selecteer **account gegevens**.

3. Onder **micro soft-klant overeenkomst** ziet u of er al dan niet een bevestiging voor deze klant is ontvangen.

## <a name="next-steps"></a>Volgende stappen

- [Acceptatie van klant bevestigen van de micro soft-klant overeenkomst in het CSP-partner programma](confirm-customer-agreement.md)

- [Verklaring van de micro soft-klant overeenkomst namens uw klant aanvaar ding](attest-acceptance-customer-agreement.md)
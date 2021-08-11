---
title: Het aantal desktops en het kostenniveau zoeken
ms.topic: how-to
ms.date: 02/18/2021
description: Meer informatie over het gebruik van het Channel Incentives Platform (CHIP) om informatie over het aantal desktops en het kostenniveau voor een overeenkomst te vinden.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: c2ae28bd6291af9c4a4445dcc4010b817e533c34b339b137b67ae1a99b5f4e2c
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115692760"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Het aantal desktop en kostenniveaus voor een overeenkomst zoeken

**Juiste rollen:** primaire contactpersoon of programmabeheerder

U kunt zich aanmelden bij [explore.ms](https://www.explore.ms/) de overeenkomst te controleren of een bestand downloaden met details van de overeenkomst voor het aantal desktops en het kostenniveau.

## <a name="to-locate-the-information"></a>De informatie zoeken

### <a name="method-1--explorems"></a>Methode 1: Explore.ms

1. Open [explore.ms](https://www.explore.ms/) in Internet Explorer. 

>[!Note]
>U kunt deze functie niet uitvoeren in Google Chrome of Microsoft Edge.

2. Meld u aan met uw werk-/schoolaccount of live-id.  

3. Selecteer overeenkomsten **in** het veld **Rapporten.**

4. Voer op de resulterende pagina het overeenkomstnummer in het **veld Zoeken** in en selecteer **vervolgens Select/Order Columns.**

5. Selecteer in het pop-upvenster **Agreement Desktop Count** in de lijst met beschikbare kolommen en selecteer vervolgens de pijl-rechts om de kolom toe te voegen. Selecteer **OK**.

6. Selecteer **Zoeken.**

7. Blader in het resulterende scherm door de resultaten om de kolom Aantal bureaubladen **overeenkomst te** vinden. 

8. Gebruik het aantal bureaubladen om het tariefniveau te bepalen op basis van de onderstaande tarieftabel.  

| Kostenniveau | Aantal bureaubladen |
| ------ | :-----------: |
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>Enterprise Incentive-niveaus zijn gebaseerd op het bureaublad of het aantal gebruikers (afhankelijk van wat hoger is) in PS-inschrijvingen (Commercial and Public Sector). Voor inschrijvingen zonder natuurlijk gekoppeld desktop- of gebruikerstelling past Microsoft het aantal desktops toe op basis van het aantal desktops of het aantal gebruikers van de bijbehorende EA. <br><br>Als er geen ea bij de hand is, is het tariefniveau gebaseerd op het prijsniveau van de inschrijving. Het prijsniveau van de deal kan ook worden bekeken op [www.explore.ms](https://www.explore.ms/). <br><br>Als er meerdere pool- en/of prijsniveaus op de bestaande EA/EAS zijn, betaalt Microsoft incentives op het hoogste toegewezen prijs-/poolniveau, met niveau A het laagste niveau en niveau D de hoogste.

#### <a name="pool-and-pricing-levels"></a>Pool- en prijsniveaus

Nadat u in de bovenstaande stappen naar het overeenkomstnummer explore.ms, selecteert u het overeenkomstnummer. Hiermee gaat u naar de pagina met details van de overeenkomst, waar het overeenkomstoverzicht **en** de **aanbiedingen worden weergegeven.** De sectie aanbiedingen bevat de prijsniveaus.

## <a name="method-2---chip"></a>Methode 2 - CHIP

1. Meld u aan bij CHIP en selecteer LSP Incentives.

2. Selecteer op **de pagina Betalingsoverzicht** partner de rapportagemaand die  u wilt weergeven en selecteer vervolgens Berekeningsdetails in de vervolgkeuzepagina onder Exporteren **naar Excel:**

:::image type="content" source="images/chip/chiplocate.png" alt-text="Zoek programmadetails.":::

3. De export wordt start en u kunt het bestand openen of opslaan/opslaan als op een bestemming.

4. Wanneer het rapport is geopend, gaat u naar **het tabblad DetailReport-FlatFile** linksonder:

:::image type="content" source="images/chip/flatfile.png" alt-text="Downloaden van plat bestand.":::

U kunt nu zoeken naar het overeenkomstnummer dat u zoekt in kolom J. En u vindt het toegewezen aantal bureaubladen in kolom R, met het Agreement_DesktopCount. U kunt ook het tariefniveau voor deze overeenkomst bevestigen in de kolom AI met het label Laag.

## <a name="next-steps"></a>Volgende stappen

- [Problemen met CHIP-toegang oplossen](chip-access-trouble.md)

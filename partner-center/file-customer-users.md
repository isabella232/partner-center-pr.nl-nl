---
title: Velden voor CSV-bestand voor het importeren van meerdere gebruikers voor een klant account
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Als u meerdere gebruikers aan een klant account wilt toevoegen, maakt u een bestand met door komma's gescheiden waarden (. CSV) met de juiste velden.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441418"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Meerdere gebruikers toevoegen aan een klant account door een CSV-bestand te maken

**Juiste rollen**

- Globale beheerder

Voeg meerdere gebruikers tegelijk aan het account van een klant toe door een gegevens bestand in de bestands indeling met door komma's gescheiden waarden (. CSV) naar het partner centrum te uploaden. U kunt een voorbeeld gegevensbestand downloaden van het partner centrum en het vervolgens bewerken voor uw gebruik. u kunt ook een nieuw gegevens bestand maken met behulp van het hieronder gedefinieerde gegevens model.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Vereisten voor het gegevens bestand

Als u meerdere gebruikers wilt toevoegen aan het account van een klant met behulp van het bulk upload proces, moet u aan de volgende vereisten voldoen:

- U moet globale beheerders machtigingen hebben voor het klant account;
- Elke gebruiker moet een uniek e-mail adres hebben dat is toegevoegd aan de e-mail domein (en) van de klant.
- U kunt Maxi maal 100 records tegelijk uploaden. Als u meer dan 100 gebruikers wilt toevoegen, maakt en uploadt u extra gegevens bestanden.
- Alle gebruikers moeten zich op dezelfde geografische **locatie** bestaan.
- Voer alleen de gegevens in die hieronder worden beschreven. Externe gegevens zorgen ervoor dat het uploaden mislukt.

Voer de volgende gegevens in het gegevens bestand in:

| **Kolomnaam** | **Beschrijving**  | **Beperking**  |
|:-------- |:------  |:----- |
| Voornaam  | De voor naam van de gebruiker (optioneel veld)  | 50-teken limiet  |
| Achternaam  | De achternaam van de gebruiker (optioneel veld)  | 50-teken limiet  |
| Weergavenaam    | De naam die wordt weer gegeven in het partner centrum (vereist veld)                            | 50-teken limiet                         |
| E-mail   | Zakelijke e-mail adres van gebruiker bij bedrijf van klant (vereist veld)           | Elke gebruiker moet een uniek e-mail adres hebben |
| Status update   | Wordt gebruikt om aan te geven of de nieuwe gebruikers record is gemaakt | \*\*Leeg laten\*\*                        |

## <a name="next-steps"></a>Volgende stappen

- [Meerdere gebruikers toevoegen aan een klant](adding-multiple-users-to-a-customer-account.md)
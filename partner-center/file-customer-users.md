---
title: Velden voor .csv voor het importeren van meerdere gebruikers voor een klantaccount
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Als u meerdere gebruikers wilt toevoegen aan een klantaccount, maakt u een bestand met door komma's gescheiden waarden (.csv) met de juiste velden.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d8cbeecf081dc82448625daeedc0ce21b31174e
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126245014"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Meerdere gebruikers toevoegen aan een klantaccount door een .csv maken

**Juiste rollen:** globale beheerder

Voeg meerdere gebruikers tegelijk toe aan het account van een klant door een gegevensbestand in de bestandsindeling met door komma's gescheiden waarden (.csv) te uploaden naar de Partner Center. U kunt een voorbeeldgegevensbestand downloaden van de Partner Center en het vervolgens bewerken voor uw gebruik, of u kunt een nieuw gegevensbestand maken met behulp van het gegevensmodel dat hieronder is gedefinieerd.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Vereisten voor gegevensbestand

Als u meerdere gebruikers wilt toevoegen aan het account van een klant met behulp van het proces voor bulksgewijs uploaden, moet u voldoen aan de volgende vereisten:

- U moet globale beheerdersmachtigingen hebben voor het klantaccount;
- Elke gebruiker moet een uniek e-mailadres hebben dat is toegevoegd aan het e-maildomein(en) van de klant;
- U kunt maximaal 100 records tegelijk uploaden. Als u meer dan 100 gebruikers wilt toevoegen, maakt en uploadt u aanvullende gegevensbestanden.
- Alle gebruikers moeten zich op dezelfde geografische **locatie bevinden.**
- Voer alleen de gegevens in die hieronder worden beschreven. Overbodige gegevens zorgen ervoor dat het uploaden mislukt.

Voer de volgende gegevens in het gegevensbestand in:

| **Kolomnaam** | **Beschrijving**  | **Beperking**  |
|:-------- |:------  |:----- |
| Voornaam  | Voornaam van gebruiker (optioneel veld)  | Limiet van 50 tekens  |
| Achternaam  | Achternaam van gebruiker (optioneel veld)  | Limiet van 50 tekens  |
| Weergavenaam    | Naam weergegeven in de Partner Center (vereist veld)                            | Limiet van 50 tekens                         |
| E-mail   | Het zakelijke e-mailadres van de gebruiker bij het klantbedrijf (vereist veld)           | Elke gebruiker moet een uniek e-mailadres hebben |
| Statusupdate   | Wordt gebruikt om aan te geven of de nieuwe gebruikersrecord is gemaakt | \*\*Leeg laten\*\*                        |

## <a name="next-steps"></a>Volgende stappen

- [Meerdere gebruikers toevoegen voor een klant](adding-multiple-users-to-a-customer-account.md)
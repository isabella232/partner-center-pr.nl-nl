---
title: Velden voor CSV-bestand voor het importeren van meerdere gebruikers voor een klantaccount
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Als u meerdere gebruikers wilt toevoegen aan een klantaccount, maakt u een bestand met door komma's gescheiden waarden (CSV) met de juiste velden.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150978"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a>Meerdere gebruikers toevoegen aan een klantaccount door een CSV-bestand te maken

**Juiste rollen:** globale beheerder

Voeg meerdere gebruikers tegelijk toe aan het account van een klant door een gegevensbestand in de bestandsindeling met door komma's gescheiden waarden (.csv) te uploaden naar de Partner Center. U kunt een voorbeeldgegevensbestand downloaden van de Partner Center en het vervolgens bewerken voor uw gebruik, of u kunt een nieuw gegevensbestand maken met behulp van het gegevensmodel dat hieronder is gedefinieerd.

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a>Vereisten voor gegevensbestand

Als u meerdere gebruikers wilt toevoegen aan het account van een klant met behulp van het proces voor bulksgewijs uploaden, moet u aan de volgende vereisten voldoen:

- U moet globale beheerdersmachtigingen hebben voor het klantaccount;
- Elke gebruiker moet een uniek e-mailadres hebben dat is toegevoegd aan de e-maildomeinen van de klant;
- U kunt maximaal 100 records tegelijk uploaden. Als u meer dan 100 gebruikers wilt toevoegen, maakt en uploadt u aanvullende gegevensbestanden.
- Alle gebruikers moeten zich in dezelfde geografische **locatie bevinden.**
- Voer alleen de gegevens in die hieronder worden beschreven. Overbodige gegevens zorgen ervoor dat het uploaden mislukt.

Voer de volgende gegevens in het gegevensbestand in:

| **Kolomnaam** | **Beschrijving**  | **Beperking**  |
|:-------- |:------  |:----- |
| Voornaam  | Voornaam van gebruiker (optioneel veld)  | Limiet van 50 tekens  |
| Achternaam  | Achternaam van gebruiker (optioneel veld)  | Limiet van 50 tekens  |
| Weergavenaam    | Naam die wordt weergegeven in het Partner Center (vereist veld)                            | Limiet van 50 tekens                         |
| E-mail   | Het zakelijke e-mailadres van de gebruiker bij het klantbedrijf (vereist veld)           | Elke gebruiker moet een uniek e-mailadres hebben |
| Statusupdate   | Wordt gebruikt om aan te geven of de nieuwe gebruikersrecord is gemaakt | \*\*Leeg laten\*\*                        |

## <a name="next-steps"></a>Volgende stappen

- [Meerdere gebruikers toevoegen voor een klant](adding-multiple-users-to-a-customer-account.md)
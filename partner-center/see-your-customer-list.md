---
title: Uw klantenlijst beheren
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Klantrecords zijn een van de belangrijkste informatieactiva. Meer informatie over het weergeven, zoeken, bijwerken & exporteren van gegevens in Partner Center lijst met klanten.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1791d415d0004520e8c7dc950decf540c91cf003
ms.sourcegitcommit: 26e6b470756aa9c1b3b0b919301b0eb38a335a52
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/26/2021
ms.locfileid: "108002838"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Uw klantenlijst beheren : klanten zoeken, bijwerken of exporteren in Partner Center

**Van toepassing op**

- Partnercentrum voor Microsoft Cloud for US Government

**Juiste rollen**

- Beheeragent
- Globale beheerder

Klantrecords zijn een van uw belangrijkste informatieactiva in Partner Center. U kunt uw database met klantaccounts doorzoeken, de hele klantdatabase exporteren of een subset exporteren naar een excel-compatibele bestandsindeling met door komma's gescheiden waarden (.csv). U kunt ook de abonnementsgegevens van een klant exporteren naar een CSV-bestand.

Activiteitenlogboeken bieden ook exporteerbare gegevens over transacties en beheeracties voor klanten. Zie Activiteitenlogboeken van [klanten weergeven voor meer informatie.](activity-logs.md)

## <a name="search-for-a-customer"></a>Een klant zoeken

1. Selecteer klanten **Partner Center** het menu **.**
2. Als u wilt zoeken naar een klant, voert u de naam of domeinnaam van de klant in het zoekvak in.
3. Selecteer de **pijl-omlaag** aan het einde van een klantrij om de Microsoft-id en de bijbehorende snelle koppelingen voor abonnementen en services te bekijken.

## <a name="update-a-customers-company-name"></a>De bedrijfsnaam van een klant bijwerken

Selecteer klanten **Partner Center** het menu **.**
2. Als u wilt zoeken naar een klant, voert u de naam of domeinnaam van de klant in het zoekvak in.
3. Selecteer de **pijl-omlaag** aan het einde van een klantrij om de Microsoft-id en de bijbehorende snelle koppelingen voor abonnementen en services te bekijken.
4. Werk onder Factuurgegevens **van de** klant de bedrijfsnaam bij. Wanneer u de nieuwe waarde op slaan, wordt deze weergegeven in de lijst met klanten. Hierdoor worden alleen de factuurnaam en de waarde van de klantlijst gewijzigd. Deze wordt nergens anders weergegeven.

## <a name="export-your-customer-list"></a>Uw klantenlijst exporteren

1. Selecteer in **Partner Center** menu **Klanten.**
2. Selecteer **Klanten exporteren.**

   Partner Center converteert uw volledige klantenlijst naar een CSV-bestand en uploadt dit naar de standaard downloadmap op uw computer. U kunt ook subsets van klantgegevens exporteren. Gegevenskolommen zijn onder andere:

   - **Microsoft-id;**
   - **Bedrijfsnaam**;
   - **Primaire domeinnaam;**
   - **Relatie:** de zakelijke relatie van de partner met elke vermelde klant.

    Standaard exporteert Partner Center de volledige klantenlijst, ongeacht de lengte. U kunt ook zoeken in de lijst met klanten op bedrijfsnaam of -domein en die subset met gegevens exporteren.

3. Als u een indirecte provider bent, kunt u uw klantenlijst filteren op indirecte reseller. Selecteer **Filteren op indirecte reseller** in de lijst en kies vervolgens een reseller.


## <a name="export-customer-subscription-information"></a>Abonnementsgegevens van klanten exporteren

1. Selecteer in **Partner Center** menu **Klanten.**

2. Selecteer de **bedrijfsnaam** voor elke klant. De pagina Abonnementen **van de klant wordt** geopend, met de volledige lijst met productabonnementen.

3. Selecteer **Abonnementen exporteren.** Partner Center converteert de abonnementsgegevens van de klant naar een CSV-bestand en uploadt deze naar de standaard downloadmap op uw computer. Gegevenskolommen zijn onder andere:
   - **Abonnements-id**;
   - **Abonnement:** de productnaam voor het abonnement;
   - **Hoeveelheid:** aantal aangeschafte licenties;
   - **Status**;
   - **Reseller:** de id van de reseller die eigenaar is van en het abonnement beheert.

> [!NOTE]  
> Zie Klantabonnementen voor meer informatie [over abonnementsbeheer.](customer-subscriptions.md)

---
title: Uw klantenlijst beheren
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Klant records zijn een van de belangrijkste informatie-assets. Meer informatie over het weer geven, zoeken, bijwerken & en exporteren van gegevens in de klanten lijst van uw partner centrum.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 244a8cfc661b371b611a19a5c90ddf131b42a46a
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441962"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Uw klanten lijst beheren-klanten zoeken, bijwerken of exporteren in het partner centrum

**Van toepassing op**

- Partnercentrum voor Microsoft Cloud for US Government

Klant records zijn van uw belangrijkste informatie-assets in Partner Center. U kunt zoeken in uw data base met klant accounts, de hele klanten database exporteren of een subset exporteren naar een met Excel compatibele bestands indeling met door komma's gescheiden waarden (. CSV). U kunt ook de abonnements gegevens van een klant exporteren naar een CSV-bestand.

Activiteiten logboeken bieden ook Exporteer bare gegevens over trans acties en beheer acties voor klanten. Zie [activiteiten logboeken voor klanten weer geven](activity-logs.md)voor meer informatie.

## <a name="search-for-a-customer"></a>Zoeken naar een klant

1. Selecteer in het menu **Partner Center** **klanten**.
2. Als u een klant wilt zoeken, voert u de naam van de klant of de domein naam in het zoekvak in.
3. Selecteer de **pijl-omlaag** aan het einde van de rij van de klant om de micro soft-id en de bijbehorende abonnementen en services snelle koppelingen te bekijken.

## <a name="update-a-customers-company-name"></a>De bedrijfs naam van een klant bijwerken

Selecteer in het menu **Partner Center** **klanten**.
2. Als u een klant wilt zoeken, voert u de naam van de klant of de domein naam in het zoekvak in.
3. Selecteer de **pijl-omlaag** aan het einde van de rij van de klant om de micro soft-id en de bijbehorende abonnementen en services snelle koppelingen te bekijken.
4. Werk de naam van het bedrijf bij aan de **factuur** informatie van de klant. Wanneer u de nieuwe waarde opslaat, wordt deze weer gegeven in de klanten lijst. Hierdoor worden alleen de naam van het factuur bedrijf en de waarde van de klanten lijst gewijzigd. Het wordt nergens anders weer gegeven.

## <a name="export-your-customer-list"></a>Uw klanten lijst exporteren

1. Selecteer in het menu **Partner Center** **klanten**.
2. Selecteer **klanten exporteren**.

   Het partner centrum zet uw volledige klanten lijst om in een CSV-bestand en uploadt deze naar de standaard downloadmap op uw computer. U kunt ook subsets van klant gegevens exporteren. Gegevens kolommen bevatten het volgende:

   - **Micro soft-id**;
   - **Bedrijfs naam**;
   - **Primaire domein naam**;
   - **Relatie**: de zakelijke relatie van de partner met elke vermelde klant.

    Standaard exporteert het partner centrum de volledige klanten lijst, ongeacht de lengte. U kunt ook de klanten lijst op bedrijfs naam of domein doorzoeken en die subset met gegevens exporteren.

3. Als u een indirecte provider bent, kunt u uw klanten lijst filteren op een indirecte wederverkoper. Selecteer **filteren op indirecte reseller** in de lijst en kies vervolgens een wederverkoper.


## <a name="export-customer-subscription-information"></a>Abonnements gegevens van de klant exporteren

1. Selecteer in het menu **Partner Center** **klanten**.

2. Selecteer de **Bedrijfs naam** voor elke klant. De pagina **abonnementen** van de klant wordt geopend, waarin de volledige lijst met product abonnementen wordt weer gegeven.

3. Selecteer **abonnementen exporteren**. Het partner centrum converteert de abonnements gegevens van de klant naar een CSV-bestand en uploadt deze naar de standaard downloadmap op uw computer. Gegevens kolommen bevatten het volgende:
   - **Abonnements-id**;
   - **Abonnement**: de product naam voor het abonnement;
   - **Aantal**: aantal aangeschafte licenties;
   - **Status**;
   - **Wederverkoper**: de id van de wederverkoper die eigenaar is van het abonnement en deze beheert.

> [!NOTE]  
> Zie [klant abonnementen](customer-subscriptions.md)voor meer informatie over het beheer van abonnementen.

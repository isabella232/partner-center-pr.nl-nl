---
title: Abonnementen migreren naar nieuwe handel
ms.topic: article
ms.date: 10/04/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over nieuwe commerce-ervaringen voor het migreren van abonnementen.
author: iragulati1
ms.author: iragulati
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bad50c36cd0e0523fe70115e0b39d88e0e68ab68
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/05/2021
ms.locfileid: "129454664"
---
# <a name="introduction-migrate-subscriptions-to-new-commerce"></a>Inleiding: Abonnementen migreren naar New Commerce

**Juiste rollen:** beheeragent | Verkoopagent | Globale beheerder

> [!NOTE]
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technische preview van Microsoft 365/Dynamics 365 New Commerce Experience.
Partners kunnen abonnementen migreren naar New Commerce als het abonnement voldoet aan geschiktheidscriteria en er een beschikbaar is zoals de aanbieding.

## <a name="ineligible-subscriptions"></a>Niet-in aanmerking komende abonnementen ##

Niet alle abonnementen komen op dit moment in aanmerking voor migratie. De volgende categorieën abonnementen komen momenteel niet in aanmerking: 

- Inactieve abonnementen (er treden geen wijzigingen in de service op als een abonnement inactief is) 

- Proefabonnementen (geen financieel voordeel of implicaties; de verwachting is dat proefversies hun cursus kunnen uitvoeren in Verouderd) 

- Abonnementen met promoties (promoties in TIJDENS zijn onafhankelijk van die promoties in verouderde) 

- Abonnementen met invoegtoepassingen (het migreren van abonnementen met invoegtoepassingen wordt later ingeschakeld; op dit moment kunnen we geen coterminous migratie ondersteunen) 

- Abonnementen voor Gov-, Edu- of Non-profitorganisaties (de toewijzing van gekwalificeerde aanbiedingen van Verouderd naar GEBRUIK wordt niet ondersteund) 

- Afgeschafte of afgeschafte abonnementen (voor deze abonnementen is er geen aanbieding zoals bestaande in New Commerce) 

Migraties van de bovenstaande abonnementen vallen op dit moment buiten het bereik van deze functie. Daarnaast is één abonnement de migratie-eenheid in plaats van batches abonnementen. 

## <a name="suspending-a-legacy-subscription-during-migration"></a>Een verouderd abonnement opschorten tijdens de migratie ##

Een verouderd abonnement wordt alleen tijdelijk opgeschort zodra een geslaagd pad naar New Commerce is ingericht voor het abonnement. Deze mogelijkheid voorkomt verlies van service als er sprake is van blokkeringen na een partner die de migratie van een abonnement start. Bovendien wordt er geen dubbele facturering uitgevoerd voor zowel het verouderde als het nieuwe commerce-abonnement. Zodra de migratie is gestart, wordt de facturering voor het verouderde abonnement gestopt om te voorkomen dat er overlap is met de facturering voor het FACTURATIE-abonnement.

## <a name="billing-term-and-frequency"></a>Factureringsperiode en -frequentie ##

De factureringsperiode en factureringsfrequentie voor het gemigreerde abonnement blijven hetzelfde als de factureringsperiode en factureringsfrequentie voor het verouderde abonnement; einddatum van de periode blijft hetzelfde.

## <a name="new-commerce-promotions"></a>Nieuwe commerce-promoties ##

Abonnementen in verouderde abonnementen met promoties komen niet in aanmerking voor migratie. Gemigreerde abonnementen komen mogelijk in aanmerking voor Introductiepromoties voor New Commerce. Promoties worden pro rated naar de rest van de abonnementsperiode op het moment van migratie. 

## <a name="cancelling-subscriptions-or-decreasing-licenses"></a>Abonnementen annuleren of licenties verlagen ##

Na de migratie is er een annuleringsvenster van 72 uur. In deze 72 uur kunnen partners het abonnement annuleren of het aantal licenties in dit venster verlagen. Op het tijdstip van 24 uur sinds de migratie is voltooid, worden annuleringen van het abonnement of van licenties pro 1 dag na gebruik pro 1. op het 48-uurs tijdstip sinds de migratie is voltooid, worden annuleringen van het abonnement of van licenties naar meer dan twee dagen van gebruik pro rated. 

## <a name="migration-history"></a>Migratiegeschiedenis ##

Via de API's zijn details over de migratiegeschiedenis, zoals de begin- en voltooiingsvoorwaarden van de migratie, toegankelijk via het nieuwe veld GetMigration API en MigrationID. Op de UX wordt de abonnements-id van waaruit het nieuwe RIJ-abonnement is gemigreerd, weergegeven boven aan de detailpagina. Deze wordt weergegeven wanneer u op het regelitem Abonnement op de pagina Abonnementen van de klant klikt. 

## <a name="apis"></a>API's ##

Voor de migratie van like-to-like-abonnementen worden er drie nieuwe REST API's uitgebracht. De eerste CheckMigration-API controleert of de migratie in aanmerking komt voor een abonnement. De tweede CreateMigration-API maakt de migratie als het abonnement in aanmerking komt. Ten laatste kunnen partners met de derde GetMigration-API de migratiestatus controleren. 

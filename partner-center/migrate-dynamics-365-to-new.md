---
title: Dynamics 365 Business Edition migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het migreren van gekwalificeerde Dynamics 365 Business Edition-aanbiedingen naar nieuwere versies voordat ze verlopen.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e83c06c11638bdde508fd27904038bcb6d8c9e9c
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132635"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrate Dynamics 365 Business Edition Offers to newer versions (Aanbiedingen van Dynamics 365 Business Edition migreren naar nieuwere versies)

**Juiste rollen**

- Globale beheerder
- Beheerder van gebruikers beheer
- Beheer agent
- Verkoop agent

Met ingang van 1 januari 2019 kunnen klanten met Dynamics 365 Business Edition-abonnementen niet langer worden verlengd naar deze verouderde aanbiedingen. bestaande abonnementen worden niet automatisch vernieuwd wanneer ze verlopen. Op de detail pagina van het abonnement wordt de abonnements status gewijzigd van ' verloopt op [datum] ' van ' automatisch relateren op [date] '.

Om klanten continuïteit te garanderen, moet u deze met verlopende abonnementen overzetten naar een ondersteunde optie die hieronder wordt weer gegeven. U wordt aangeraden klanten te verplaatsen naar nieuwe abonnementen vóór de jaarlijkse eind datum van het abonnement om eventuele service storingen voor klanten te voor komen.

Als u de API (topof het partner centrum) gebruikt, kunt u verlopen abonnementen vinden door de eind datum van het abonnement samen met de eigenschap automatisch verlengen = false te evalueren. De betreffende abonnementen worden ingesteld op automatisch verlengen = False op 1 januari 2019. U kunt klanten op elk gewenst moment verplaatsen naar een nieuw abonnement. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>De Dynamics 365 Business-edities buiten gebruik gesteld

- Dynamics 365 voor Financiën en operationele activiteiten, Business Edition
- Dynamics 365 for Team Members, Business edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics business Central-de Dynamics 365 Business Edition nieuwe aanbiedingen

Met de nieuwe aanbiedingen voor Dynamics business Central kunnen uw klanten hun financiën, verkoop, service en activiteiten verbinden om bedrijfs processen te stroom lijnen, interacties van klanten te verbeteren en betere beslissingen te nemen. Dynamics 365 Business Central is alleen beschikbaar via Cloud Solution Provider (CSP)-programma partners.
Dynamics 365 Business Edition-klanten komen in aanmerking voor korting op prijzen voor de nieuwe Business Central-aanbiedingen tot en met 30 juni 2020.

## <a name="transition-customers-to-new-product-plans"></a>Klanten overstappen naar nieuwe product abonnementen

 Voor het verplaatsen van klanten uit buiten gebruik gestelde Sku's naar nieuwere versies moeten de volgende stappen worden uitgevoerd in deze volg orde:

- Het nieuwe abonnement kopen
- Huidige gebruikers licenties opnieuw toewijzen
- Oud abonnement annuleren

## <a name="purchase-the-new-plan-for-your-customer"></a>Koop het nieuwe abonnement voor uw klant

1. Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u naar het nieuwe abonnement wilt verplaatsen.
2. Selecteer **abonnement toevoegen**.
3. Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer vervolgens **verzenden**. 

Uw klant heeft nu zowel het oude als het nieuwe abonnement. De volgende stap is het opnieuw toewijzen van licenties aan de gebruikers van de klant.

1. Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.
2. Selecteer **gebruikers en licenties**.
3. Als u een licentie wilt toewijzen aan een gebruiker, selecteert u de gebruiker en selecteert u vervolgens **licenties beheren**. 
4. Schakel op de pagina **licenties beheren** het selectie vakje Dynamics 365 voor verkoop/klant engagement van de Basic-licentie (gekwalificeerd aanbod) uit en selecteer een nieuw service plan voor het abonnement waarnaar de klant wordt verplaatst. 
5. Selecteer **Indienen**. U kunt dit doen voor elke gebruiker die de nieuwe licentie nodig heeft. 

Zodra u de licenties hebt verplaatst naar het nieuwe abonnement, kunt u het oude abonnement annuleren. 

1. Selecteer **klanten** in het linkerdeel venster en selecteer vervolgens de klant die u wilt verplaatsen.
2. Stel op de pagina abonnements Details het oude abonnement in op **opgeschort** en selecteer **indienen**.

Het oude abonnement is nu onderbroken en het nieuwe abonnement is actief. Het opgeschorte abonnement wordt na 120 dagen niet meer ingericht. Uw klant heeft geen extra kosten in rekening gebracht voor het oude abonnement.

---
title: Gekwalificeerde Dynamics 365-abonnementen migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe u migreert van gekwalificeerd, Basic Dynamics 365-abonnementen naar een nieuw abonnement voordat bestaande abonnementen verlopen.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 363c97b8c2b62e8d6b62cbe3b2807fb3c0ef3e38
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132737"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions (Abonnement van Dynamics 365 en Customer Engagement (gekwalificeerde aanbiedingen) migreren van Basic naar nieuwere versies)

**Juiste rollen**

- Globale beheerder
- Beheerder van gebruikers beheer
- Beheer agent
- Verkoop agent

Met ingang van 1 januari 2019 kunnen deze verouderde aanbiedingen niet langer worden vernieuwd door klanten met Dynamics 365 voor verkoop-en klant betrokkenheid van basis abonnementen. bestaande abonnementen worden niet automatisch vernieuwd wanneer ze verlopen. Op de detail pagina van het abonnement wordt de abonnements status gewijzigd van ' verloopt op [datum] ' van ' automatisch relateren op [date] '. 

Om klanten continuïteit te garanderen, moet u deze met verlopende abonnementen overzetten naar een ondersteunde optie die hieronder wordt weer gegeven. U wordt aangeraden klanten te verplaatsen naar nieuwe abonnementen vóór de jaarlijkse eind datum van het abonnement om eventuele service storingen voor klanten te voor komen.

Als u de API (topof het partner centrum) gebruikt, kunt u verlopen abonnementen vinden door de eind datum van het abonnement samen met de eigenschap automatisch verlengen = false te evalueren. De betreffende abonnementen worden ingesteld op automatisch verlengen = False op 1 januari 2019. U kunt klanten op elk gewenst moment verplaatsen naar een nieuw abonnement. 

### <a name="the-dynamics-365-offers-being-retired"></a>De Dynamics 365-aanbiedingen die buiten gebruik worden gesteld

- Dynamics 365 for Sales, Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding)
- Dynamics 365 for Sales, Enter prise Edition CRMOL Basic (gekwalificeerd aanbod) voor faculteiten
- Dynamics 365 for Sales, Enter prise Edition CRMOL Basic (gekwalificeerd aanbod) voor studenten
- Dynamics 365 voor Sales Enter prise Edition (prijzen voor de overheid) CRMOL Basic (gekwalificeerde aanbieding)
- Dynamics 365 voor Sales Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 voor Sales Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding) voor faculteiten
- Dynamics 365 voor Sales Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding) voor studenten
- Dynamics 365 voor Sales Enter prise Edition (overheids prijzen) van SA voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 for Sales Edition Add-On voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 voor Sales Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor faculteiten
- Dynamics 365 voor Sales Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor studenten
- Dynamics 365 voor Sales Enter prise Edition (overheids prijzen) Add-On voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer engagement plan Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer engagement plan Enter prise Edition (overheids prijzen) CRMOL Basic (aanbieding in aanmerking komend)
- Dynamics 365 Customer engagement plan Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding) voor studenten
- Dynamics 365 Customer engagement plan Enter prise Edition CRMOL Basic (gekwalificeerde aanbieding) voor faculteiten
- Dynamics 365 Customer engagement plan Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer engagement plan Enter prise Edition (overheids prijzen) van SA voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer engagement plan Enter prise Edition van SA voor CRM Basic (gekwalificeerde aanbieding) voor studenten
- Dynamics 365 Customer engagement plan Enter prise Edition van SA for CRM Basic (gekwalificeerde aanbieding) voor faculteiten
- Dynamics 365 Customer engagement plan Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer engagement plan Enter prise Edition (overheids prijzen) Add-On voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer engagement plan Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor studenten
- Dynamics 365 Customer engagement plan Enter prise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding) voor faculteiten



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 voor verkoop/klant engagement plan van basis (aanbiedingen)

**Aanbiedingen buiten gebruik gesteld**   

- Dynamics 365 voor verkoop van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer engagement plan van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)

**Vervangende opties**
- Dynamics 365 voor Sales Professional (nieuw)
- Dynamics 365 voor Sales Professional (nieuw)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer engagement-abonnement of
- Dynamics 365-team leden



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
 

 




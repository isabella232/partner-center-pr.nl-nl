---
title: Dynamics 365 Business Edition migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over het migreren van gekwalificeerde Dynamics 365 Business Edition-aanbiedingen naar nieuwere versies voordat ze verlopen.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 40be8c8a338f5bbcbc8a10ccd9343f7ef52817902cdf7a5a54e8631a2d2c8b4b
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681532"
---
# <a name="migrate-dynamics-365-business-edition-offers-to-newer-versions"></a>Migrate Dynamics 365 Business Edition Offers to newer versions (Aanbiedingen van Dynamics 365 Business Edition migreren naar nieuwere versies)

**Juiste rollen:** Globale | Gebruikersbeheerbeheer | Beheeragent | Verkoopagent

Vanaf 1 januari 2019 kunnen klanten met Dynamics 365 Business Edition-abonnementen niet langer worden verlengd voor deze verouderde aanbiedingen; bestaande abonnementen worden niet automatisch vernieuwd wanneer ze verlopen. Op de detailpagina van het abonnement wordt de status van het abonnement gewijzigd in 'Verloopt op [datum]' van 'Automatisch verlengen op [datum]'.

Om de continuïteit voor klanten te waarborgen, moet u de abonnementen met verlopende abonnementen overstappen naar een ondersteunde optie, die hieronder wordt vermeld. Het is raadzaam om klanten vóór de jaarlijkse einddatum van het abonnement over te brengen naar nieuwe abonnementen om service-uitval voor klanten te voorkomen.

Als u de API (ZOWEL VOOR- als Partner Center) gebruikt, kunt u verlopende abonnementen vinden door de einddatum van het abonnement samen met de eigenschap auto renew = False te evalueren. De abonnementen in kwestie worden op 1 januari 2019 ingesteld op auto renew=False. U kunt klanten op elk moment verplaatsen naar een nieuw plan. 

## <a name="the-dynamics-365-business-editions-being-retired"></a>De Dynamics 365 Business Editions wordt niet meer gebruikt

- Dynamics 365 for Finance and Operations, Business Edition
- Dynamics 365 for Team Members, Business edition

## <a name="dynamics-business-central---the-dynamics-365-business-edition-new-offers"></a>Dynamics Business Central: de nieuwe aanbiedingen voor Dynamics 365 Business Edition

Met de nieuwe Dynamics Business Central-aanbiedingen kunnen uw klanten hun financiële gegevens, verkoop, service en activiteiten verbinden om bedrijfsprocessen te stroomlijnen, interacties van klanten te verbeteren en betere beslissingen te nemen. Dynamics 365 Business Central is gebaseerd op de cloud en is alleen beschikbaar via Cloud Solution Provider (CSP)-programmapartners.
Klanten van Dynamics 365 Business Edition kunnen tot en met 30 juni 2020 korting krijgen voor de overgangsprijzen voor de nieuwe Business Central-aanbiedingen.

## <a name="transition-customers-to-new-product-plans"></a>Klanten overstappen op nieuwe productplannen

 Voor het verplaatsen van klanten van niet-bestaande SKU's naar nieuwere SKU's zijn de volgende stappen in deze volgorde vereist:

- Het nieuwe abonnement kopen
- Huidige gebruikerslicenties opnieuw toewijzen
- Oud abonnement annuleren

## <a name="purchase-the-new-plan-for-your-customer"></a>Het nieuwe abonnement voor uw klant kopen

1. Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u wilt verplaatsen naar het nieuwe abonnement.
2. Selecteer **Abonnement toevoegen.**
3. Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer **verzenden.** 

Uw klant heeft nu zowel het oude als het nieuwe abonnement. De volgende stap is het opnieuw toewijzen van licenties aan de gebruikers van de klant.

1. Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u verplaatst.
2. Selecteer **Gebruikers en licenties.**
3. Als u een licentie opnieuw wilt toewijzen aan een gebruiker, selecteert u de gebruiker en selecteert u **vervolgens Licenties beheren.** 
4. Schakel **op** de pagina Licenties beheren het selectievakje Licentie voor Dynamics 365 for Sales/Customer Engagement Plan van Basic (gekwalificeerde aanbieding) uit en selecteer een nieuw serviceplan voor het abonnement waar de klant naar overstapt. 
5. Selecteer **Indienen**. U doet dit voor elke gebruiker die de nieuwe licentie nodig heeft. 

Nadat u de licenties hebt verplaatst naar het nieuwe abonnement, kunt u het oude abonnement annuleren. 

1. Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u verplaatst.
2. Stel op de detailpagina van het abonnement het oude abonnement in op **Tijdelijk en** selecteer **Verzenden.**

Het oude abonnement is nu tijdelijk opgeschort en het nieuwe abonnement is actief. De inrichting van het abonnement wordt na 120 dagen automatisch verwijderd. Uw klant maakt geen extra kosten voor het oude abonnement.

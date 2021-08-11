---
title: Gekwalificeerde Dynamics 365-abonnementen migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Leer hoe u migreert van gekwalificeerde, eenvoudige Dynamics 365-abonnementen naar een nieuw abonnement voordat bestaande abonnementen verlopen.
author: Brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 71c3af5cdb3cb35ff13a455748a93699df43a8b1615116ca7058df3c6a23b7b9
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115694656"
---
# <a name="migrate-dynamics-365-and-customer-engagement-plan-from-basic-qualified-offers-to-newer-versions"></a>Migrate Dynamics 365 and Customer Engagement Plan from Basic (qualified offers) to newer versions (Abonnement van Dynamics 365 en Customer Engagement (gekwalificeerde aanbiedingen) migreren van Basic naar nieuwere versies)

**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Beheeragent | Verkoopagent

Vanaf 1 januari 2019 kunnen klanten met een Dynamics 365 for Sales-/Customer Engagement-abonnement van Basic-abonnementen (gekwalificeerde aanbiedingen) deze verouderde aanbiedingen niet meer vernieuwen; bestaande abonnementen worden niet automatisch vernieuwd wanneer ze verlopen. Op de detailpagina van het abonnement wordt de status van het abonnement gewijzigd in 'Verloopt op [datum]' van 'Automatisch verlengen op [datum]'. 

Om de continuïteit voor klanten te waarborgen, moet u de klanten met verlopen abonnementen overstappen naar een ondersteunde optie, die hieronder wordt vermeld. Het is raadzaam om klanten vóór de jaarlijkse einddatum van het abonnement over te brengen naar nieuwe abonnementen om service-uitval voor klanten te voorkomen.

Als u de API (ZOWEL VOOR als Partner Center) gebruikt, kunt u verlopende abonnementen vinden door de einddatum van het abonnement te evalueren, samen met de eigenschap auto renew = False. De abonnementen in kwestie worden op 1 januari 2019 ingesteld op automatisch verlengen=Onwaar. U kunt klanten op elk moment verplaatsen naar een nieuw abonnement. 

### <a name="the-dynamics-365-offers-being-retired"></a>De Dynamics 365-aanbiedingen worden niet meer gebruikt

- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding)
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding) voor onderwijsmedewerkers
- Dynamics 365 for Sales Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding) voor studenten
- Dynamics 365 for Sales Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer)
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty
- Dynamics 365 for Sales Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students
- Dynamics 365 for Sales Enterprise Edition (government pricing) From SA for CRM Basic (Qualified Offer)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (gekwalificeerde aanbieding) voor onderwijsmedewerkers
- Dynamics 365 for Sales Enterprise Edition Add-On for CRM Basic (gekwalificeerde aanbieding) voor studenten
- Dynamics 365 for Sales Enterprise Edition (government pricing) Add-On for CRM Basic (Qualified Offer)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) CRMOL Basic (Qualified Offer)
- Dynamics 365 Customer Engagement Plan Enterprise Edition CRMOL Basic (Qualified Offer) for Students
- Dynamics 365 Customer Engagement-plan Enterprise Edition CRMOL Basic (gekwalificeerde aanbieding) voor onderwijsmedewerkers
- Dynamics 365 Customer Engagement-Enterprise Edition van SA voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) From SA for CRM Basic (Qualified Offer)
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Students
- Dynamics 365 Customer Engagement Plan Enterprise Edition From SA for CRM Basic (Qualified Offer) for Faculty
- Dynamics 365 Customer Engagement-Enterprise Edition Add-On voor CRM Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer Engagement Plan Enterprise Edition (Government Pricing) Add-On for CRM Basic (Qualified Offer)
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Students
- Dynamics 365 Customer Engagement Plan Enterprise Edition Add-On for CRM Basic (Qualified Offer) for Faculty



## <a name="dynamics-365-for-sales-customer-engagement-plan-from-basic-qualified-offers-replacement-plans"></a>Dynamics 365 for Sales/Customer Engagement Plan from Basic (Qualified Offers) replacement plans (Dynamics 365 for Sales/Customer Engagement Plan van Basic-vervangingsplannen (gekwalificeerde aanbiedingen)

**Gestopte aanbiedingen**   

- Dynamics 365 for Sales van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)
- Dynamics 365 Customer Engagement Plan van CRM Basic of CRMOL Basic (gekwalificeerde aanbieding)

**Vervangingsopties**
- Dynamics 365 for Sales Professional (NIEUW)
- Dynamics 365 for Sales Professional (NIEUW)
- Dynamics 365 for Customer Service
- Dynamics 365 Customer Engagement Plan of
- Dynamics 365-teamleden



## <a name="transition-customers-to-new-product-plans"></a>Klanten overstappen op nieuwe productplannen

Voor het verplaatsen van klanten van niet-bestaande SKU's naar nieuwere SKU's zijn de volgende stappen in deze volgorde vereist:

- Het nieuwe abonnement kopen
- Huidige gebruikerslicenties opnieuw toewijzen
- Oud abonnement annuleren

## <a name="purchase-the-new-plan-for-your-customer"></a>Het nieuwe abonnement voor uw klant kopen

1. Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u wilt verplaatsen naar het nieuwe abonnement.
2. Selecteer **Abonnement toevoegen.**
3. Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer **vervolgens Verzenden.** 

Uw klant heeft nu zowel het oude als het nieuwe abonnement. De volgende stap is het opnieuw toewijzen van licenties aan de gebruikers van de klant.

1. Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u verplaatst.
2. Selecteer **Gebruikers en licenties.**
3. Als u een licentie opnieuw wilt toewijzen aan een gebruiker, selecteert u de gebruiker en selecteert u **vervolgens Licenties beheren.** 
4. Schakel  op de pagina Licenties beheren het selectievakje Licentie voor Dynamics 365 for Sales/Customer Engagement Plan van Basic (gekwalificeerde aanbieding) uit en selecteer een nieuw serviceplan voor het abonnement waar de klant naar overstapt. 
5. Selecteer **Indienen**. U doet dit voor elke gebruiker die de nieuwe licentie nodig heeft. 

Nadat u de licenties hebt verplaatst naar het nieuwe abonnement, kunt u het oude abonnement annuleren. 

1. Selecteer **Klanten** in het linkernavigatiebalk en selecteer vervolgens de klant die u verplaatst.
2. Stel op de detailpagina van het abonnement het oude abonnement in op **Tijdelijk en** selecteer **Verzenden.**

Het oude abonnement is nu opgeschort en het nieuwe abonnement is actief. De inrichting van het abonnement wordt na 120 dagen automatisch verwijderd. Uw klant maakt geen extra kosten voor het oude abonnement.
 

 




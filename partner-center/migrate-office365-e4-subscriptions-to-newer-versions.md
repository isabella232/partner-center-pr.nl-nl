---
title: Office 365 E4-abonnementen migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enter prise E4 Edition wordt vanaf 7 april 2017 buiten gebruik gesteld. Meer informatie over het migreren van uw klanten abonnementen naar nieuwere versies van Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a9662e0ce99fc054149dfbd4149532ce336eff6
ms.sourcegitcommit: f24089cd27b1de6ecf6ddbefb6cbb2d340e144de
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/01/2021
ms.locfileid: "106132618"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrate Office 365 E4 subscriptions to newer Office 365 versions (Abonnementen op Office 365 E4 naar nieuwe versies van Office 365 migreren)

**Juiste rollen**

- Globale beheerder
- Beheerder van gebruikers beheer
- Beheer agent
- Verkoop agent

Het abonnement Office 365 Enter prise E4 wordt buiten gebruik gesteld, vanaf 7 april 2017. U kunt na deze datum geen nieuwe Office 365 E4-abonnementen meer kopen en bestaande E4-abonnementen worden niet automatisch verlengd wanneer ze verlopen.

Wanneer E4-abonnementen eindigen, worden ze geannuleerd. Om ervoor te zorgen dat klanten zich kunnen voordoen, moet u klanten overstappen met het verloop van E4-abonnementen naar een ondersteunde SKU-optie, hieronder weer gegeven. U wordt aangeraden klanten te verplaatsen naar nieuwe abonnementen vóór de jaarlijkse eind datum van het abonnement om eventuele service storingen voor klanten te voor komen. 

> [!NOTE]  
> Zowel Office 365 Enter prise E4 Commercial als Government Sku's worden buiten gebruik gesteld.
 
Op de detail pagina van het abonnement is de status van het E4-abonnement gewijzigd in ' verloopt op [date] ' van ' automatisch relateren op [date] '. 

Als u de API (topof het partner centrum) gebruikt, kunt u verlopen abonnementen detecteren door de eind datum van het abonnement samen met de eigenschap automatisch verlengen = false te evalueren. 

De E4-abonnementen worden ingesteld op automatisch verlengen = False in 7 april 2017. U kunt klanten op elk gewenst moment verplaatsen naar een nieuw abonnement. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Vervangings plannen voor Office 365 Enter prise E4 Edition

U kunt ervoor kiezen om dezelfde functionaliteit te onderhouden met E4, of uw klanten profiteren van nieuwere functies en functionaliteit in Office 365 en Skype voor bedrijven online. Prijs informatie vindt u in de matrix prijs lijst en aanbiedings lijst in partner centrum. Veilig product Enter prise E3 of Secure productief Enter prise E5 kan worden vervangen door respectievelijk de volgende opties voor Office 365 Enter prise E3 of Office 365 Enter prise E5.

- Optie 1: Office 365 Enter prise E5

- Optie 2: Office 365 Enter prise E3 + Skype voor bedrijven cloud PBX

- Optie 3: Office 365 Enter prise E3 + Skype voor bedrijven plus CAL (prijs-en functionaliteits pariteit met E4)

- Optie 4: Office 365 Enter prise E3


| Functie | Optie 1 | Optie 2 | Optie 3 | Optie 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Alle functies uit Office 365 Enter prise E4 ophalen? | Ja | Ja | Ja | Nee |
| Telefoon nummers die worden beheerd in Office 365 | Ja | Ja | Nee | Nee |
| Telefoon nummers die zowel on-premises als in Office 365 (hybride implementatie) worden beheerd | Ja | Ja | Nee | Nee |
| Optie voor het toevoegen van een PSTN-telefoon gespreks plan? | Ja | Ja | Nee | Nee |
| PSTN-vergaderingen? | Ja | Nee | Nee | Nee |
| Geavanceerde hulp middelen voor samen werking, analyses en beveiliging? | Ja | Nee | Nee | Nee |
| Interactieve rapporten, Dash boards en gegevens visualisaties? | Ja | Nee | Nee | Nee | 
| Meer controle over de beveiliging van gegevens en naleving van ingebouwde privacy-, transparantie-en verfijnde gebruikers besturings elementen? | Ja | Nee | Nee | Nee | 

## <a name="transition-customers-to-new-product-plans"></a>Klanten overstappen naar nieuwe product abonnementen

Micro soft biedt voortdurend nieuwe producten en services aan onze partners. In dergelijke gevallen moet u mogelijk klanten upgraden naar nieuwe services of hun abonnementen migreren vanuit Sku's die uiteindelijk worden afgesloten. Voor het migreren van klanten uit buiten gebruik gestelde Sku's naar nieuwere versies moeten de volgende stappen worden uitgevoerd:

-   Het nieuwe abonnement kopen
-   Huidige gebruikers licenties opnieuw toewijzen
-   Het oude abonnement annuleren

Voer de volgende stappen uit om het Office 365 Enter prise E4-abonnement van de klant te migreren naar een van de opties in de bovenstaande tabel.

### <a name="step-1---purchase-the-new-subscription"></a>Stap 1: het nieuwe abonnement kopen

1. Selecteer in het menu **Partner Center** **klanten**, selecteer de klant die u wilt verplaatsen en selecteer vervolgens **abonnementen toevoegen**.

2. Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer vervolgens **verzenden**.

   Uw klant moet nu over zowel oude als nieuwe abonnementen beschikken, het oude Office 365 Enter prise E4-abonnement en het nieuwe ' target '-abonnement, bijvoorbeeld optie 1-Office 365 Enter prise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Stap 2: de gebruikers licenties van de klant opnieuw toewijzen

1. Selecteer in het menu **Partner Center** **klanten**, selecteer de klant die u wilt verplaatsen en selecteer vervolgens **gebruikers en licenties**. De pagina gebruikers en licenties van de klant wordt geopend.

2. Als u gebruikers licenties opnieuw wilt toewijzen, selecteert u de gebruiker die u opnieuw wilt toewijzen en selecteert u vervolgens **licenties beheren**.

3. Schakel op de pagina **licenties beheren** het selectie vakje **Office 365 Enter prise E4** -licentie uit en selecteer een nieuw service plan voor het abonnement waarnaar de klant wordt verplaatst.

4. Selecteer **Indienen**. Een bevestigings pagina bevat een lijst met de nieuwe licentie toewijzingen.

5. Herhaal dezelfde stappen met andere gebruikers van klanten die de licentie opnieuw moeten toewijzen.

Nadat u de gebruikers licenties naar de nieuwe service hebt verplaatst, kunt u het buiten gebruik gestelde abonnement op het hoogste klant niveau gewoon annuleren.

### <a name="step-3---cancel-the-old-subscription"></a>Stap 3: het oude abonnement annuleren

1. Selecteer in het menu **Partner Center** **klanten**. Selecteer de klant die u wilt verplaatsen en selecteer het abonnement dat u wilt annuleren.

2. Stel op de pagina abonnements Details de status van het abonnement in op **opgeschort**.

3. Selecteer **Indienen**.

Het oude abonnement is onderbroken en het nieuwe abonnement is actief. Het opgeschorte abonnement wordt na 120 dagen niet meer ingericht. De klant heeft geen extra kosten in rekening gebracht voor het oude abonnement.



 




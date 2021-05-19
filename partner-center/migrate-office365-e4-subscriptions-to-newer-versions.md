---
title: Office 365 E4-abonnementen migreren
ms.topic: article
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Microsoft Office 365 Enterprise E4-editie is per 7 april 2017 uit gebruik genomen. Meer informatie over het migreren van uw klantabonnementen naar nieuwere versies van Office 365.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f738ddace805838cdf202c23cca8535c11cbdf54
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151556"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrate Office 365 E4 subscriptions to newer Office 365 versions (Abonnementen op Office 365 E4 naar nieuwe versies van Office 365 migreren)

**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Beheeragent | Verkoopagent

Het Office 365 Enterprise E4-abonnement is met ingang van 7 april 2017 ingetrokken. U kunt na deze datum geen nieuwe Office 365 E4-abonnementen meer aanschaffen en bestaande E4-abonnementen worden niet automatisch verlengd wanneer ze verlopen.

Wanneer E4-abonnementen zijn beëindigen, worden ze geannuleerd. Om de continuïteit voor klanten te waarborgen, moet u klanten met verlopen E4-abonnementen overstappen naar een ondersteunde SKU-optie, die hieronder wordt vermeld. Het is raadzaam om klanten vóór de jaarlijkse einddatum van het abonnement over te brengen naar nieuwe abonnementen om service-uitval voor klanten te voorkomen. 

> [!NOTE]  
> Zowel commerciële als overheids-SKU's van Office 365 Enterprise E4 worden niet meer in gebruik genomen.
 
Op de detailpagina van het abonnement is de status van het E4-abonnement gewijzigd in 'Verloopt op [datum]' van 'Automatisch verlengen op [datum]'. 

Als u de API (ZOWEL VOOR als Partner Center) gebruikt, kunt u verlopende abonnementen ontdekken door de einddatum van het abonnement samen met de eigenschap auto renew = False te evalueren. 

De E4-abonnementen worden op 7 april 2017 ingesteld op automatisch verlengen=Onwaar. U kunt klanten op elk moment naar een nieuw plan verplaatsen. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Office 365 Enterprise E4-editievervangingsplannen

U kunt ervoor kiezen om dezelfde functionaliteit te behouden met E4 of uw klanten te laten profiteren van nieuwere functies en functionaliteit in Office 365 en Skype voor Bedrijven Online. Prijsdetails vindt u in de matrix met prijzen en aanbiedingslijst in Partner Center. Secure Product Enterprise E3 of Secure Productive Enterprise E5 kan worden vervangen door respectievelijk Office 365 Enterprise E3 of Office 365 Enterprise E5.

- Optie 1: Office 365 Enterprise E5

- Optie 2: Office 365 Enterprise E3 + Skype voor Bedrijven Cloud PBX

- Optie 3: Office 365 Enterprise E3 + Skype voor Bedrijven Plus CAL (prijs- en functionaliteitspariteit met E4)

- Optie 4: Office 365 Enterprise E3


| Functie | Optie 1 | Optie 2 | Optie 3 | Optie 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Alle functies van Office 365 Enterprise E4? | Ja | Ja | Ja | Nee |
| Telefoonnummers die worden beheerd in Office 365? | Ja | Ja | Nee | Nee |
| Telefoonnummers die zowel on-premises als in Office 365 (hybride implementatie) worden beheerd? | Ja | Ja | Nee | Nee |
| Optie voor het toevoegen van een PSTN-abonnement voor spraakbellen? | Ja | Ja | Nee | Nee |
| PSTN-conferencing? | Ja | Nee | Nee | Nee |
| Geavanceerde hulpprogramma's voor samenwerking, analyse en beveiliging? | Ja | Nee | Nee | Nee |
| Interactieve rapporten, dashboards en gegevensvisualisaties? | Ja | Nee | Nee | Nee | 
| Meer controle over gegevensbeveiliging en naleving met ingebouwde privacy, transparantie en verfijnde gebruikersbesturingselementen? | Ja | Nee | Nee | Nee | 

## <a name="transition-customers-to-new-product-plans"></a>Klanten overstappen op nieuwe productplannen

Microsoft biedt voortdurend nieuwe producten en services aan onze partners. In dergelijke gevallen moet u mogelijk klanten upgraden naar nieuwe services of hun abonnementen migreren van SKU's die uiteindelijk worden afgesloten. Voor het migreren van klanten van buiten gebruik stellende SKU's naar nieuwere SKU's zijn de volgende stappen vereist:

-   Het nieuwe abonnement kopen
-   Huidige gebruikerslicenties opnieuw toewijzen
-   Het oude abonnement annuleren

Volg deze stappen om het Office 365 Enterprise E4-abonnement van een klant te migreren naar een van de opties in de bovenstaande tabel.

### <a name="step-1---purchase-the-new-subscription"></a>Stap 1: het nieuwe abonnement kopen

1. Selecteer in **Partner Center** menu **Klanten,** selecteer de klant die u wilt verplaatsen en selecteer vervolgens **Abonnementen toevoegen.**

2. Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer **vervolgens Verzenden.**

   Uw klant moet nu zowel oude als nieuwe abonnementen, het oude Office 365 Enterprise E4-abonnement en het nieuwe doelabonnement hebben, bijvoorbeeld Optie 1 - Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Stap 2: wijs de licenties van de gebruikers van de klant opnieuw toe

1. Selecteer in **Partner Center** menu **Klanten,** selecteer de klant die u wilt verplaatsen en selecteer vervolgens Gebruikers **en licenties.** De pagina Gebruikers en licenties van de klant wordt geopend.

2. Als u gebruikerslicenties opnieuw wilt toewijzen, selecteert u de gebruiker die u opnieuw wilt toewijzen en selecteert u **vervolgens Licenties beheren.**

3. Schakel op **de pagina** Licenties beheren het selectievakje **Office 365 Enterprise E4-licentie** uit en selecteer een nieuw serviceabonnement voor het abonnement waar de klant naar overstapt.

4. Selecteer **Indienen**. Een bevestigingspagina bevat de nieuwe licentietoewijzingen.

5. Ga door met dezelfde stappen als andere klantgebruikers die opnieuw licenties moeten toewijzen.

Nadat u de gebruikerslicenties naar de nieuwe service hebt verplaatst, kunt u het uit gebruik genomen abonnement veilig op het hoogste klantniveau annuleren.

### <a name="step-3---cancel-the-old-subscription"></a>Stap 3: het oude abonnement annuleren

1. Selecteer in **Partner Center** menu **Klanten.** Selecteer de klant die u wilt verplaatsen en selecteer het abonnement dat u wilt annuleren.

2. Stel op de pagina met abonnementsdetails de abonnementsstatus in op **Tijdelijk.**

3. Selecteer **Indienen**.

Het oude abonnement is opgeschort en het nieuwe abonnement is actief. De inrichting van het abonnement wordt na 120 dagen automatisch verwijderd. De klant maakt geen extra kosten voor het oude abonnement.



 




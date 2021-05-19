---
title: Kaizala Pro-abonnementen migreren naar Microsoft 365
description: Meer informatie over het migreren van Kaizala Pro-abonnementen naar Microsoft 365 of Office 365-versies. Lees dit artikel voor meer informatie over het overstappen van uw klanten.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 583e9c40bb8d161c30440f12331dc8dcbf3db417
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146422"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Zelfstandige Kaizala Pro-abonnementen migreren naar Microsoft 365 of Office 365-versies

**Juiste rollen:** Verkoopagent

Met ingang van 1 juli 2020 stopt Microsoft de verkoop van de zelfstandige Kaizala Pro-service. Klanten kunnen na deze datum geen nieuwe Kaizala Pro-abonnementen meer aanschaffen en bestaande Kaizala Pro-abonnementen worden niet automatisch verlengd wanneer ze verlopen.

Om de continuïteit voor klanten te waarborgen, moet u klanten met verlopen zelfstandige Kaizala Pro-abonnementen overstappen op een ondersteunde SKU-optie, die hieronder wordt vermeld. Het is raadzaam om klanten vóór de jaarlijkse einddatum van het abonnement over te brengen naar nieuwe abonnementen om service-uitval voor klanten te voorkomen.

Als u de API (ZOWEL VOOR als Partner Center) gebruikt, kunt u verlopende abonnementen ontdekken door de einddatum van het abonnement te evalueren, samen met de eigenschap auto renew ingesteld op false: `auto renew = False` .

De E4-abonnementen worden ingesteld op 1 juli `auto renew=False` 2020. U kunt klanten op elk moment verplaatsen naar een nieuw plan.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro Standalone-vervangingsplannen

Met de nieuwe abonnementen kunnen uw klanten profiteren van nieuwere functies en functionaliteit in Microsoft 365. Prijsgegevens vindt u in de prijslijst en aanbiedingslijstmatrix in Partner Center.

- [**Microsoft 365 voor Bedrijven,**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2)waaronder:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business Standard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 voor Frontline,**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab)waaronder:
   - Microsoft 365 F3 (voorheen Microsoft 365 F1) en Office 365 F3
    
- [**Microsoft 365 voor Enterprise,**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans)waaronder: 
   - Office 365 E1
   - Microsoft 365 E3 en Office 365 E3
   - Microsoft 365 E5 en Office 365 E5

- [**Microsoft 365 for Education,**](https://www.microsoft.com/education/buy-license/microsoft365)waaronder: 
    - Microsoft 365 A1 en Office 365 A1
    - Microsoft 365 A3 en Office 365 A3
    - Microsoft 365 A5 en Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Klanten overstappen op nieuwe productplannen

Microsoft biedt voortdurend nieuwe producten en services aan onze partners. In dergelijke gevallen moet u mogelijk klanten upgraden naar nieuwe services of hun abonnementen migreren van SKU's die uiteindelijk worden afgesloten. Voor het migreren van klanten van buiten gebruik stellende SKU's naar nieuwere SKU's zijn de volgende stappen vereist:

A. Het nieuwe abonnement kopen

B. Huidige gebruikerslicenties opnieuw toewijzen

C. Oud abonnement annuleren


## <a name="migrate-your-customers-to-new-plans"></a>Uw klanten migreren naar nieuwe abonnementen

### <a name="a-purchase-the-new-subscription"></a>A. Het nieuwe abonnement kopen

1. Als u het nieuwe abonnement wilt kopen, selecteert u **in** Partner Center menu **Klanten,** selecteert u de klant die u wilt verplaatsen en selecteert u vervolgens **Abonnementen toevoegen.**

2. Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer **verzenden.**

Uw klant moet nu zowel oude als nieuwe abonnementen hebben, het oude zelfstandige Kaizala Pro-abonnement en het nieuwe doelabonnement, bijvoorbeeld Optie 1 - Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Huidige gebruikerslicenties opnieuw toewijzen

1. Als u de licenties van de gebruikers van de klant opnieuw wilt toewijzen, selecteert u klanten in het **menu Partner Center,** selecteert u de klant die u verplaatst en selecteert u vervolgens Gebruikers **en licenties.** De pagina Gebruikers en licenties van de klant wordt geopend.

2. Als u de gebruikerslicentie opnieuw wilt toewijzen, selecteert u de gebruiker die u opnieuw wilt toewijzen en selecteert u **vervolgens Licenties beheren.**

3. Schakel op **de pagina** Licenties beheren het selectievakje Kaizala Pro Standalone license uit en selecteer een nieuw serviceplan voor het abonnement waar de klant naar overstapt.

4.  Selecteer **Indienen**. Op een bevestigingspagina worden de nieuwe licentietoewijzingen vermeld. Ga door met hetzelfde proces voor andere gebruikers die licentietoewijzingen nodig hebben.

### <a name="c-cancel-old-subscription"></a>C. Oud abonnement annuleren

Nadat u de gebruikerslicentie naar de nieuwe service hebt verplaatst, kunt u het uit gebruik genomen abonnement veilig op klantniveau annuleren.

1.  Selecteer klanten **Partner Center** het menu **.** Selecteer de klant van wie u het abonnement annuleert.

2.  Stel op de detailpagina van het abonnement het abonnement in op **Opgeschort.**

3.  Selecteer **Indienen**.

Het oude abonnement is opgeschort en het nieuwe abonnement is actief. De inrichting van het abonnement wordt na 120 dagen automatisch verwijderd. De klant maakt geen extra kosten voor het oude abonnement.

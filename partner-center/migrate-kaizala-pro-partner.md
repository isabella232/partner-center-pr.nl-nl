---
title: Kaizala Pro-abonnementen migreren naar Microsoft 365
description: Meer informatie over Kaizala Pro migreren naar Microsoft 365 of Office 365 versies. Lees dit artikel voor meer informatie over het overstappen van uw klanten.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: e248657b9b4d4cf50cb7d38b2a0593ae6445bd28
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114843133"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft-365-or-office-365-versions"></a>Zelfstandige Kaizala Pro migreren naar Microsoft 365 of Office 365 versies

**Juiste rollen:** Verkoopagent

Vanaf 1 juli 2020 stopt Microsoft de verkoop van de Kaizala Pro zelfstandige service. Klanten kunnen na deze datum geen nieuwe Kaizala Pro meer aanschaffen en bestaande Kaizala Pro-abonnementen worden niet automatisch verlengd wanneer ze verlopen.

Om de continuïteit voor klanten te waarborgen, moet u klanten met verlopende Kaizala Pro zelfstandige abonnementen over zetten naar een ondersteunde SKU-optie, die hieronder wordt vermeld. Het is raadzaam om klanten vóór de jaarlijkse einddatum van het abonnement over te brengen naar nieuwe abonnementen om service-uitval voor klanten te voorkomen.

Als u de API (ZOWEL VOOR als Partner Center) gebruikt, kunt u verlopende abonnementen ontdekken door de einddatum van het abonnement te evalueren, samen met de eigenschap voor automatisch verlengen ingesteld op false: `auto renew = False` .

De E4-abonnementen worden ingesteld `auto renew=False` op 1 juli 2020. U kunt klanten op elk moment verplaatsen naar een nieuw abonnement.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Kaizala Pro Zelfstandige vervangingsplannen

Met de nieuwe abonnementen kunnen uw klanten profiteren van nieuwere functies en functionaliteit in Microsoft 365. Prijsdetails vindt u in de matrix met prijzen en aanbiedingslijst in Partner Center.

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

- [**Microsoft 365 for Education,**](https://www.microsoft.com/education/buy-license/microsoft365)met inbegrip van: 
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

2. Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer **vervolgens Verzenden.**

Uw klant moet nu zowel oude als nieuwe abonnementen hebben, het oude zelfstandige Kaizala Pro-abonnement en het nieuwe doelabonnement, bijvoorbeeld Optie 1 - Office 365 Enterprise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Huidige gebruikerslicenties opnieuw toewijzen

1. Als u de licenties van de gebruikers van de klant opnieuw wilt toewijzen, selecteert u klanten in het **menu Partner Center,** selecteert u de klant die u verplaatst en selecteert u vervolgens Gebruikers **en licenties.** De pagina Gebruikers en licenties van de klant wordt geopend.

2. Als u de gebruikerslicentie opnieuw wilt toewijzen, selecteert u de gebruiker die u opnieuw wilt toewijzen en selecteert u **vervolgens Licenties beheren.**

3. Schakel op **de pagina** Licenties beheren het selectievakje Kaizala Pro zelfstandige licentie uit en selecteer een nieuw serviceabonnement voor het abonnement waar de klant naar overstapt.

4.  Selecteer **Indienen**. Een bevestigingspagina bevat de nieuwe licentietoewijzingen. Ga door met hetzelfde proces voor andere gebruikers die licentietoewijzingen nodig hebben.

### <a name="c-cancel-old-subscription"></a>C. Oud abonnement annuleren

Nadat u de gebruikerslicentie hebt verplaatst naar de nieuwe service, kunt u het uit gebruik genomen abonnement veilig op klantniveau annuleren.

1.  Selecteer in **Partner Center** menu **Klanten.** Selecteer de klant van wie u het abonnement annuleert.

2.  Stel op de detailpagina van het abonnement het abonnement in op **Tijdelijk ingesteld.**

3.  Selecteer **Indienen**.

Het oude abonnement is opgeschort en het nieuwe abonnement is actief. De inrichting van het abonnement wordt na 120 dagen automatisch verwijderd. De klant maakt geen extra kosten voor het oude abonnement.

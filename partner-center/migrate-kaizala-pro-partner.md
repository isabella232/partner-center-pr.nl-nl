---
title: Kaizala Pro-abonnementen migreren naar Microsoft365
description: Meer informatie over het migreren van Kaizala Pro-abonnementen naar Microsoft365 of Office 365-versies. Lees dit artikel voor meer informatie over het overstappen van uw klanten.
ms.topic: article
ms.service: partner-dashboard
ms.author: sukumart
author: sukumart
ms.date: 06/01/2020
localization_priority: Normal
ms.openlocfilehash: 0807931ae95b5c7d76f4ad33708cc8014412f55f
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92528754"
---
# <a name="migrate-kaizala-pro-standalone-subscriptions-to-microsoft365-or-office-365-versions"></a>Zelfstandige Kaizala Pro-abonnementen migreren naar Microsoft365 of Office 365-versies

Met ingang van 1 juli 2020 wordt de verkoop van de zelfstandige Pro-service van Kaizala Professional beëindigd. Klanten kunnen na deze datum geen nieuwe Kaizala Pro-abonnementen meer kopen en bestaande Kaizala Pro-abonnementen worden niet automatisch verlengd wanneer ze verlopen.

Om ervoor te zorgen dat klanten zich kunnen voordoen, moet u klanten overstappen met de zelfstandige Kaizala Pro-abonnementen op een ondersteunde SKU-optie die hieronder wordt weer gegeven. U wordt aangeraden klanten te verplaatsen naar nieuwe abonnementen vóór de jaarlijkse eind datum van het abonnement om eventuele service storingen voor klanten te voor komen.

Als u de API (topof partner centrum) gebruikt, kunt u verlopen abonnementen detecteren door de eind datum van het abonnement te evalueren en de eigenschap automatisch verlengen in te stellen op False: `auto renew = False` .

De E4-abonnementen worden ingesteld op `auto renew=False` 1 juli 2020. U kunt klanten op elk gewenst moment verplaatsen naar een nieuw abonnement.

## <a name="kaizala-pro-standalone-replacement-plans"></a>Zelfstandige Kaizala Pro-vervangings plannen

Met de nieuwe plannen kunnen uw klanten profiteren van nieuwere functies en functionaliteit in Microsoft 365. Prijs informatie vindt u in de matrix prijs lijst en aanbiedings lijst in partner centrum.

- [**Microsoft 365 voor bedrijven**](https://www.microsoft.com/microsoft-365/compare-all-microsoft-365-products?&activetab=tab:primaryr2), waaronder:  
   - Microsoft 365 Business Basic
   - Microsoft 365 Business standaard
   - Microsoft 365 Business Premium
    
- [**Microsoft 365 voor Frontline**](https://www.microsoft.com/microsoft-365/microsoft-365-enterprise-f3?activetab=pivot:overviewtab), met inbegrip van:
   - Microsoft 365 F3 (voorheen Microsoft 365 F1) en Office 365 F3
    
- [**Microsoft 365 voor bedrijven**](https://www.microsoft.com/microsoft-365/compare-microsoft-365-enterprise-plans), waaronder: 
   - Office 365 E1
   - Microsoft 365 E3 en Office 365 E3
   - Microsoft 365 E5 en Office 365 E5

- [**Microsoft 365 voor onderwijs**](https://www.microsoft.com/education/buy-license/microsoft365), waaronder: 
    - Microsoft 365 a1 en Office 365 a1
    - Microsoft 365 a3 en Office 365 a3
    - Microsoft 365 A5 en Office 365 A5

## <a name="transition-customers-to-new-product-plans"></a>Klanten overstappen naar nieuwe product abonnementen

Micro soft biedt voortdurend nieuwe producten en services aan onze partners. In dergelijke gevallen moet u mogelijk klanten upgraden naar nieuwe services of hun abonnementen migreren vanuit Sku's die uiteindelijk worden afgesloten. Voor het migreren van klanten uit buiten gebruik gestelde Sku's naar nieuwere versies moeten de volgende stappen worden uitgevoerd:

A. Het nieuwe abonnement kopen

B. Huidige gebruikers licenties opnieuw toewijzen

C. Oud abonnement annuleren


## <a name="migrate-your-customers-to-new-plans"></a>Uw klanten migreren naar nieuwe abonnementen

### <a name="a-purchase-the-new-subscription"></a>A. Het nieuwe abonnement kopen

1. Als u het nieuwe abonnement wilt kopen, selecteert u in het menu van het **partner centrum** **klanten** , selecteert u de klant die u wilt verplaatsen en selecteert u vervolgens **abonnementen toevoegen** .

2. Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer vervolgens **verzenden** .

Uw klant moet nu over zowel oude als nieuwe abonnementen beschikken, het oude Kaizala Pro zelfstandige-abonnement en het nieuwe doel abonnement, bijvoorbeeld optie 1-Office 365 Enter prise F1.

### <a name="b-reassign-current-user-licenses"></a>B. Huidige gebruikers licenties opnieuw toewijzen

1. Als u de gebruikers licenties van de klant opnieuw wilt toewijzen, selecteert u in het menu van het **partner centrum** **klanten** , selecteert u de klant die u wilt verplaatsen en selecteert u vervolgens **gebruikers en licenties** . De pagina gebruikers en licenties van de klant wordt geopend.

2. Als u de gebruikers licentie opnieuw wilt toewijzen, selecteert u de gebruiker die u opnieuw wilt toewijzen en selecteert u vervolgens **licenties beheren** .

3. Schakel op de pagina **licenties beheren** het selectie vakje Kaizala Pro-zelfstandige licentie uit en selecteer een nieuw service plan voor het abonnement waarnaar de klant wordt verplaatst.

4.  Selecteer **Indienen** . Een bevestigings pagina bevat een lijst met de nieuwe licentie toewijzingen. Herhaal dit hetzelfde proces voor andere gebruikers die licentie toewijzingen nodig hebben.

### <a name="c-cancel-old-subscription"></a>C. Oud abonnement annuleren

Nadat u de gebruikers licentie hebt verplaatst naar de nieuwe service, kunt u het buiten gebruik gestelde abonnement op klant niveau veilig annuleren.

1.  Selecteer in het menu **Partner Center** **klanten** . Selecteer de klant van wie u het abonnement wilt annuleren.

2.  Stel op de pagina abonnements Details het abonnement in op **opgeschort** .

3.  Selecteer **Indienen** .

Het oude abonnement is onderbroken en het nieuwe abonnement is actief. Het opgeschorte abonnement wordt na 120 dagen niet meer ingericht. De klant heeft geen extra kosten in rekening gebracht voor het oude abonnement.

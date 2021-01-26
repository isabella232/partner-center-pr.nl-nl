---
title: Locaties in uw partner account beheren
ms.topic: how-to
ms.date: 01/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het toevoegen van een nieuwe locatie en hoe de MPN-ID van de locatie wordt gebruikt in prikkel Programma's, CSP-bedrijven, abonnementen en andere trans acties.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 38ea8a451f51d80998643e2a023420ea3efaa6ba
ms.sourcegitcommit: e99882e9b6c9b1a0f7427fb133693b1d977be76b
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/26/2021
ms.locfileid: "98773433"
---
# <a name="manage-your-mpn-account-locations-and-add-a-new-location"></a>Uw MPN-account locaties beheren en een nieuwe locatie toevoegen


**Juiste rollen**

- Globale beheerder
- Accountbeheerder

De MPN-ID van de locatie identificeert elke specifieke locatie van uw bedrijf. U gebruikt de MPN-ID van de locatie om in te schrijven in prikkel-Program ma's, voor het bedrijf van de Transact Cloud Solution Provider (CSP) en andere zakelijke trans acties. De ID van de globale MPN wordt gebruikt voor niet-transactionele activiteiten zoals ondersteunings aanvragen.

## <a name="the-following-is-a-typical-scenario"></a>Hier volgt een typisch scenario:

Contoso heeft het wereld wijde account van de partner (PGA) in het Verenigd Konink rijk. Dit is hun rechts bedrijf en de algemene MPN-ID wordt gebruikt voor het beheren van alle niet-transactionele zakelijke activiteiten. Contoso heeft ook partner locatie accounts (PLA) die gelijk zijn aan dochter ondernemingen of afdelingen op een andere locatie in UK, Frank rijk en de Verenigde Staten. In de MPN-account structuur worden deze PLAs vertegenwoordigd als unieke locatie MPN-Id's. De PLAs worden gebruikt voor transactionele activiteiten zoals CSP of prikkel Programma's. Uitbetalingen zijn gekoppeld aan specifieke locaties. 

>[!NOTE]
>Er is een 1-1-relatie tussen een CSP-Tenant en een MPN locatie-ID.

:::image type="content" source="images/locations/locations1.png" alt-text="Structuur van MPN-locaties":::

## <a name="prerequisites-in-order-to-add-a-new-account-location-for-a-csp-business"></a>Vereisten voor het toevoegen van een nieuwe account locatie voor een CSP-bedrijf

Er zijn verschillende vereisten om een nieuwe CSP-bedrijfs locatie toe te voegen:

1. U moet een locatie MPN-ID hebben in het land waar u zaken wilt doen.

1. U hebt een nieuwe Azure AD-Tenant nodig in de [bedrijfs regio](regional-authorization-overview.md) die nog niet is inge SCHREVEN bij CSP. Dit maken wanneer u zich registreert bij CSP.
 
3. Gebruik de nieuwe AAD-Tenant om u aan te melden bij het CSP-programma in de regio.
Juridische Bedrijfs gegevens opgeven, inclusief de naam van het bedrijf, het adres, de primaire contact gegevens. Dit account wordt gecontroleerd. Zorg er dus voor dat u geldige gegevens toevoegt.

>[!NOTE] 
 >Meld u aan met de **nieuwe** referenties voor de **nieuwe** Azure AD-Tenant. Gebruik uw bestaande referenties niet als het partner centrum u heeft herkend als al een account.

4. Ga akkoord met de micro soft-partner overeenkomst en activeer het account.

## <a name="add-an-mpn-location"></a>Een MPN-locatie toevoegen

1. Meld u aan met het MPN-account in het partner centrum. Het MPN-account moet globale beheerders-of account beheerders bevoegdheden hebben. 

1. Selecteer de **organisatie-instellingen** op het **pictogram instelling**.

2. Selecteer **juridisch** en selecteer vervolgens **locaties.**

3. Selecteer **een locatie toevoegen** en voeg de adres gegevens in van de locatie die u wilt toevoegen aan uw bedrijf, evenals een primaire contact persoon voor de locatie.

> [!NOTE]
> Zodra een locatie is toegevoegd in het partner centrum, kan deze niet meer worden verwijderd. U ziet **MPN** in het menu links van partner centrum als u de juiste MPN-id hebt gebruikt om u aan te melden.

## <a name="change-global-partner-account-location"></a>Locatie van globale partner account wijzigen

1. Controleer op **[bedrijfs locaties](https://partner.microsoft.com/dashboard/account/v3/organization/legalinfo#mpn)** de lijst met locaties om ervoor te zorgen dat de gewenste locatie als uw rechts persoon wordt weer gegeven. Als dat niet het geval is, voegt u deze toe.

   :::image type="content" source="images/accountsettings/location1.png" alt-text="Scherm afbeelding van de pagina account locaties van partner centrum met een lijst met alle huidige locaties.":::

2. Selecteer **juridisch** en selecteer **juridisch zakelijk profiel bijwerken**
  
3. Selecteer de regio en rechts persoon en **Verzend** deze.

  
## <a name="next-steps"></a>Volgende stappen

- Meer informatie over het [verificatie proces](verification-responses.md).

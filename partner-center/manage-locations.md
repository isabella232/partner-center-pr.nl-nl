---
title: Locaties in uw partner account beheren
ms.topic: how-to
ms.date: 01/26/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het toevoegen van een nieuwe locatie en hoe de MPN-ID van de locatie wordt gebruikt in prikkel Programma's, CSP-bedrijven, abonnementen en andere trans acties.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 21d82fc3ec4470d4941d3ca7436089d3e892439e
ms.sourcegitcommit: 81017727107a907bf1f3246097b51667d7c5fb18
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/30/2021
ms.locfileid: "99098887"
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

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Vereisten voor het toevoegen van een nieuw account voor een CSP-bedrijf

Als u een nieuw CSP-account wilt toevoegen, moet u eerst controleren of u aan de vereisten hebt voldaan.

1. U moet een locatie MPN-ID hebben in het land waar u de CSP-onderneming wilt maken. Lees "een MPN-locatie toevoegen" hieronder om een nieuwe MPN-locatie te maken.
  
1. Lees voor het maken van een nieuwe CSP indirecte reseller-inschrijving [werk met indirecte providers](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Meld u aan met de **nieuwe** referenties voor het **nieuwe** CSP-account. Gebruik uw bestaande referenties niet als het partner centrum u heeft herkend als al een account.

2. Ga akkoord met de micro soft-partner overeenkomst en activeer het account.

## <a name="view-your-mpn-locations"></a>Uw MPN-locaties weer geven

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard/home) van de partner centrum met de referenties van uw MPN-account. (Uw MPN-referenties kunnen afwijken van uw CSP-referenties) 
 
1. Selecteer op het pictogram **instellingen** **account instellingen**, **organisatie profiel**, **juridisch**. 

1. Controleer op het tabblad **partner** of er geen banner fout bericht wordt weer gegeven waarin u wordt gevraagd om gemigreerde locaties te herstellen vanuit PMC. Als dat het geval is, volgt u de instructies en verhelpt u deze locaties. 

3. Als er geen fout bericht wordt weer gegeven, selecteert u in  **instellingen**  **account instellingen**, **organisatie profiel**, **id's**.

4. Zoek naar de MPN-ID van het type "locatie" die overeenkomt met het land van dit CSP-account en gebruik het om de koppeling te doorzoeken en te volt ooien.

5. Als u de locatie MPN-ID die overeenkomt met de CSP-account die u wilt gebruiken niet kunt vinden, kunt u een nieuwe locatie toevoegen waarmee een nieuwe MPN-ID wordt gemaakt. Zie hieronder **een MPN-locatie toevoegen** .

## <a name="add-an-mpn-location"></a>Een MPN-locatie toevoegen

1. Meld u aan met het MPN-account in het partner centrum. (Uw MPN-referenties kunnen afwijken van uw CSP-referenties). Het MPN-account moet globale beheerders-of account beheerders bevoegdheden hebben. 

1. Selecteer op het **pictogram instellingen** de **account instellingen** en selecteer vervolgens **organisatie profiel**.

2. Selecteer **juridisch** en selecteer vervolgens op het tabblad **partner** de optie **bedrijfs locaties** en klik op **een locatie toevoegen.**

3. Geef de vereiste gegevens op, inclusief de naam van het bedrijf, het adres en de contact persoon voor de locatie die u aan uw bedrijf wilt toevoegen.
 
1. Klik op **locatie toevoegen**. Hiermee wordt een nieuwe MPN-ID gemaakt voor de nieuwe locatie die u kunt gebruiken voor CSP-trans acties en-prikkels.

:::image type="content" source="images/legal-biz.png" alt-text="Een nieuw juridisch bedrijf toevoegen":::

> [!NOTE]
> Zodra een locatie is toegevoegd in het partner centrum, kan deze niet meer worden verwijderd. U ziet **MPN** in het menu links van partner centrum als u de juiste MPN-id hebt gebruikt om u aan te melden.

## <a name="change-country-of-partner-global-account"></a>Het wereld wijde account land van de partner wijzigen 

1. Meld u aan met het MPN-account in het partner centrum. (Uw MPN-referenties kunnen afwijken van uw CSP-referenties). Het MPN-account moet globale beheerders-of account beheerders bevoegdheden hebben. 

2. Ga op het tabblad **partner** naar **bedrijfs locaties** en controleer de lijst met locaties om te controleren of de gewenste locatie als uw juridische entiteit wordt vermeld. 
 
1. Als u een locatie wilt toevoegen, klikt u op **een locatie toevoegen** en geeft u in de vlucht uit de vereiste gegevens op, inclusief de naam van het bedrijf, het adres en de primaire contact persoon voor de locatie die u aan uw bedrijf wilt toevoegen. 
 
1. Selecteer **uw land wijzigen** naast de vervolg keuzelijst **land/regio** en volg de stappen. 

:::image type="content" source="images/lbp.png" alt-text="Gegevens van juridisch zakelijk profiel worden in vlucht gegeven":::

5. Klik op **Opslaan**.

6. De land instelling van het MPN Global-account wordt gewijzigd in het nieuwe juridische land.
  
## <a name="next-steps"></a>Volgende stappen

- Meer informatie over het [verificatie proces](verification-responses.md).

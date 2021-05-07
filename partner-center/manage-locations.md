---
title: Locaties in uw partneraccount beheren
ms.topic: how-to
ms.date: 05/01/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het toevoegen van een nieuwe locatie en hoe de MPN-id van de locatie wordt gebruikt in incentive-programma's, CSP-bedrijven, abonnementen en andere transacties.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8a2b4fa8b204b10d5d45c0e1409ab4bc463e272f
ms.sourcegitcommit: 22e257d5b334ca8d3fc072f59010a508e1022694
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/06/2021
ms.locfileid: "108702889"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Uw MPN-accountlocaties beheren en een locatie toevoegen (verwijderen)


**Juiste rollen**

- Globale beheerder
- Accountbeheerder

De MPN-id van de locatie identificeert elke specifieke locatie van uw bedrijf. U gebruikt de MPN-locatie-id om u in te schrijven voor incentive-programma's, om Cloud Solution Provider (CSP)-transacties en andere zakelijke transacties uit te voeren. De algemene MPN-id wordt gebruikt voor niet-transactionele activiteiten, zoals ondersteuningsaanvragen.

## <a name="the-following-scenario-is-typical"></a>Het volgende scenario is gebruikelijk:

Contoso heeft een Partner Global Account (PGA) in het Vk. De PGA is hun geregistreerde juridische bedrijf en de globale MPN-id wordt gebruikt voor het beheren van alle niet-transactionele bedrijf. Contoso heeft ook partnerlocatieaccounts (PLA) die gelijk zijn aan dochterondernemingen of divisies op een andere locatie in het Vk, Frankrijk en de Verenigde Staten. In de structuur van het MPN-account worden deze PLA's weergegeven als unieke LOCATIE-MPN-ID's. De PLA's worden gebruikt voor transactionele activiteiten zoals CSP of incentives-programma's. Uitbetalingen zijn gekoppeld aan specifieke locaties. 

>[!NOTE]
>Er is een 1-1-relatie tussen een CSP-tenant en een MPN-locatie-id.

:::image type="content" source="images/locations/locations1.png" alt-text="Structuur van MPN-locaties":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Vereisten voor het toevoegen van een nieuw account voor een CSP-bedrijf

Als u een nieuw CSP-bedrijfsaccount wilt toevoegen, moet u er eerst voor zorgen dat u aan de vereisten hebt voldaan.

1. U moet een MPN-locatie-id hebben in het land waar u CSP-zaken wilt doen. Lees 'Een MPN-locatie toevoegen' hieronder om een nieuwe MPN-locatie te maken.
  
1. Als u een nieuwe CSP Indirect Reseller wilt maken, leest [u Werken met indirecte providers](indirect-reseller-tasks-in-partner-center.md#get-started) 

>[!NOTE] 
 >Vergeet niet om u aan te melden met **de nieuwe** referenties voor het **nieuwe** CSP-account. Gebruik uw bestaande referenties niet, omdat Partner Center herkent dat u al een account hebt.

2. Accepteer de Microsoft Partner-overeenkomst en activeer het account.

1. Als u zich wilt inschrijven als partner voor directe factuur, leest u [Vereisten voor directe factuurpartners](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>Uw MPN-locaties weergeven en bijwerken

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard/home) met de referenties van uw MPN-account. (Uw MPN-referenties kunnen verschillen van uw CSP-referenties) 
 
1. Selecteer in **het** pictogram Instellingen de optie **Accountinstellingen,** **Organisatieprofiel,** **Juridisch.** 

1. Controleer op **het tabblad Partner** of er geen bannerfoutbericht wordt weergegeven waarin u wordt gevraagd om gemigreerde locaties van PMC op te lossen.  Als uw locaties niet correct zijn ingesteld in PMC en nog niet zijn overgestappen naar pc, moet u deze locaties bijwerken.

:::image type="content" source="images/locations/location-two.png" alt-text="Schermkapje laat zien hoe u de locatie bij kunt werken.":::
 
4.  Selecteer in **het scherm PMC-locaties** controleren de optie **Bijwerken.**
Werk de volgende velden bij:

- **Veld Naam:** zorg ervoor dat de naam van de bedrijfslocatie juist is. Als er een dubbele fout wordt weergegeven, probeert u te wijzigen van bijvoorbeeld Contoso in Contoso, Inc.

- **Veld Juridische entiteit:** Zorg ervoor dat u de juridische entiteit hebt gekozen waar de locatie aan is gekoppeld

- **Adresregel 1 & 2 velden:** zorg ervoor dat het adres juist is

- **Velden & plaats/provincie:** zorg ervoor dat de combinatie tussen de plaats en de staat/provincie juist is. Er zijn landen waar de vervolgkeuzelijst voor het kiezen van staat/provincie van toepassing is en in andere landen moet dat veld handmatig worden ingevoegd.

- **Postcodeveld: zorg** ervoor dat het postcodeveld overeenkomt met uw aangegeven land, regio, plaats of adres.

- **Velden** met primaire contactgegevens: zorg ervoor dat de velden voor- en achternaam zijn ingevuld en dat het aangegeven e-mailadres een werk-e-mailadres is en geen persoonlijk e-mailadres (bijvoorbeeld @outlook.com , , @live.com enzovoort)

- **Veld Telefoonnummer:** zorg ervoor dat het telefoonnummer GEEN speciale tekens, spaties of landcode bevat. De waarde die in het veld Telefoonnummer wordt ingevoerd, bevat altijd maximaal 10 tekens.

5. Als er geen foutbericht is, selecteert u in Instellingen de optie **Accountinstellingen,** **Organisatieprofiel,** **Id's.**

6. Zoek de MPN-id met het type 'Locatie' die overeenkomt met het land van dit CSP-account en gebruik deze om de associatie te voltooien.

7. Als u de MPN-locatie-id die overeenkomt met het CSP-account dat u wilt gebruiken niet kunt vinden, kunt u een nieuwe locatie toevoegen, waarmee een nieuwe MPN-id wordt gemaakt. Zie **Een MPN-locatie toevoegen** hieronder.

## <a name="add-an-mpn-location"></a>Een MPN-locatie toevoegen

1. Meld u aan met het MPN-account in Partner Center. (Uw MPN-referenties kunnen verschillen van uw CSP-referenties). Het MPN-account moet globale beheerders- of accountbeheerdersbevoegdheden hebben. 

1. Selecteer in **het pictogram Instellingen** de **accountinstellingen en** selecteer vervolgens **Organisatieprofiel.**

2. Selecteer **Juridisch** en selecteer vervolgens op het **tabblad Partner** de optie **Bedrijfslocaties en** klik op Een locatie **toevoegen.**

3. Geef de vereiste gegevens op, zoals de bedrijfsnaam, het adres en de contactpersoon voor de locatie die u aan uw bedrijf wilt toevoegen.
 
1. Klik **op Locatie toevoegen.** Hiermee maakt u een nieuwe MPN-id voor de nieuwe locatie die u kunt gebruiken voor CSP-transacties en incentives.

:::image type="content" source="images/legal-biz.png" alt-text="Een nieuw juridisch bedrijf toevoegen":::

> [!NOTE]
> Zodra een locatie is toegevoegd aan Partner Center, kunt u deze niet verwijderen. U ziet **MPN** in het linkermenu van Partner Center als u de juiste MPN-id hebt gebruikt om u aan te melden.

## <a name="add-the-registration-number-id"></a>De id van het registratienummer toevoegen

Als u een indirecte provider, directe factuurpartner of indirecte reseller bent en u zaken doet met nieuwe of bestaande klanten in de volgende landen, moet u registratie-id-nummers voor uw bedrijf verstrekken. Als het land waarin u zaken doet niet hieronder wordt vermeld, is de registratie-id optioneel.

- Armenië 
- Azerbeidzjan 
- Belarus 
- Brazilië 
- Hongarije 
- India 
- Irak 
- Kazachstan 
- Kirgistan 
- Moldavië 
- Myanmar 
- Polen 
- Rusland 
- Saoedi-Arabië 
- Zuid-Afrika 
- Zuid-Soedan  
- Tadzjikistan 
- Thailand
- Turkije 
- Oekraïne 
- Verenigde Arabische Emiraten 
- Oezbekistan 
- Venezuela
- Vietnam 


Lees Registratie-id-nummergegevens [voor meer informatie](reg-number-id.md)

## <a name="delete-a-location"></a>Een locatie verwijderen

Als u een locatie uit uw account wilt verwijderen, moet u contact opnemen met [partnerondersteuning.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) Zorg ervoor dat u begrijpt wat de impact van deze actie is. Verwijderde locaties kunnen niet worden opgehaald en alles wat is gekoppeld aan die specifieke MPN-id, wordt niet meer herkend of is actief voor uw bedrijf.

## <a name="change-country-of-partner-global-account"></a>Land van algemeen partneraccount wijzigen 

1. Meld u aan met het MPN-account in Partner Center. (Uw MPN-referenties kunnen verschillen van uw CSP-referenties). Het MPN-account moet de bevoegdheden Globale beheerder of Accountbeheerder hebben. 

2. Ga op **het tabblad Partner** naar Bedrijfslocaties en controleer de lijst met locaties om ervoor te zorgen dat de locatie die u wilt gebruiken als uw juridische entiteit wordt vermeld.  
 
1. Als u een locatie wilt toevoegen, klikt u op Een locatie toevoegen en geeft u in het fly-outvenster de vereiste gegevens op, waaronder de bedrijfsnaam, het adres en de primaire contactpersoon voor de locatie die u aan uw bedrijf wilt toevoegen. 
 
1. Selecteer **Uw land wijzigen** naast de **vervolgkeuzekeuze** selecteren en volg de stappen. 

:::image type="content" source="images/lbp.png" alt-text="Juridische bedrijfsprofielgegevens zijn beschikbaar":::

5. Klik op **Opslaan**.

6. Het land van het globale MPN-account wordt gewijzigd in het nieuwe juridische land.
  
## <a name="next-steps"></a>Volgende stappen

- Meer informatie over het [verificatieproces](verification-responses.md).

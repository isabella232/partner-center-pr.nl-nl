---
title: Locaties in uw partneraccount beheren
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Meer informatie over het toevoegen van een nieuwe locatie en hoe de MPN-id van de locatie wordt gebruikt in incentive-programma's, CSP-bedrijven, abonnementen en andere transacties.
author: vinayks
ms.author: vinayks
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b994d4dc483e030586ea615b5835afbc7555cabe
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129075855"
---
# <a name="manage-your-mpn-account-locations-and-add-delete-a-location"></a>Uw MPN-accountlocaties beheren en een locatie toevoegen (verwijderen)

**Juiste rollen:** Globale | Accountbeheerder

De MPN-id van de locatie identificeert elke specifieke locatie van uw bedrijf. U gebruikt de MPN-id van de locatie om u in te schrijven voor incentive-programma's, om Cloud Solution Provider (CSP) en andere zakelijke transacties uit te voeren. De algemene MPN-id wordt gebruikt voor niet-transactionele activiteiten, zoals ondersteuningsaanvragen.

## <a name="the-following-scenario-is-typical"></a>Het volgende scenario is gebruikelijk:

Contoso heeft een Partner Global Account (PGA) in het Vk. De PGA is hun geregistreerde juridische bedrijf en de globale MPN-id wordt gebruikt voor het beheren van alle niet-transactionele bedrijf. Contoso heeft ook partnerlocatieaccounts (PLA) die gelijk zijn aan dochterondernemingen of divisies op een andere locatie in het Vk, Frankrijk en de Verenigde Staten. In de structuur van het MPN-account worden deze PLA's weergegeven als unieke LOCATIE-MPN-ID's. De PLA's worden gebruikt voor transactionele activiteiten zoals CSP of incentives-programma's. Uitbetalingen zijn gekoppeld aan specifieke locaties.

> [!NOTE]
> Er is een een-op-een-relatie tussen een CSP-tenant en een MPN-locatie-id.

:::image type="content" source="images/locations/locations1.png" alt-text="Structuur van MPN-locaties.":::

## <a name="prerequisites-in-order-to-add-a-new-account-for-a-csp-business"></a>Vereisten voor het toevoegen van een nieuw account voor een CSP-bedrijf

Als u een nieuw CSP-bedrijfsaccount wilt toevoegen, moet u er eerst voor zorgen dat u aan de vereisten hebt voldaan.

1. U moet een MPN-locatie-id hebben in het land waar u CSP-zaken wilt doen. Lees 'Een MPN-locatie toevoegen' hieronder om een nieuwe MPN-locatie te maken.
  
2. Als u een nieuwe CSP Indirect Reseller wilt maken, leest [u Werken met indirecte providers.](indirect-reseller-tasks-in-partner-center.md#get-started)

> [!NOTE]
> Vergeet niet om u aan te melden met **de nieuwe** referenties voor het **nieuwe** CSP-account. Gebruik uw bestaande referenties niet, omdat Partner Center herkent dat u al een account hebt.

3. Accepteer de Microsoft Partner-overeenkomst en activeer het account.

4. Als u zich wilt inschrijven als partner voor directe factuur, leest [u Vereisten voor directe factuurpartners](direct-partner-new-requirements.md)

## <a name="view-and-update-your-mpn-locations"></a>Uw MPN-locaties weergeven en bijwerken

1. Meld u aan bij [Partner Center dashboard met](https://partner.microsoft.com/dashboard) de referenties van uw MPN-account. (Uw MPN-referenties kunnen verschillen van uw CSP-referenties.)

2. Selecteer het Instellingen tandwielpictogram en selecteer vervolgens **Account Instellingen** en vervolgens **Juridisch.**

3. Controleer op **het tabblad Partner** of er geen bannerfoutbericht wordt weergegeven waarin u wordt gevraagd om gemigreerde locaties van PMC op te lossen.  Als uw locaties niet correct zijn ingesteld in PMC en nog niet naar de pc zijn overgestappen, moet u deze locaties bijwerken.

:::image type="content" source="images/locations/location-two.png" alt-text="Schermkapje laat zien hoe u de locatie bij kunt werken.":::

4. Selecteer in **het scherm PMC-locaties** controleren de optie **Bijwerken.**
Werk de volgende velden bij:

- **Naamveld:** zorg ervoor dat de naam van de bedrijfslocatie juist is. Als er een duplicaatfout wordt weergegeven, probeert u te wijzigen van bijvoorbeeld Contoso in Contoso, Inc.

- **Veld Juridische entiteit:** Zorg ervoor dat u de juridische entiteit hebt gekozen waar de locatie aan is gekoppeld

- **Adresregel 1 & 2 velden:** zorg ervoor dat het adres juist is

- **Velden & staat/provincie:** zorg ervoor dat de combinatie tussen de plaats en de staat/provincie juist is. Er zijn landen waar de vervolgkeuzelijst voor het kiezen van de staat/provincie van toepassing is en in andere landen moet dat veld handmatig worden ingevoegd.

- **Postcodeveld: zorg** ervoor dat het postcodeveld overeenkomt met uw aangegeven land, regio, plaats of adres.

- **Velden** met primaire contactgegevens: zorg ervoor dat de velden voor- en achternaam zijn ingevuld en dat het aangegeven e-mailadres een werk-e-mailadres is en geen persoonlijk e-mailadres (bijvoorbeeld @outlook.com , , @live.com enzovoort)

- **Telefoon getalveld:** zorg ervoor dat het Telefoon geen speciale tekens, spaties of landcode bevat. De waarde die is ingevoerd in Telefoon veld Getal, bevat altijd maximaal 10 tekens.

5. Als er geen foutbericht is, selecteert u **Instellingen**, Instellingen **Accountprofiel** **,** Organisatieprofiel , **Id's.**

6. Zoek de MPN-id met het type 'Locatie' die overeenkomt met het land van dit CSP-account en gebruik deze om de associatie te voltooien.

7. Als u de MPN-locatie-id die overeenkomt met het CSP-account dat u wilt gebruiken niet kunt vinden, kunt u een nieuwe locatie toevoegen, waarmee een nieuwe MPN-id wordt gemaakt. Zie **Een MPN-locatie toevoegen** hieronder.

## <a name="add-an-mpn-location"></a>Een MPN-locatie toevoegen

1. Meld u aan met het MPN-account in Partner Center. (Uw MPN-referenties kunnen verschillen van uw CSP-referenties.) Het MPN-account moet globale beheerders- of accountbeheerdersbevoegdheden hebben.

2. Selecteer het Instellingen tandwielpictogram, vervolgens **Account Instellingen** en selecteer **vervolgens Organisatieprofiel.**

3. Selecteer **Juridisch** en selecteer vervolgens op het **tabblad Partner** de optie **Bedrijfslocaties en** selecteer Een locatie **toevoegen.**

4. Geef de vereiste gegevens op, zoals de bedrijfsnaam, het adres en de contactpersoon voor de locatie die u aan uw bedrijf wilt toevoegen.

5. Selecteer **Locatie toevoegen.** Hiermee maakt u een nieuwe MPN-id voor de nieuwe locatie die u kunt gebruiken voor CSP-transacties en incentives.

:::image type="content" source="images/legal-biz.png" alt-text="Voeg een nieuw juridisch bedrijf toe.":::

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

Als u een locatie uit uw account wilt verwijderen, neemt u contact op met [partnerondersteuning.](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=1af7f3a0-1757-3543-4b6a-c945c3ad187b) Zorg ervoor dat u begrijpt wat de impact van deze actie is. Verwijderde locaties kunnen niet worden opgehaald en alles wat is gekoppeld aan die specifieke MPN-id, wordt niet meer herkend of is actief voor uw bedrijf.

## <a name="change-country-of-partner-global-account"></a>Land van partneraccount wijzigen

1. Meld u aan met het MPN-account in Partner Center. (Uw MPN-referenties kunnen verschillen van uw CSP-referenties.) Het MPN-account moet globale beheerders- of accountbeheerdersbevoegdheden hebben.

2. Selecteer het Instellingen tandwielpictogram en vervolgens **Account Instellingen**. Ga op **het tabblad Partner** naar Bedrijfslocaties en controleer de lijst met locaties om ervoor te zorgen dat de locatie die u wilt gebruiken als uw juridische entiteit wordt vermeld. 

3. Als u een locatie wilt toevoegen, klikt u op Een locatie toevoegen en geeft u de vereiste gegevens op, waaronder de bedrijfsnaam, het adres en de primaire contactpersoon voor de locatie die u aan uw bedrijf wilt toevoegen.

4. Selecteer **Uw land wijzigen** naast de **vervolgkeuzelijst Land/regio** en volg de stappen.

:::image type="content" source="images/lbp.png" alt-text="Juridische bedrijfsprofielgegevens zijn beschikbaar.":::

5. Selecteer **Opslaan**.

6. Het land van het globale MPN-account wordt gewijzigd in het nieuwe juridische land.
  
## <a name="next-steps"></a>Volgende stappen

- Meer informatie over het [verificatieproces](verification-responses.md).

---
title: Pagina Klanten voor MCI-betrokkenheid
description: Gebruik de pagina Klanten in de sectie Microsoft Commerce Incentive (MCI)-programma Engagements om klanten te beheren.
author: Karthic83
ms.author: kashanum
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
ms.topic: how-to
ms.date: 09/29/2021
ms.custom: template-how-to
ms.openlocfilehash: 4d4d3de7bc53440765538654f8e82c3c048f5922
ms.sourcegitcommit: a59e1abb470f4847e8f8337ffa4ba705514a0424
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/29/2021
ms.locfileid: "129293390"
---
# <a name="customers-page-for-mci-engagements"></a>Pagina Klanten voor MCI-betrokkenheid

**Juiste rollen:** Incentives-| Incentives-gebruiker

>[!NOTE]
>Dit is alleen van toepassing op betrokkenheid bij build-intenties, dat wil zeggen workshops. 

Op **de** pagina Klanten worden klanten gesorteerd op in aanmerking komende, niet-in aanmerking komende klanten en voltooid voor elke betrokkenheid. De pagina wordt vooraf weergegeven met alle klanten die toestemming hebben gegeven voor een workshop in Partner Center. 

:::image type="content" source="images/incentives/customers-page.png" alt-text="Schermopname van de pagina Klanten." lightbox="images/incentives/customers-page.png":::

- Op **het tabblad** In aanmerking komend worden alle klanten weergegeven die in aanmerking komen voor de workshop. 
   - In **de kolom Type** worden klanten weergegeven als 'actief' als u toestemming van de klant hebt ontvangen. Tot die tijd wordt er 'niet gestart' gezegd.
- Op **het tabblad Ineligible** worden om een van de volgende drie redenen alle klanten weergegeven die niet in aanmerking komen voor de workshop:  
   - De klant voldoet niet aan de geschiktheidscriteria voor de betrokkenheid, 
   - De klant heeft toestemming gegeven aan een andere partner, of 
   - De klant heeft al met een andere partner deelgenomen aan de workshop. 
- Op **het** tabblad Voltooid ziet u alle klanten voor wie u deze workshop hebt voltooid. U kunt de details van uw claim met deze klant bekijken door Workshopclaim **weergeven te selecteren** onder de **kolom** Actie.

Voor elke betrokkenheid moet u een klant toevoegen of een klant claimen (niet beide).

## <a name="add-a-customer"></a>Een klant toevoegen 
1. Selecteer **+ Klant toevoegen op** de pagina **Klanten** van de relevante workshopafspraak met behulp van het tabblad **In aanmerking** komend.
2. Geef een MPN-locatie-id op voor de workshop en het e-mailadres van de klant. Het **veld Customer TPID /Tenant ID** is optioneel. Alleen MPN-locatie-ID's die zijn ingeschreven bij het MCI-programma en in aanmerking komen voor deze betrokkenheid, worden weer geven. Selecteer **Next**.
   - Als u geen tenant-id of bovenste bovenliggende id (TPID) voor de klant op geeft, leidt het systeem de tenant-id af van het e-mailadres van de klant. Vervolgens wordt de geschiktheidscontrole voor de klant uitgevoerd voor de workshop.
   - Als de tenant-id van de klant niet kan worden gevonden met behulp van het e-mailadres, wordt u gevraagd een ander e-mailadres of de tenant-id/TPID op te geven.
   - Als de tenant-id/TPID is opgegeven, zorgt het systeem ervoor dat het e-maildomein overeenkomt met de tenant-id. Als er een niet-overeenkomende wordt gevonden, vraagt het systeem u om een reden op te geven.

   :::image type="content" source="images/incentives/add-customer-1.png" alt-text="Schermopname 1 van 3 die laat zien hoe u een klant toevoegt." lightbox="images/incentives/add-customer-1.png":::

3. Kies de workshop(s) waarvoor u de klant wilt toevoegen. Alleen die workshops kunnen worden geselecteerd waarvoor zowel u als uw klant in aanmerking komen. Selecteer **Next**.

:::image type="content" source="images/incentives/add-customer-2.png" alt-text="Schermopname 2 van 3 die laat zien hoe u een klant toevoegt." lightbox="images/incentives/add-customer-2.png":::

4. Bekijk de informatie en selecteer **Klant toevoegen.** U krijgt een bevestiging dat de klant is toegevoegd.

:::image type="content" source="images/incentives/add-customer-3.png" alt-text="Schermopname 3 van 3 die laat zien hoe u een klant toevoegt." lightbox="images/incentives/add-customer-3.png":::

U ziet nu de klant die u  hebt toegevoegd op de respectieve pagina's klanten voor de workshopafspraak die u in stap 3 hebt geselecteerd.

## <a name="claim-a-customer"></a>Een klant claimen 
Op **het** tabblad In **aanmerking** komend op de pagina Klanten wordt vooraf een lijst met klanten weergegeven die bekend zijn bij u, de partner, via andere betrokkenheiden. U kunt een workshop starten met elk van deze klanten. 
1. Selecteer **Klant claimen** in de **kolom** Actie. 
2. Kies een MPN-locatie-id voor de workshop. Alleen de MPN-locatie-ID's die zijn ingeschreven bij het MCI-programma en die in aanmerking komen voor deze betrokkenheid, worden weergegeven. Selecteer **Next**.

   :::image type="content" source="images/incentives/claim-customer-1.png" alt-text="Schermopname 1 van 3 die laat zien hoe u een klant claimt." lightbox="images/incentives/claim-customer-1.png":::

3. Kies de workshop(s) die u wilt toevoegen en selecteer vervolgens **Volgende.**

   :::image type="content" source="images/incentives/claim-customer-2.png" alt-text="Schermopname 2 van 3 die laat zien hoe u een klant kunt claimen." lightbox="images/incentives/claim-customer-2.png":::

4. Bekijk de informatie en selecteer **Klant toevoegen.** U ontvangt een bevestiging dat de klant is geclaimd.

   :::image type="content" source="images/incentives/claim-customer-3.png" alt-text="Schermopname 3 van 3 die laat zien hoe u een klant claimt." lightbox="images/incentives/claim-customer-3.png":::

## <a name="ask-for-customer-consent"></a>Vragen om toestemming van de klant 
Als u een workshop wilt uitvoeren met een klant, moet u de klant om toestemming vragen. Dit is hun overeenkomst om deel te nemen aan de workshop. U hebt in totaal 30 dagen om toestemming te krijgen nadat u de klant hebt toegevoegd of geclaimd.

Nadat u een klant hebt toegevoegd of geclaimd, ziet u hoeveel dagen u nog hebt om toestemming te krijgen in de statuskolom op de **pagina** Klanten.
1. Selecteer **Toestemming van klant activeren** in de **kolom** Actie. 
2. Geef de e-mail en contactgegevens van de klant op, samen met contactgegevens voor uw eigen bedrijf. Selecteer vervolgens **Volgende**.

   :::image type="content" source="images/incentives/ask-consent-1.png" alt-text="Schermopname 1 van 2 die laat zien hoe u toestemming van de klant kunt aanvragen." lightbox="images/incentives/ask-consent-1.png":::

3. Controleer de details en selecteer **Verzenden voor toestemming.** Er wordt een e-mailbericht verzonden naar de klant, zodat deze de workshop kan accepteren of weigeren.
   - Als u nog geen toestemming hebt ontvangen, kunt u een herinnering verzenden door te klikken op de koppeling Klant toestemming **opnieuw** verzenden onder de **kolom** Actie.
   - Als een klant zojuist is toegevoegd, maar deelname aan de workshop weigert of niet binnen  de vereiste tijdlijn reageert, wordt deze niet meer weergegeven op de pagina Klanten voor die betrokkenheid.

   :::image type="content" source="images/incentives/ask-consent-2.png" alt-text="Schermopname 2 van 2 die laat zien hoe u toestemming van de klant aanvraagt." lightbox="images/incentives/ask-consent-2.png":::

Zodra de klant toestemming heeft gegeven, hebt u 90 dagen om de workshop uit te voeren.

## <a name="next-steps"></a>Volgende stappen
[Een workshopclaim indienen](/mci-engagements-workshop)

[Overzicht en geschiktheid van MCI-betrokkenheiden](/mci-engagements)

[Gebruik deze resources om aan de slag te gaan met incentives](/incentives-get-started-intro)

[Geschiktheid van uw incentives-programma bepalen](/incentives-determined-your-program-eligibility)

[Inschrijving en gebruikersbeheer in het incentives-programma](/incentives-enroll)
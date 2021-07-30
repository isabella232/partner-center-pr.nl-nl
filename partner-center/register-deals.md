---
title: Uw deals registreren
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Wanneer u een deal registreert die u hebt gewonnen in Partner Center, kan Microsoft u in de toekomst meer mogelijkheden bieden.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: 1a3d83dbac20cbcb038345ba90ae1a4dc345c060
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842538"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Registreer deals die u hebt gewonnen in Partner Center

**Juiste rollen:** Verwijzingenbeheerder

U kunt deals die u hebt gewonnen, registreren in Partner Center door aanvullende informatie over het contract op te geven. Deze informatie helpt ons om u in de toekomst meer mogelijkheden te bieden.

Er zijn twee paden die leiden tot dealregistratie:

- U hebt een nieuwe deal gemaakt in de sectie Kansen voor **co-verkoop** en uw deal voldoet aan de criteria voor dealregistratie.
- U wilt een gesloten ISV-Verbinding maken, die niet samen met Microsoft is verkocht.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Een deal registreren die afkomstig is van een co-verkoopkans

Als u een deal wilt registreren die afkomstig is van een verkoopkans, moet uw deal voldoen aan de volgende geschiktheidsvereisten:

- Het type deal is co-sell of partner-led (u hebt ervoor gekozen om Microsoft-verkopers toe te staan deze deal te bekijken).
- Er is ten minste één oplossing die in aanmerking komt voor een incentive in de deal. Een oplossing komt in aanmerking voor een incentive als deze ten minste een van de volgende tags bevat:
  - Azure IP Co-sell
  - Business Applications Premium
  - Business Applications Standard
- De status van de deal is 'Gewonnen'.
- Als het type deal co-sell is, moet Microsoft de uitnodiging hebben geaccepteerd of de deal als gewonnen hebben gemarkeerd. U kunt de Microsoft-status bekijken door te kijken naar de Microsoft-kaart onder de details van uw deal.

Als u aan de geschiktheidsvereisten voldoet, wordt u automatisch gevraagd om uw deal te registreren met een **knop** Nu registreren die wordt weergegeven op de voortgangsbalk van de deal:

:::image type="content" source="images/register-deals.png" alt-text="Schermopname van de voortgangsbalk van de deal.":::

> [!NOTE]
> Als het **dealregistratie-item** niet wordt weer geven in de voortgangsbalk van de deal, voldoet de deal niet aan alle vereisten voor dealregistratie.

Nadat u op **Nu registreren** hebt geklikt, wordt u omgeleid naar de pagina Dealregistratie en wordt u gevraagd een formulier in te vullen met vooraf ingevulde gegevens voor uw klant en oplossing. Vul het formulier in met behulp van de onderstaande instructies en klik op **Registreren.**

Na registratie worden er een of twee dealregistratierecords gemaakt, afhankelijk van de oplossing.

- Als uw oplossing in aanmerking komt voor ISV Connect, wordt er een ISV Connect-dealregistratierecord gemaakt. Deze dealregistratierecord wordt gebruikt voor facturering.
- Als uw oplossing in aanmerking komt voor incentives voor ip-co-verkoop, wordt er een registratierecord voor een IP-deal gemaakt. Deze registratierecord van de deal wordt beoordeeld en goedgekeurd of afgewezen door het beoordelingsteam van de deal voor co-sell.

## <a name="report-a-closed-isv-connect-deal"></a>Een gesloten ISV-Verbinding maken melden

Als u een gesloten ISV-Verbinding maken wilt rapporteren, gaat u naar het tabblad **Dealregistratie** en klikt u op + Rapport gesloten **ISV-Verbinding maken deal**. Vul de vereiste velden in en klik op **Registreren.** Deze dealregistratierecord wordt gebruikt voor facturering.

## <a name="fill-out-the-deal-registration-form"></a>Vul het formulier voor dealregistratie in

> [!NOTE]
> U kunt deals filteren op klantnaam, status en type deal. Klik om dit te doen op **de knop Filteren** bovenaan de pagina Dealregistratie.

Of u nu registratie wilt dealen vanuit een verkoopkans of u een gesloten ISV-Verbinding maken-deal rapporteert die niet samen met Microsoft is verkocht, u wordt gevraagd de volgende velden in te vullen op het formulier voor dealregistratie.

- **Klantgegevens:** voer de **bedrijfsnaam voor** uw klant in en selecteer hun **land/regio.** Voer vervolgens hun **plaats en** **staat/provincie in.**
- **Oplossing:** selecteer de oplossing die wordt gebruikt voor de deal. Als de juiste oplossing niet wordt vermeld, neem dan contact op met de ondersteuning.
- **Contracttype:** geef op of deze deal een **nieuw** contract of een **verlenging van** een eerder contract is.
- **Totale contractwaarde:** de totale verwachte waarde voor de overeenkomst. Deze waarde moet alle software- en servicekosten omvatten, maar niet de hardwarekosten. Zorg ervoor dat u de juiste valuta selecteert.
- **Oplossingswaarde:** de totale waarde van de cloudoplossing die voor de deal wordt gebruikt. Vergeet niet alle kosten op te nemen die zijn gekoppeld aan software- en onderhoudskosten, maar niet de kosten voor het opnieuw betalen van items, niet-terugkerende aanpassingskosten of rechtstreeks gekoppelde CSP-licentiekosten die door Microsoft worden betaald.
- **Wordt de oplossing geïmplementeerd in Azure? Als dat niet het beste is, kiest** u Overige: selecteer **Azure** of **Overige.**
- **Wordt het verbruik van de oplossing uitgevoerd op de partner- of klant-tenant?**: Selecteer de **tenant Klant** of **de Partner-tenant.**
- **Begindatum van contract:** de datum waarop het contract begint. Gebruik voor betalen per gebruik-deals de datum van de eerste factuur. Met deze Partner Center u geen begindatum eerder dan de contractdatum invoeren. Dit kan van invloed zijn op sommige deals, zoals IP-implementaties die vóór de aanmeldingsdatum beginnen. Als u deze deals wilt invoeren, gebruikt  u de contractdatum voor de velden voor zowel de tekendatum als de begindatum wanneer u een aanvraag indient. (In het contract moet expliciet de duur van de deal worden vermeld, zodat ACV correct kan worden berekend.)
- **Einddatum van contract:** als het contract op een specifieke datum eindigt, selecteert u **Heeft een einddatum** en geeft u die datum op. Als het contract geen specifieke einddatum heeft, selecteert u **Doorlopende**. Gebruik voor betalen per gebruik-deals de datum van de laatste of meest recente factuur.
- **Contract ondertekende** datum: de datum waarop het definitieve contract is ondertekend door uw organisatie en door de klant. Gebruik voor betalen per gebruik-deals de datum van de eerste factuur.
- **Contactpersoon voor** registratie: de voornaam, achternaam,  **Telefoon-nummer** en e-mail voor een persoon in uw organisatie met wie we contact kunnen opnemen als we meer informatie nodig hebben over een van de informatie die hier wordt verstrekt.  

Wanneer u alle secties van de pagina hebt voltooid, klikt u op **Registreren.**

- Als de deal een ISV-Verbinding maken is, ziet u dat de status van de deal 'Ingediend, Voltooid' is. Er is geen verdere actie vereist voor deze registratierecord van de deal. Deze record wordt gebruikt voor facturering.
- Als de deal een IP-deal voor co-verkoop is, ziet u dat de status van de deal 'Ingediend' is. Het beoordelingsteam van Microsoft Co-Sell Deal beoordeelt de informatie die u hebt opgegeven in deze registratierecord van de deal. Het beoordelingsteam vraagt u indien nodig meer actie aan of keurt de deal rechtstreeks goed/af.
- Als u een deal registreert die afkomstig is van een verkoopkans en u ziet dat er twee registratierecords voor deal zijn gemaakt, betekent dit dat de oplossing voor uw deal in aanmerking komt voor zowel ISV-Verbinding maken als IP-co-verkoop. De ISV Verbinding maken record wordt gebruikt voor facturering. De IP-record voor co-sell wordt beoordeeld door het validatieteam van de deal voor co-sell.

## <a name="simplified-deal-registration-for-commercial-marketplace-transactions"></a>Vereenvoudigde dealregistratie voor commerciële marketplace-transacties

Co-Sell via de commerciële marketplace [](https://docs.microsoft.com/azure/marketplace/) wint, profiteert u van een aanzienlijke vereenvoudiging van het dealregistratieformulier.  Daarnaast zijn voor deals die worden gedaan via commerciële marketplace geen aanvullende aanroepen voor beoordeling van deals nodig, waardoor de operationele tijd en inspanningen worden bespaart.

U hoeft slechts drie gegevens op te geven:

1. Geef aan (selectievakje) of de deal is ver transacted of zal worden ver transact via de commerciële marketplace.
2. Geschatte transactiedatum (MM-DD-YYYY).
3. Partnercontactgegevens registreren voor het geval er vragen zijn over de deal.

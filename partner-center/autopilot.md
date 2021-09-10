---
title: De out-of-box-ervaring van een apparaat aanpassen
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Voordat u het nieuwe apparaat van een klant levert, kunt u Windows Autopilot-profielen gebruiken om de out-of-box experience (OOBE) van het apparaat aan te passen of vooraf te configureren.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 95a201c53fc2eaf230d08bb4cfdd03a5747b5c05
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957325"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Windows Autopilot-profielen gebruiken op nieuwe apparaten om de kant-en-klaar-ervaring van een klant aan te passen

**Juiste rollen:** beheeragent | Globale beheerder | Verkoopagent | Beheerder van gebruikersbeheer

Als u klantapparaten beheert, moet u mogelijk de out-of-box experience (OOBE) aanpassen voor de gebruikers van de klant. U kunt nieuwe apparaten vooraf configureren met Windows Autopilot-profielen voordat u de apparaten aan klanten levert en nieuwe profielen kunt toepassen op apparaten die klanten al hebben aangeschaft. 

Houd er rekening mee dat OEM's zijn begonnen met het gebruik van een verzendlabel aan de buitenzijde van het Autopilot-apparaatvak, met daarin de **PKID (Product Key ID)** van het apparaat.  Deze 1-dimensionale, leesbare streepjescode biedt downstreampartners een manier om apparaten te registreren voor Autopilot zonder dat de apparaat-id's moeten worden uit postvak gemaakt en de apparaat-id op een alternatieve manier moet worden gesereerd.

In dit artikel wordt uitgelegd hoe u Autopilot-profielen kunt maken en toepassen op apparaten in Partner Center.

Als u nog niet bekend bent met Autopilot, bekijkt u de informatie in deze artikelen:

- [Overzicht van Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Naslaghandleiding voor Autopilot-implementatie](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Overzicht

Met de Windows Autopilot-functie in Partner Center kunt u aangepaste profielen maken om toe te passen op apparaten van klanten. De volgende profielinstellingen waren beschikbaar op het moment dat dit artikel werd gepubliceerd:

- Privacy-instellingen overslaan. Met deze optionele Autopilot-profielinstelling kunnen organisaties geen vragen stellen over privacy-instellingen tijdens het OOBE-proces.

- Het maken van lokale beheerdersaccounts op het apparaat uitschakelen. Organisaties kunnen bepalen of de gebruiker die het apparaat instel, beheerderstoegang moet hebben zodra het proces is voltooid.

- Apparaat automatisch instellen voor werk of school. Alle apparaten die zijn geregistreerd bij Autopilot, worden automatisch beschouwd als werk- of schoolapparaten. Deze vraag wordt dus niet gesteld tijdens het OOBE-proces.

- Sla Cortana pagina's voor OneDrive- en OEM-registratie over. Alle apparaten die zijn geregistreerd bij Autopilot slaan deze pagina's automatisch over tijdens het OOBE-proces (Out-Of-Box Experience).

- Gebruikslicentieovereenkomst (EULA) overslaan. Vanaf Windows 10 versie 1709 kunnen organisaties besluiten de pagina met de eula die tijdens het OOBE-proces wordt gepresenteerd, over te slaan. Zie [Windows autopilot-eula](#windows-autopilot-eula-dismissal) hieronder voor belangrijke informatie over het overslaan van de eula-pagina tijdens Windows installatie.

De volgende profiel- en apparaatbeheermachtigingen en -beperkingen zijn van toepassing:

- CSP-partners kunnen Autopilot-profielen blijven beheren voor bestaande klanten waarmee ze een reseller-relatie hebben, zelfs als de klanten de gedelegeerde beheermachtigingen van de partner hebben verwijderd.

- U kunt bestaande apparaten beheren voor de klanten die u hebt toegevoegd.

- U kunt geen apparaten beheren die uw klant heeft geüpload naar Microsoft Store voor Bedrijven of de Microsoft Intune-portal.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Autopilot-profielen maken en beheren in Partner Center

In Partner Center kunt u Windows Autopilot-implementatieprofielen maken en deze toepassen op apparaten.

>[!NOTE]
>Alleen beheerdersagents kunnen profielen maken en toepassen.

### <a name="create-a-new-autopilot-profile"></a>Een nieuw Autopilot-profiel maken

1. Selecteer **Klanten** in Partner Center menu en selecteer vervolgens de klant voor wie u het Autopilot-profiel maakt.

2. Selecteer apparaten op de detailpagina van **de klant.**

3. Selecteer **Windows Autopilot-profielen** **de optie Nieuw profiel toevoegen.**

4. Voer de naam en beschrijving van het profiel in en configureer vervolgens de OOBE-instellingen. U kunt kiezen uit:  

   - Privacy-instellingen overslaan tijdens de installatie

   - Lokaal beheerdersaccount uitschakelen tijdens de installatie
  
   - Pagina's automatisch overslaan tijdens de installatie<br>
        (Inclusief *de pagina's Automatisch instellen* voor werk of school selecteren en *Pagina'Cortana, OneDrive oem-registratie instellen)*
  
   - Gebruikersinterfaceovereenkomst (EULA) overslaan<br> 
       >[!IMPORTANT] 
       >Zie [Windows autopilot-eula](#windows-autopilot-eula-dismissal) hieronder voor belangrijke informatie over het overslaan van de eula-pagina tijdens Windows installatie.

5. Selecteer **Verzenden** wanneer u klaar bent.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Een Autopilot-profiel toepassen op apparaten van klanten

>[!NOTE]
>In de onderstaande instructies wordt ervan uitgenomen dat u de apparaten van de klant al hebt toegevoegd aan Partner Center en dat u toegang hebt tot de apparatenlijst. Als u de apparaten van de klant nog niet hebt toegevoegd, volgt u de instructies in Apparaten toevoegen aan het account van een [klant](#add-devices-to-a-customers-account) en volgt u de onderstaande stappen.

Nadat u een Autopilot-profiel voor een klant hebt gemaakt, kunt u dit toepassen op de apparaten van de klant.

1. Selecteer **Klanten** in het Partner Center selecteer vervolgens de klant voor wie u het Autopilot-profiel hebt gemaakt.

2. Selecteer apparaten op de detailpagina van **de klant.**

3. Selecteer **onder Profielen toepassen op apparaten** de apparaten of apparaatgroepen aan wie u profielen wilt toevoegen en selecteer vervolgens Profiel **toepassen.** Het profiel dat u zojuist hebt toegepast, wordt weergegeven in de **kolom** Profiel.

4. Volg de onderstaande stappen om te controleren of het profiel wordt toegepast op het apparaat.

    a.  Verbinding maken apparaat aan het netwerk en schakel het in.

    b.  Controleer of de juiste OOBE-schermen (indien van toepassing) worden weergegeven.

    c.  Wanneer het OOBE-proces stopt, stelt u de fabrieksinstellingen van het apparaat opnieuw in om het voor te bereiden voor een nieuwe gebruiker.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Een Autopilot-profiel verwijderen van het apparaat van een klant

1. Selecteer **Klanten** in het Partner Center selecteer vervolgens de klant voor wie u het Autopilot-profiel hebt gemaakt.

2. Selecteer apparaten op de detailpagina van **de klant.**

3. Selecteer **onder Profielen toepassen op** apparaten de apparaten waar u het profiel uit wilt verwijderen en selecteer vervolgens Profiel **verwijderen.**

   >[!NOTE]
   >Als u een profiel van een apparaat verwijdert, wordt het profiel niet uit de lijst verwijderd. Als u een profiel wilt verwijderen, volgt u de instructies in [Een Autopilot-profiel](#update-or-delete-an-autopilot-profile)bijwerken of verwijderen.

### <a name="update-or-delete-an-autopilot-profile"></a>Een Autopilot-profiel bijwerken of verwijderen

Als een klant de out-of-box-ervaring wil wijzigen nadat u de apparaten naar hen hebt verzonden, kunt u het profiel wijzigen in Partner Center.

Wanneer het apparaat van de klant verbinding maakt met internet, wordt de meest recente profielversie gedownload tijdens het OOBE-proces. Steeds als een klant de fabrieksinstellingen van een apparaat herstelt, downloadt het apparaat opnieuw de meest recente profielversie tijdens het OOBE-proces.

1. Selecteer **Klanten** in het Partner Center selecteer vervolgens de klant die u een Autopilot-profiel wilt laten wijzigen.

2. Selecteer apparaten op de detailpagina van **de klant.**

3. Selecteer **Windows Autopilot-profielen** het profiel dat u wilt bijwerken. Maak de vereiste wijzigingen en selecteer vervolgens **Verzenden.**

Als u dit profiel wilt verwijderen, **selecteert u** Profiel verwijderen in de rechterbovenhoek van de pagina.

### <a name="add-devices-to-a-customers-account"></a>Apparaten aan de account van een klant toevoegen

>[!NOTE]
>Verkoopagents en beheerdersagenten kunnen apparaten toevoegen aan het account van een klant.

Voordat u aangepaste Autopilot-profielen kunt toepassen op apparaten van klanten, moet u toegang hebben tot de apparatenlijst van de klant.

Als u van plan bent om de combinatie van OEM-naam, serienummer en model te gebruiken, moet u rekening houden met de volgende beperkingen:

- Deze tuple werkt alleen voor nieuwere apparaten (bijvoorbeeld 4k hashes) en wordt niet ondersteund voor 128b-hashes (RS2 en eerdere apparaten).

- De tuple-registratie is bestandsgevoelig, dus de gegevens in  het bestand moeten exact overeenkomen met de namen van het model en de fabrikant, zoals opgegeven door de OEM-provider (hardwareprovider).

Volg de onderstaande instructies om apparaten toe te voegen aan het account van een klant in Partner Center.

1. Selecteer **Klanten** in het Partner Center selecteer vervolgens de klant van wie u de apparaten wilt beheren.

2. Selecteer apparaten op de detailpagina van **de klant.**

3. Selecteer **onder Profielen toepassen op apparaten** de optie Apparaten **toevoegen.**

4. Voer een naam in voor de lijst met apparaten en selecteer vervolgens **Bladeren** om de lijst van de klant te uploaden (in .csv bestandsindeling) naar Partner Center.

    >[!NOTE]
    >U hebt dit bestand .csv ontvangen bij de aankoop van uw apparaat. Als u geen .csv hebt ontvangen, kunt u er zelf een maken door de stappen in Apparaten toevoegen aan Windows [Autopilot te volgen.](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)  

5. Upload het .csv en selecteer vervolgens **Opslaan.**

Als u een foutbericht krijgt terwijl u probeert het .csv-bestand te uploaden, moet u de bestandsindeling controleren. U kunt alleen de hardwarehash gebruiken, of de OEM-naam, het serienummer en het model (in die kolomvolgorde) of de Windows-product-id. U kunt ook het voorbeeldbestand .csv de koppeling naast **Apparaten toevoegen** gebruiken om een apparaatlijst te maken.

Uw .csv ziet er als het volgende uit:

> **Serienummer van apparaat,Windows product-id,hardware-hash,fabrikantnaam,apparaatmodel**

> **{serialNumber},,,Microsoft Corporation,Surface Laptop**

>[!NOTE]
> 'Fabrikantnaam' en 'Apparaatmodel' zijn casegevoelig.

Als u niet weet welke waarde u moet gebruiken voor Fabrikantnaam en Apparaatmodel, kunt u dit op het apparaat uitvoeren om de juiste waarden te verzamelen:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows Autopilot EULA-lidmaatschap

### <a name="important-information"></a>BELANGRIJKE INFORMATIE

Windows Met Autopilot kunt u aangepaste installaties van Windows op apparaten die u voor uw klanten beheert. Als de klant gemachtigd is om dit te doen, kunt u bepaalde instelschermen onderdrukken of verbergen die normaal gesproken aan gebruikers worden gepresenteerd bij het instellen van Windows, met inbegrip van het acceptatiescherm voor de gebruikersinterface (gebruikslicentieovereenkomst).

Door deze functie te gebruiken, gaat u ermee akkoord dat het onderdrukken of verbergen van schermen die zijn ontworpen om gebruikers te voorzien van kennisgeving of acceptatie van voorwaarden betekent dat u voldoende toestemming en autorisatie van uw klant hebt verkregen om voorwaarden te verbergen, en dat u namens uw klant (ongeacht of het om een organisatie of een afzonderlijke gebruiker gaat),  toestemming geven voor kennisgevingen en alle voorwaarden accepteren die van toepassing zijn op uw klant. Dit omvat overeenkomst met de voorwaarden van de licentie of kennisgeving die aan de gebruiker wordt gepresenteerd als u deze niet onderdrukt of verbergt met behulp van dit hulpprogramma. Uw klant mag de Windows-software op deze apparaten niet gebruiken als de klant geen geldige licentie voor de software heeft verkregen van Microsoft of zijn gelicentieerde distributeurs.
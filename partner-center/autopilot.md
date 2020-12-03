---
title: De out-of-Box Experience van een apparaat aanpassen
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Voordat u het nieuwe apparaat van een klant aflevert, kunt u Windows auto pilot-profielen gebruiken om de out-of-Box Experience (OOBE) van het apparaat aan te passen of vooraf te configureren.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534983"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Windows Autopilot-profielen gebruiken op nieuwe apparaten om de kant-en-klaar-ervaring van een klant aan te passen

**Juiste rollen**

- Beheer agent
- Globale beheerder
- Verkoop agent
- Beheerder van gebruikers beheer

Als u klant apparaten beheert, moet u mogelijk de out-of-Box Experience (OOBE) aanpassen voor de gebruikers van de klant. U kunt vooraf nieuwe apparaten configureren met Windows auto pilot-profielen voordat u de apparaten aan klanten levert en nieuwe profielen toepast op apparaten die klanten al hebben gekocht. 

Houd er rekening mee dat Oem's zijn begonnen met het verzenden van een verzend label op de buiten kant van het auto pilot-apparaat waarin de **product code-id (PKID)** van het apparaat wordt weer gegeven.  Deze 1-dimensionale, lees bare streepjes code biedt downstream partners een manier om apparaten te registreren voor auto pilot zonder dat ze de apparaten hoeven te Unbox en de apparaat-ID niet op een andere manier te hoeven verzamelen.

In dit artikel wordt uitgelegd hoe u auto pilot-profielen kunt maken en Toep assen op apparaten in het partner centrum.

Als u nog niet bekend bent met auto pilot, raadpleegt u de informatie in deze artikelen:

- [Overzicht van Windows Autopilot](/windows/deployment/windows-10-auto-pilot)
- [Naslag Gids voor auto pilot-implementatie](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Overzicht

Met de functie Windows auto pilot in Partner Center kunt u aangepaste profielen maken om op klant apparaten toe te passen. De volgende profiel instellingen zijn beschikbaar op het moment dat dit artikel werd gepubliceerd:

- Privacy-instellingen overs Laan. Met deze optionele auto pilot-profiel instelling kunnen organisaties geen privacy-instellingen meer vragen tijdens het OOBE-proces.

- Het maken van een lokaal beheerders account op het apparaat uitschakelen. Organisaties kunnen bepalen of de gebruiker die het apparaat instelt, beheerders toegang moet hebben nadat het proces is voltooid.

- Apparaat automatisch instellen voor werk of school. Alle apparaten die zijn geregistreerd met auto pilot worden automatisch beschouwd als werk-of school apparaten, zodat deze vraag niet wordt gesteld tijdens het OOBE-proces.

- Sla Setup-pagina's voor Cortana, OneDrive en OEM-registratie over. Alle apparaten die zijn geregistreerd met auto pilot, slaan deze pagina's automatisch over tijdens het OOBE-proces (out-of-Box Experience).

- De gebruiksrecht overeenkomst (EULA) overs Laan. Met ingang van Windows 10 versie 1709 kunnen organisaties besluiten de EULA-pagina die wordt gepresenteerd tijdens het OOBE-proces over te slaan. Zie de [gebruiksrecht overeenkomst voor Windows auto pilot](#windows-autopilot-eula-dismissal) hieronder voor belang rijke informatie over het overs laan van de EULA-pagina tijdens Windows Setup.

De volgende profiel- en apparaatbeheermachtigingen en -beperkingen zijn van toepassing:

- CSP-partners kunnen Autopilot-profielen blijven beheren voor bestaande klanten waarmee ze een reseller-relatie hebben, zelfs als de klanten de gedelegeerde beheermachtigingen van de partner hebben verwijderd.

- U kunt bestaande apparaten beheren voor de klanten die u hebt toegevoegd.

- U kunt geen apparaten beheren die uw klant heeft geüpload naar Microsoft Store voor Bedrijven of de Microsoft Intune-portal.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Auto Pilot-profielen maken en beheren in het partner centrum

In Partner Center kunt u Windows auto pilot-implementatie profielen maken en deze Toep assen op apparaten.

>[!NOTE]
>Alleen beheerder-agents kunnen profielen maken en Toep assen.

### <a name="create-a-new-autopilot-profile"></a>Een nieuw auto pilot-profiel maken

1. Selecteer **klanten** in het menu van het partner centrum en selecteer vervolgens de klant voor wie u het auto pilot-profiel wilt maken.

2. Selecteer op de detail pagina van de klant de optie **apparaten**.

3. Onder **Windows auto pilot-profielen** selecteert u **Nieuw profiel toevoegen**.

4. Voer de naam en beschrijving van het profiel in en configureer de OOBE-instellingen. U kunt kiezen uit:  

   - Privacy-instellingen in Setup overs Laan

   - Lokale beheerders account uitschakelen in installatie
  
   - Pagina's in Setup automatisch overs Laan<br>
        (Hiertoe *selecteert u automatisch instellingen voor werk of school en gaat u naar* de *pagina instellingen voor het instellen van Cortana, OneDrive en OEM-registratie.*
  
   - Gebruiksrecht overeenkomst overs Laan (EULA)<br> 
       >[!IMPORTANT] 
       >Zie de [gebruiksrecht overeenkomst voor Windows auto pilot](#windows-autopilot-eula-dismissal) hieronder voor belang rijke informatie over het overs laan van de EULA-pagina tijdens Windows Setup.

5. Selecteer **verzenden** wanneer u klaar bent.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Een auto pilot-profiel Toep assen op klant apparaten

>[!NOTE]
>In de onderstaande instructies wordt ervan uitgegaan dat u de apparaten van de klant al aan het partner centrum hebt toegevoegd en dat u toegang hebt tot hun apparaten lijst. Als u de apparaten van de klant nog niet hebt toegevoegd, volgt u de instructies in [apparaten toevoegen aan het account van een klant](#add-devices-to-a-customers-account) en volgt u de onderstaande stappen.

Nadat u een auto pilot-profiel voor een klant hebt gemaakt, kunt u dit Toep assen op de apparaten van de klant.

1. Selecteer **klanten** in het menu van het partner centrum en selecteer vervolgens de klant voor wie u het auto pilot-profiel hebt gemaakt.

2. Selecteer op de detail pagina van de klant de optie **apparaten**.

3. Selecteer onder **profielen Toep assen op apparaten** de apparaten of apparaatgroepen waaraan u profielen wilt toevoegen en selecteer vervolgens **profiel Toep assen**. Het profiel dat u zojuist hebt toegepast, wordt weer gegeven in de kolom **profiel** .

4. Volg de onderstaande stappen om te controleren of het profiel correct wordt toegepast op het apparaat.

    a.  Sluit een apparaat aan op het netwerk en schakel het in.

    b.  Controleer of de juiste OOBE-schermen (indien aanwezig) worden weer gegeven.

    c.  Wanneer het OOBE-proces wordt gestopt, herstelt u de fabrieks instellingen van het apparaat om het voor te bereiden voor een nieuwe gebruiker.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Een auto pilot-profiel verwijderen van het apparaat van een klant

1. Selecteer **klanten** in het menu van het partner centrum en selecteer vervolgens de klant voor wie u het auto pilot-profiel hebt gemaakt.

2. Selecteer op de detail pagina van de klant de optie **apparaten**.

3. Selecteer onder **profielen Toep assen op apparaten** de apparaten waarvan u het profiel wilt verwijderen en selecteer vervolgens **profiel verwijderen**.

   >[!NOTE]
   >Als u een profiel van een apparaat verwijdert, wordt het profiel niet uit de lijst verwijderd. Als u een profiel wilt verwijderen, volgt u de instructies in [Update of verwijdert u een auto pilot-profiel](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Een auto pilot-profiel bijwerken of verwijderen

Als een klant de out-of-Box-ervaring wil wijzigen nadat u de apparaten naar hen hebt verzonden, kunt u het profiel wijzigen in partner centrum.

Wanneer het apparaat van de klant verbinding maakt met internet, wordt de nieuwste profiel versie gedownload tijdens het OOBE-proces. Elke keer dat een klant een apparaat herstelt naar de standaard instellingen van de fabriek, zal het apparaat de meest recente profiel versie opnieuw downloaden tijdens het OOBE-proces.

1. Selecteer **klanten** in het menu van het partner centrum en selecteer vervolgens de klant voor wie u een auto pilot-profiel wilt wijzigen.

2. Selecteer op de detail pagina van de klant de optie **apparaten**.

3. Selecteer onder **Windows auto pilot-profielen** het profiel dat u wilt bijwerken. Breng de gewenste wijzigingen aan en selecteer vervolgens **verzenden**.

Als u dit profiel wilt verwijderen, selecteert u **profiel verwijderen** in de rechter bovenhoek van de pagina.

### <a name="add-devices-to-a-customers-account"></a>Apparaten aan de account van een klant toevoegen

>[!NOTE]
>Verkoop medewerkers en beheerders kunnen apparaten toevoegen aan het account van een klant.

Voordat u aangepaste auto pilot-profielen op klant apparaten kunt Toep assen, moet u toegang hebben tot de apparaten lijst van de klant.

Als u van plan bent om de combi natie van OEM-naam, serie nummer en model te gebruiken, moet u rekening houden met de volgende beperkingen:

- Deze tuple werkt alleen voor nieuwere apparaten (bijvoorbeeld 4.000 hashes) en wordt niet ondersteund voor 128b-hashes (RS2 en eerdere apparaten).

- De tuple-registratie is hoofdletter gevoelig, dus de gegevens in het bestand moeten overeenkomen met de namen van het model en de fabrikant **_precies_* gelijk aan de naam van de OEM-provider (hardwareprovider).

Volg de onderstaande instructies om apparaten toe te voegen aan het account van een klant in het partner centrum.

1. Selecteer _ *klanten** in het menu van het partner centrum en selecteer vervolgens de klant van wie u de apparaten wilt beheren.

2. Selecteer op de detail pagina van de klant de optie **apparaten**.

3. Selecteer **apparaten toevoegen** onder **profielen Toep assen op apparaten** .

4. Voer een naam in voor de apparaten lijst en selecteer vervolgens **Bladeren** om de lijst van de klant (in CSV-bestands indeling) naar het partner centrum te uploaden.

    >[!NOTE]
    >U zou dit CSV-bestand moeten hebben ontvangen bij de aankoop van uw apparaat. Als u geen CSV-bestand hebt ontvangen, kunt u er zelf een maken door de stappen in [apparaten toevoegen aan Windows auto pilot te](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell)volgen.  

5. Upload het CSV-bestand en selecteer vervolgens **Opslaan**.

Als u een foutbericht krijgt terwijl u probeert het .csv-bestand te uploaden, moet u de bestandsindeling controleren. U kunt alleen de hardwarehash gebruiken, of de OEM-naam, het serienummer en het model (in die kolomvolgorde) of de Windows-product-id. U kunt ook het bestand Sample. csv gebruiken dat is opgenomen in de koppeling naast **apparaten toevoegen** om een apparaten lijst te maken.

Het CSV-bestand ziet er ongeveer als volgt uit:

> **Serie nummer van apparaat, Windows-product-ID, hardware-hash, naam van fabrikant, model van apparaat**

> **{serialNumber},,, micro soft Corporation, Surface-laptop**

>[!NOTE]
> ' Fabrikant naam ' en ' apparaat model ' zijn hoofdletter gevoelig.

Als u niet weet welke waarde moet worden geplaatst voor de naam van de fabrikant en het model van het apparaat, kunt u dit op het apparaat uitvoeren om de juiste waarden te verzamelen:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Windows auto pilot-gebruiksrecht overeenkomst wordt genegeerd

### <a name="important-information"></a>BELANG RIJKE INFORMATIE

Met Windows auto pilot kunt u aangepaste installaties van Windows configureren op apparaten die u beheert voor uw klanten. Als de klant hiertoe hiertoe toestemming heeft gegeven, kunt u bepaalde ingestelde schermen onderdrukken of verbergen die normaal gesp roken worden gepresenteerd aan gebruikers bij het instellen van Windows, met inbegrip van de gebruiksrecht overeenkomst (EULA) op het acceptatie scherm.

Als u deze functie gebruikt, u stemt ermee in dat alle schermen die zijn ontworpen om gebruikers te voorzien van een kennisgeving of instemming van de voor waarden, te onderdrukken of te verbergen. Dit betekent dat u voldoende toestemming hebt verkregen voor het verbergen van de voor waarden en dat u namens uw klant (of een organisatie of een individuele gebruiker als het geval) de voor waarden die van toepassing zijn op uw klant. Dit omvat overeenkomst met de voor waarden van de licentie of de kennisgeving die aan de gebruiker zou worden gepresenteerd als u deze niet hebt onderdrukt of verborgen met dit hulp programma. Uw klant gebruikt de Windows-software mogelijk niet op deze apparaten als de klant geen licentie heeft aangeschaft voor de software van micro soft of haar gelicentieerde distributeurs.
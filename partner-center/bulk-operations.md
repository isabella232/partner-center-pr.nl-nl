---
title: Verkoopkansen voor bulksgewijs exporteren en importeren via Excel/CSV-bestanden in Verwijzingen
description: Informatie over het downloaden, maken of bijwerken van kansen voor co-verkoop met behulp van Excel -bestanden (CSV) in Partner Center
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-referrals
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 09/08/2021
ms.openlocfilehash: eb0f85eab9340d08a1f121c27f9a1956f5b71635
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244715"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Bulkbewerkingen voor verkoopkansen met behulp van CSV-bestanden (door komma's gescheiden waarden)

**Juiste rollen:** Beheerdersrollen voor verwijzingen | Verwijzingsgebruiker

Bulkbewerkingen in Partner Center helpen uw bedrijf bij het exporteren en importeren van gegevens voor collectieve-verkoopkansen. Navigeer naar de pagina voor **collectieve-verkoopkansen** voor de koppelingen voor **importeren** en **exporteren** rechtsboven in de banner met de paginatitel. Gebruikers met de machtigingen **Verwijzingenbeheerder** en **Verwijzingengebruiker** kunnen deze functionaliteit gebruiken.

> [!IMPORTANT]
> De acties voor maken/bijwerken die worden uitgevoerd via bulkimport, zijn niet omkeerbaar. Wees voorzichtig wanneer u een groot aantal records wijzigt of maakt. Na het maken van een deal kan slechts een subset velden worden gewijzigd. **Er zijn geen acties toegestaan zodra een deal een eindstatus heeft bereikt, zoals Geweigerd/Verlopen/Gewonnen/Verloren.**

## <a name="export-co-sell-opportunities"></a>Collectieve-verkoopkansen exporteren

In de volgende informatie wordt de exportfunctionaliteit beschreven:

- U kunt maximaal **5000 records exporteren** door op de **knop Exporteren te** klikken.
- De deals die worden gedownload, worden gebaseerd op uw toegangsniveaus. Verwijzingsbeheerders en verwijzingsgebruikers kunnen verschillende resultaten krijgen op basis van hun bereik en insluiting als teamleden in de deals. Meer informatie over [verwijzingenmachtigingen](permissions-overview.md#manage-referrals).
- Met de exportfunctie wordt rekening gehouden met het huidige tabblad op de pagina voor verkoopkansen voor co-verkoop en de filters die zijn toegepast.
- Er wordt een CSV-bestand gegenereerd met alle gegevens op basis van de toegepaste filters.
- Het downloaden van de records kan tot één minuut duren.
- U hoeft niet te wachten tot de downloadactie is voltooid. Zelfs als u naar andere pagina's in Partner Center navigeert, wordt het bestand gedownload zodra de exportfunctie is voltooid.
- U kunt het gedownloade bestand opnieuw gebruiken om de details van de deal te wijzigen en te uploaden om records bij te werken.

## <a name="import-co-sell-opportunities"></a>Collectieve-verkoopkansen importeren

- U kunt maximaal **1000 records** maken of bijwerken met behulp van de importfunctionaliteit.
- U kunt de sjabloon vanaf het begin bouwen door de sjabloon te downloaden van de pagina Importeren op Partner Center.
- U kunt ook de functionaliteit Exporteren gebruiken om de bestaande records te downloaden en bij te werken.
- Als het bestand meer dan 1000 records heeft, kan het niet worden verwerkt.
- Nadat het bestand is verwerkt, wordt een samenvatting met het aantal verwijzingen dat is gemaakt, bijgewerkt en niet verwerkt weergegeven in de kaart van het laatste procesbestand.
- U kunt de details van de verwerkte records downloaden, eventuele fouten oplossen en hetzelfde bestand uploaden om de records te maken of bij te werken die in de vorige run zijn mislukt. **Verwijder alle geslaagde records uit het bestand voordat u de gecorrigeerde records uploadt die in de vorige run zijn mislukt.**
- Als u meer oplossingen wilt toevoegen, voegt u extra kolommen toe naast oplossing 1 en gebruikt u de kolomnaam als Oplossing X, waarbij X het nummer van de oplossing in de deal vertegenwoordigt. Bijvoorbeeld Oplossing 2, Oplossing 3.
- U kunt maximaal 50 oplossingen toevoegen aan een deal.
- Als u meer teamleden wilt toevoegen, voegt u extra kolommen toe naast Teamlid 1 en gebruikt u de kolomnaam als Teamlid X, waarbij X het nummer van het teamlid in de deal vertegenwoordigt. Bijvoorbeeld Teamlid 2, Teamlid 3.
- U kunt maximaal 50 teamleden toevoegen aan een deal.

> [!NOTE]
> U hoeft niet te wachten tot de verwerking is voltooid. De details van het laatst verwerkte bestand kunnen worden gedownload zodra de verwerking is voltooid. **Het kan tot 10 minuten duren als u bestanden met 1000 records uploadt.**

> [!IMPORTANT]
> Lees alle instructies zorgvuldig en controleer de indeling van elke kolom uit de onderstaande tabel voordat u deals maakt of bijgaat met csv-bestanden in Partner Center.

|**Kolomnaam**|**Is verplicht?**|**Beschrijving**|**Voorbeeldwaarde(n)**|
|-----|:-----|:---------|:---|
Fouten|No|Fouten als er fouten zijn die betrekking hebben op de maak-/updatebewerkingen w.r.t naar de verwijzingen, worden in deze kolom opgenomen. Als er meerdere fouten zijn, worden deze allemaal weergegeven, gescheiden door puntkomma's.|Verplicht veld Oplossing 1 ontbreekt|
Betrokkenheids-id|No|De betrokkenheids-id wordt gegenereerd door microsoft Partner Center verwijzingssysteem. Niet vereist voor het maken van een nieuwe verwijzing. U kunt de bestaande betrokkenheids-id gebruiken als u een record bij wilt werken.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Verwijzings-id|No|Verwijzings-id wordt gegenereerd door microsoft Partner Center verwijzingssysteem. Niet vereist voor het maken van een nieuwe verwijzing. Vul deze in met de verwijzings-id als u een bestaande record bij wilt werken.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Dealnaam|Yes|De gebruiksvriendelijke naam voor de deal ter referentie.|UK Spring Deal
Naam van klant|Yes|Naam van het klantbedrijf. Gebruik de juridische naam van de organisatie voor snelle matching aan de zijde van Microsoft.|Contoso Corporation
Klantadresregel 1|Yes|Adresregel 1 van het klantbedrijf. |One Contoso Way
Klantadresregel 2|No|Adresregel 2 van het klantbedrijf.|NE 148 street
Plaats van klant|Yes|Plaats waar de klantorganisatie zich bevindt.|Redmond
Status van de klant|No|Staat waar de klantorganisatie zich bevindt.|Washington
Postcode van klant|No|Postcode van de regio waar de klantorganisatie zich bevindt.|98052
Land van klant|Yes|Land/regio waar de klantorganisatie zich bevindt. Gebruik de tweeletterig landcodes zoals hier [wordt vermeld.]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)|VS
D-U-N-S-id van klant|No|Probeer de DUNS-id van de klantorganisatie op te halen. Dit helpt bij een snellere afstemming van de klantorganisatie aan de zijde van Microsoft, waardoor verkopers sneller kunnen worden toewijsen. U kunt de DUNS-id gratis op deze [website downloaden.](https://www.dnb.com/duns-number/lookup.html)|81466849
Voornaam van contactpersoon van klant|Hangt|De voornaam is alleen verplicht als u hulp van Microsoft nodig hebt. De voornaam van de primaire contactpersoon van de klantorganisatie die aan deze deal werkt.|Jan
Achternaam van contactpersoon van klant|Hangt|De achternaam is alleen verplicht als u hulp van Microsoft nodig hebt. De achternaam van de primaire contactpersoon van de klantorganisatie die aan deze deal werkt.|Klant
Klantcontactnummer Telefoon|Hangt|Telefoon is alleen verplicht als u Hulp van Microsoft nodig hebt. Telefoon van de primaire contactpersoon van de klantorganisatie die aan deze deal werkt.|9999999999
E-mailadres van klantcontact|Hangt|E-mailadres is alleen verplicht als u Hulp van Microsoft nodig hebt. Het e-mailadres van de primaire contactpersoon van de klantorganisatie die aan deze deal werkt.|john.customer@contoso.com
Verwijzingsstatus van partner|Yes|Geeft de status van de deal aan vanuit het perspectief van uw bedrijf. Vereist als u een verwijzing wilt maken of wijzigen. Gebruik **Nieuw** als u een nieuwe deal probeert te maken. Geaccepteerde waarden worden hier [beschreven.](/partner/develop/referral-resources#referralstatus)|Actief
Partnerverwijzingssubstatus|Yes|Geeft de exacte status van de deal aan. Gebruik **Geaccepteerd** als u een nieuwe deal probeert te maken. Dit is ook vereist als u een bestaande verwijzing wijzigt. Geaccepteerde waarden worden hier [beschreven.](/partner/develop/referral-resources#referralsubstatus)|Geaccepteerd
Verwijzingsstatus van Microsoft|Hangt|Geeft de status aan van de aanvraag voor co-verkoop die u naar Microsoft hebt verzonden om hulp te vragen. Dit is een alleen-lezen veld. Elke wijziging die in dit veld is aangebracht tijdens het importeren van de gegevens, wordt genegeerd.| In behandeling
Afgewezen/verloren reden|Hangt| U hoeft deze informatie alleen op te geven als u de substatus van uw veld wilt wijzigen in Geweigerd of Verloren. U kunt deze kolom anders negeren. <br/> **Voer een getal in op basis van de onderstaande opties** <br/><br/> **1**- Project budget is niet voldoende  <br/> **2**- De klant heeft niet gereageerd  <br/> **3**- De klant heeft een andere leverancier gekozen  <br/> **4** - Niet voldaan aan klantvereisten  <br/> **5** - Geen klant <br/> **6**- Voorgestelde tijdlijn was te kort <br/> **7** - Rapporteren als misbruik, spam of phishing <br/> **8** - Overige |6|
Verkoopfase|No|Dit is het veld om de gedetailleerde verkoopfase van de verwijzing aan te geven. Lees hier meer over [verkoopfasen](./manage-co-sell-opportunities.md)|40
Geschatte waarde deal|Yes|De waarde van de deal op basis van de eerste gesprekken met de klant. Dit kan worden gewijzigd totdat de deal een van de terminale staten heeft bereikt die **zijn gewonnen** of **verloren.**|12563
Valuta|Yes|De valuta waarin de dealwaarde wordt ingevoerd. U vindt de valutacodes [hier.](https://en.wikipedia.org/wiki/ISO_4217)|USD
Geschatte einddatum|Yes|De geschatte einddatum van de deal op basis van de initiële gesprekken met de klant in de indeling MM/DD/YYYY. <br/> **De datum moet in de UTC-tijdzone zijn. Alle datums die in de gebruikersinterface Partner Center worden weergegeven, zijn gebaseerd op gelokaliseerde tijdzones. Er is mogelijk een verschil van +/- één dag in de gebruikersinterface Partner Center als u de verwijzing ziet waarvoor u de datum hebt opgegeven in de UTC-tijdzone.**|1/30/2020
CRM-id|No|Id van deze specifieke verwijzing in uw CRM-systeem, indien van deze. Dit is een veld voor tekstinvoer in vrije vorm.|34234324-sdfsdf-345345-sfd
Marketingcampagne-id|No|Dit veld geeft de marketingcampagne aan, wat heeft geleid tot deze specifieke verwijzing. Wordt doorgaans gebruikt voor de berekening van het rendement|BingSummer2020
Notities|No|Gedetailleerde notities die de updates met betrekking tot de verwijzing aangeven|Dit is een voorbeeld van een opmerking
Microsoft-hulp vereist?|Yes|Dit is om aan te geven of u wilt dat Microsoft u helpt bij het maken van deze aanvraag voor co-verkoop|Yes
Welke specifieke hulp van Microsoft?|Hangt|Een van de zes verschillende manieren waarop Microsoft u kan helpen. Dit is alleen van toepassing als u Ja kiest voor de vraag 'Microsoft Help vereist? " <br/> **Voer een getal in op basis van de onderstaande opties** <br/><br/> **1**- Workload - specifieke waardepropositie  <br/> **2**- Technische architectuur van de klant  <br/> **3**- Proof of concept /Demo  <br/> **4**- Aanhalingstekens en licenties  <br/> **5**- Posten - verkoopklant geslaagd  <br/> **6**- Algemeen of anders|1|
Delen met microsoft-verkoopteam|Yes|Dit is om aan te geven of u de details van de deal wilt delen met het verkoopteam van Microsoft. Dit is alleen van toepassing als u Nee kiest voor de vraag 'Microsoft Help vereist? "|Yes
Opmerkingen bij Microsoft|No|Eventuele specifieke opmerkingen bij Microsoft als u hulp van Microsoft nodig hebt|Hulp nodig met een POC voor Contoso-klant
Toestemming voor het delen van de contactpersoon van de klant/partner|Yes|Toestemming geven voor het delen van contactgegevens van klanten en de contactgegevens van de werknemers van uw bedrijf die aan de deal werken. **Deals worden niet gemaakt of bijgewerkt als u Nee kiest voor deze kolom.** |Yes
CLA-nummer|Hangt|CLA-nummer is niet vereist bij het maken of bijwerken van een IOT-deal. Dit wordt vereist wanneer u naar de win-fase van het ontwerp gaat.
Apparaatcategorie|No|Lijst met alle IoT-apparaatcategorieën. Selecteer een categorie uit de onderstaande opties <br>Apparaat voor het gamen van consumenten <br> Geldautomaat <br> Auto& transportsystemen <br> Azure Sphere Board<br> Azure Sphere Component <br> Azure Sphere Guardian<br> Azure Sphere Module <br> Automatisering bouwen<br> Apparaat voor gaming <br> Communicatieapparaten<br> Internetapparaat voor consumenten <br> Wearable voor consumenten<br> Digitaal fotoframe <br> Digital Signage <br> Gateway <br> HHT/Mobile<br> Industrial Automation Device<br> Tablet in de branche (niet-POS) <br> Kiosk<br> Media Player<br> Mediaapparaat <br> Mobile POS <br> Navigatieapparaat<br> Netwerkprojector<br> Anders<br> Ander bankapparaat<br> Ander elektronisch apparaat voor consumenten<br> Ander apparaat<br> Ander enterprise-apparaat<br>  Andere sensor/knooppunt <br> Verkooppuntapparaat<br> Apparaat afdrukken <br> Beveiliging/bewaking <br>  Server<br> Set-Top Box<br> Smart TV <br> Test- en meetapparaat<br> Thin Client-apparaat <br/>
Silicon Type|No|Voer de gegevens van het Chipset-model in door een optie in de onderstaande lijst te selecteren <br> AMD - A10 <br> AMD - A4 <br> AMD - A6 <br> AMD - A8 <br> AMD - E2 <br> AMD - FX 7500 <br> AMD - FX 7600P <br> AMD - FX 9370 <br> AMD - FX 9590 <br> AMD - G-serie <br> AMD - overige <br> AMD - R-serie <br> AMD - Rest van FX-modellen <br> Intel - Atom <br> Intel - Celeron - N1900 <br> Intel - Celeron - N2807 <br> Intel - Celeron - N2930 <br> Intel - Celeron - N3060 <br> Intel - Celeron - N3160 <br> Intel - Core i3 <br> Intel - Core i5 <br> Intel - Core i7 <br> Intel - Core M <br> Intel - Overige <br> Intel - Pentium <br> Intel - Rest van Celeron <br> Intel - XEON <br> MediaTek MT3620 <br> NXP 8ULP-CS <br> Andere <br/>
Azure Certified Device|No|Dit is om aan te geven of de Azure-compatibiliteitscertificering is bereikt voor het apparaat
Services koppelen|No|Dit is om aan te geven of de Azure-services tijdens de implementatie moeten worden gebundeld met de IoT-oplossing
Microsoft MSX-id|No|Id van een deal op het Microsoft MSX-systeem, alleen beschikbaar voor verkoopkansen
Gemigreerde PSC-deal-id|No|PSC-deal-id, alleen beschikbaar voor een deal die is gemigreerd van PSC naar pc
MPN-id|No|MPN-id van de organisatie waarvoor de kansen voor co-verkoop worden gemaakt
Oplossing 1|Yes|Oplossings-id (vereist), De valuta (optioneel) waarin de dealwaarde wordt ingevoerd. U vindt de [valutacodes](https://en.wikipedia.org/wiki/ISO_4217), prijs van de SKU (optioneel) en Hoeveelheid van de SKU (optioneel)  |SOL-1234-PQRS, USD, 10, 100
Teamlid 1|Yes|Voornaam, Achternaam, mobiel nummer en e-mail-id van het respectieve teamlid.| Bob, Partner, 999999, Bob.partner@Contoso.com
Microsoft-teamlid 1|No|Voornaam, Achternaam, mobiel nummer en e-mail-id van het respectieve teamlid van Microsoft dat aan de verkoopkans voor de co-verkoop werkt.| Sam, Verkoper, 999999, Sam.seller@Microsoft.com

## <a name="next-steps"></a>Volgende stappen

U kunt deze Partner Center connectors voor co-verkoop gebruiken om samen met Microsoft te verkopen vanuit uw CRM-systemen.

- [Connector voor co-verkoop voor Dynamics 365 CRM – Overzicht](connector-dynamics.md)
- [Connector voor co-verkoop voor Salesforce CRM - overzicht](connector-salesforce.md)

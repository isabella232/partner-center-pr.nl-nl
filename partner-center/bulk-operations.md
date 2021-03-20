---
title: Bulksgewijs exporteren en verkoop kansen importeren via Excel/CSV-bestanden in verwijzingen
description: Meer informatie over het downloaden, maken of bijwerken van verkoop kansen met Excel (CSV)-bestanden in het partner centrum
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 39a1370ad4e5da9120c74b46dfb0c20cd93df4e3
ms.sourcegitcommit: e8e8362d2777d25efac3e1076af5939765ed13d0
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/20/2021
ms.locfileid: "104712186"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-value-csv-files"></a>Bulk bewerkingen voor verkoop kansen met bestanden met door komma's gescheiden waarden (CSV)

**Juiste rollen**

- Beheerder van verwijzingen
- Referenties gebruiker

Bulk bewerkingen in het partner centrum helpen uw bedrijf bij het exporteren en importeren van gegevens over de verkoop kansen. Ga naar de pagina **verkoop kansen** om de koppelingen **importeren** en **exporteren** in de rechter bovenhoek van het vaandel met de pagina titel te vinden. Gebruikers met de machtigingen **beheerder** en **verwijzingen** van verwijzingen kunnen deze functionaliteit gebruiken.

> [!IMPORTANT]
> De acties voor maken/bijwerken die worden uitgevoerd via bulk import, kunnen niet onomkeerbaar zijn. Wees voorzichtig wanneer u een groot aantal records wijzigt of maakt. Er kan alleen een subset van velden worden gewijzigd na het maken van een deal. **Er zijn geen acties toegestaan zodra een van de deals een Terminal status bereikt zoals geweigerd/verlopen/gewonnen/verloren.**

## <a name="export-co-sell-opportunities"></a>Verkoop kansen exporteren

De volgende informatie beschrijft de export functionaliteit:

- U kunt **Maxi maal 5000 records** exporteren door te klikken op de knop **exporteren** .
- De deals die worden gedownload, zijn gebaseerd op uw toegangs niveaus. Verwijzings beheerders en verwijzings gebruikers kunnen verschillende resultaten krijgen op basis van hun bereik en worden opgenomen als team leden in de deals. Meer informatie over [machtigingen voor verwijzingen](permissions-overview.md#manage-referrals).
- De functie exporteren neemt het huidige tabblad op op de pagina verkoop kansen en de filters die zijn toegepast.
- Een CSV-bestand met alle gegevens op basis van de toegepaste filters worden gegenereerd.
- Het kan een minuut duren voordat de records zijn gedownload.
- U hoeft niet te wachten totdat de download actie is voltooid. Zelfs als u naar andere pagina's in het partner centrum navigeert, wordt het bestand gedownload zodra de export functie is voltooid.
- U kunt het gedownloade bestand opnieuw gebruiken om de details van de deal te wijzigen en te uploaden om alle records bij te werken.

## <a name="import-co-sell-opportunities"></a>Verkoop kansen importeren

- U kunt **Maxi maal 1000 records** maken of bijwerken met behulp van de import functionaliteit.
- U kunt de sjabloon helemaal zelf bouwen door de sjabloon te downloaden van de pagina importeren in Partner Center.
- U kunt ook de export functionaliteit gebruiken om de bestaande records te downloaden en ze bij te werken.
- Als het bestand meer dan 1000 records bevat, kan het niet worden verwerkt.
- Wanneer het bestand wordt verwerkt, wordt een samen vatting met het aantal verwijzingen dat is gemaakt, bijgewerkt en niet verwerkt, weer gegeven in de laatste proces bestands kaart.
- U kunt de details van de verwerkte records downloaden, eventuele fouten herstellen en hetzelfde bestand uploaden om de records te maken of bij te werken die in de vorige uitvoering zijn mislukt. **Verwijder alle geslaagde records uit het bestand voordat u de gecorrigeerde records uploadt die zijn mislukt tijdens de vorige uitvoering.**
- Als u meer oplossingen wilt toevoegen, voegt u extra kolommen naast oplossing 1 toe en gebruikt u de naam van de kolom als oplossing X, waarbij X het nummer van de oplossing in de deal aangeeft. Bijvoorbeeld oplossing 2, oplossing 3.
- U kunt Maxi maal 50 oplossingen aan een deal toevoegen.
- Als u meer team leden wilt toevoegen, voegt u extra kolommen toe naast team lid 1 en gebruikt u de kolom naam als teamlid, waarbij X staat voor het nummer van het teamlid in de deal. Bijvoorbeeld team lid 2, team lid 3.
- U kunt Maxi maal 50 team leden aan een deal toevoegen.

> [!NOTE]
> U hoeft niet te wachten totdat de verwerking is voltooid. De details van het laatst verwerkte bestand kunnen worden gedownload zodra de verwerking is voltooid. **Het kan Maxi maal tien minuten duren als u bestanden met 1000 records uploadt.**

> [!IMPORTANT]
> Lees alle instructies aandachtig door en controleer de indeling van elke kolom in de tabel hieronder voordat u deals maakt of bijwerkt met behulp van CSV-bestanden in het partner centrum.

|**Kolomnaam**|**Is verplicht?**|**Beschrijving**|**Voorbeeld waarde (n)**|
|-----|:-----|:---------|:---|
Fouten|Nee|Er worden fouten weer gegeven als er een fout is opgetreden met betrekking tot de maken/bijwerken-bewerkingen w. r. t met de verwijzingen in deze kolom. Als er meerdere fouten zijn, worden deze weer gegeven gescheiden door een punt komma.|Verplicht veld oplossing 1 ontbreekt|
Betrokkenheid-ID|Nee|De betrokkenheid-ID wordt gegenereerd door het micro soft Partner Center referrals-systeem. Niet vereist voor het maken van nieuwe verwijzingen. U kunt de bestaande betrokkenheid-ID gebruiken als u een record bijwerkt.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
Verwijzings-id|Nee|Verwijzings-ID wordt gegenereerd door het micro soft Partner Center referrals-systeem. Niet vereist voor het maken van nieuwe verwijzingen. Vul het met de verwijzings-ID in als u een bestaande record bijwerkt.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Naam van deal|Ja|De beschrijvende naam voor de deal van uw referentie.|Voor jaar van UK
Naam van klant|Ja|De naam van het bedrijf van de klant. Gebruik de juridische naam van de organisatie voor een snelle afstemming aan de kant van micro soft.|Contoso Corporation
Adres regel 1 van klant|Ja|Adres regel 1 van het bedrijf van de klant. |Eén contoso-manier
Adres regel 2 van klant|Nee|Adres regel 2 van het bedrijf van de klant.|NE 148 straat
Klant plaats|Ja|De plaats waar de organisatie van de klant zich bevindt.|Redmond
Klant status|Nee|De status waarin de klant organisatie zich bevindt.|Washington
Post code van de klant|Nee|Post code van de regio waar de organisatie van de klant zich bevindt.|98052
Klant land|Ja|Het land of de regio waar de organisatie van de klant zich bevindt. Gebruik de land codes van twee letters, zoals [hier]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes)wordt vermeld.|VS
D-U-N-S-ID van klant|Nee|Probeer de DUNS-ID van de organisatie van de klant op te halen. Dit helpt bij een snellere afstemming van de klant organisatie aan de kant van micro soft, die een snellere toewijzing van de verkoper kan worden. U kunt een DUNS-ID gratis ophalen van deze [website](https://www.dnb.com/duns-number/lookup.html).|81466849
Voor naam van klant contact persoon|Is afhankelijk van|De voor naam is alleen verplicht als u micro soft Help nodig hebt. De voor naam van de primaire contact persoon van de organisatie van de klant die aan deze deal werkt.|Jan
Achternaam van klant contact persoon|Is afhankelijk van|De achternaam is alleen verplicht als u micro soft Help nodig hebt. De achternaam van de primaire contact persoon van de organisatie van de klant die aan deze deal werkt.|Klant
Telefoon nummer van contact persoon klant|Is afhankelijk van|Het telefoon nummer is alleen vereist als u micro soft Help nodig hebt. Het telefoon nummer van de primaire contact persoon van de organisatie van de klant die aan deze deal werkt.|9999999999
E-mail adres contact persoon klant|Is afhankelijk van|E-mail adres is alleen vereist als u micro soft Help nodig hebt. Het e-mail adres van de primaire contact persoon van de organisatie van de klant die aan deze deal werkt.|john.customer@contoso.com
Referentie status partner|Ja|Geeft de status van de deal van het perspectief van uw bedrijf aan. Vereist als u probeert een verwijzing te maken of te wijzigen. Gebruik **nieuwe** als u probeert een nieuwe deal te maken. Geaccepteerde waarden worden [hier](/partner/develop/referral-resources#referralstatus)beschreven.|Actief
Substatus partner referentie|Ja|Hiermee wordt de exacte status van de deal aangegeven. Gebruik **geaccepteerd** als u een nieuwe deal wilt maken. Het is ook vereist als u een bestaande verwijzing wijzigt. Geaccepteerde waarden worden [hier](/partner/develop/referral-resources#referralsubstatus)beschreven.|Geaccepteerd
Micro soft Referral-status|Is afhankelijk van|Hiermee wordt de status van de aanvraag voor samen verkoop aangegeven die u hebt verzonden naar micro soft zoeken naar hulp. Dit is een alleen-lezen veld. Wijzigingen die in dit veld zijn aangebracht tijdens het importeren van de gegevens, worden genegeerd.| In behandeling
Reden afgewezen/verloren|Is afhankelijk van| U moet deze informatie alleen opgeven als u de substatus van uw veld wijzigt in geweigerd of verloren. U kunt deze kolom anders negeren. <br/> **Voer een getal in dat is gebaseerd op de onderstaande opties** <br/><br/> **1**-project budget is niet voldoende  <br/> **2**-de klant heeft niet gereageerd  <br/> **3**-klant heeft een andere leverancier gekozen  <br/> **4** -niet voldaan aan de vereisten van de klant  <br/> **5** -geen klant <br/> **6**-voorgestelde tijd regel is te kort <br/> **7** -rapporteren als misbruik, ongewenste e-mail of phishing <br/> **8** -andere |6|
Verkoopfase|Nee|Dit is het veld om de gedetailleerde verkoop fase van de verwijzing aan te geven. Lees [hier](./manage-co-sell-opportunities.md) meer over verkoop stadia|40
Geschatte deal waarde|Ja|"De waarde van de deal op basis van de eerste gesp rekken met de klant. Dit kan worden gewijzigd totdat de deal een van de statussen van de Terminal bereikt| gewonnen of verloren. '|12563
Valuta|Ja|De valuta waarin de deal waarde wordt ingevoerd. U kunt [hier](https://en.wikipedia.org/wiki/ISO_4217)de valuta codes vinden.|USD
Geschatte Sluitings datum|Ja|De geschatte Sluitings datum van de deal op basis van de eerste gesp rekken met de klant in de notatie MM/DD/JJJJ. <br/> **De datum moet in UTC-tijd zone zijn. Alle datums die worden weer gegeven in de gebruikers interface van het partner centrum zijn gebaseerd op gelokaliseerde tijd zones. In de gebruikers interface van het partner centrum is er mogelijk een verschil van +/-dag als u de verwijzing bekijkt waarvoor u de datum in UTC-tijd zone hebt opgegeven.**|1/30/2020
CRM-ID|Nee|Id van deze specifieke verwijzing in uw CRM-systeem, indien van toepassing. Dit is een invoer veld voor tekst in een vrije vorm.|34234324-sdfsdf-345345-SFD
Marketing campagne-ID|Nee|Dit veld geeft aan op welke marketing campagne is geresulteerd in deze specifieke verwijzing. Normaal gesp roken gebruikt voor berekening van de ROI|BingSummer2020
Notities|Nee|Gedetailleerde opmerkingen die de updates met betrekking tot de verwijzing aangeven|Dit is een voor beeld van een opmerking
Is micro soft Help vereist?|Ja|Dit is om aan te geven of u wilt dat micro soft u helpt bij het maken van deze mede koop-aanvraag|Ja
Welke specifieke hulp van micro soft?|Is afhankelijk van|Een van de zes verschillende manieren waarop micro soft u kan helpen. Dit is alleen van toepassing als u Ja kiest voor de vraag ' micro soft Help vereist? " <br/> **Voer een getal in dat is gebaseerd op de onderstaande opties** <br/><br/> **1**-specifiek toegevoegde waarde voor de werk belasting  <br/> **2**-technische architectuur van de klant  <br/> **3**-testen van concept/demo  <br/> **4**-offertes en licenties  <br/> **5**-verkoop succes van de klant  <br/> **6**-algemeen of ander|1|
Delen met het micro soft-verkoop team|Ja|Dit is om aan te geven of u de details van de deal wilt delen met het micro soft-verkoop team of niet. Dit geldt alleen als u Nee kiest voor de vraag ' micro soft Help vereist? "|Ja
Opmerkingen bij micro soft|Nee|Eventuele specifieke opmerkingen bij micro soft als u hulp nodig hebt van micro soft|Hulp nodig bij een haalbaarheids test voor contoso-klanten
Toestemming voor het delen van contact persoon van klant/partner|Ja|Toestemming om contact gegevens van klanten te delen en uw werk nemers van uw bedrijf contact opnemen met gegevens die aan de deal werken. **Er worden geen deals gemaakt of bijgewerkt als u Nee kiest voor deze kolom.** |Ja
Oplossing 1|Ja|Oplossings-ID (vereist), de valuta (optioneel) waarin de deal waarde is ingevoerd. U kunt [hier](https://en.wikipedia.org/wiki/ISO_4217)de valuta codes vinden, de prijs van de SKU (optioneel) en de hoeveelheid van de SKU (optioneel)  |SOL-1234-PQRS, USD, 10, 100
Team lid 1|Ja|De voor naam, achternaam, het mobiele nummer en de e-mail-ID van het betrokken teamlid.| Bob, partner, 999999, Bob.partner@Contoso.com

## <a name="next-steps"></a>Volgende stappen

U kunt deze connectors voor partner Centers gebruiken om te verkopen met micro soft vanuit uw CRM-systemen.

- [Connector voor Dynamics 365-overzicht co-sell](connector-dynamics.md)
- [Connector voor Sales Force-verkoop-overzicht](connector-salesforce.md)

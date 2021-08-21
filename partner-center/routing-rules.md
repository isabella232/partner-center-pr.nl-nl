---
title: Regels voor routering van binnenkomende verkoopkansen maken en beheren
ms.topic: article
ms.date: 08/20/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Uw bedrijf kan regels maken om te bepalen hoe een binnenkomende verkoopkans van Microsoft-verkopers wordt doorgeleid.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: efb76953b05bfb10a18657155349e267ee84f456
ms.sourcegitcommit: 42238e2ce36725631f542887c9112593d701ca9c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/20/2021
ms.locfileid: "122621702"
---
# <a name="create-and-manage-inbound-opportunities-routing-rules"></a>Regels voor routering van binnenkomende verkoopkansen maken en beheren

**Juiste rollen:** Beheerdersrollen voor verwijzingen | Verwijzingsgebruiker

> [!IMPORTANT]
> **Het maken van routeringsregels is optioneel.** Het wordt alleen aanbevolen voor grotere bedrijven met aanwezigheid over de hele wereld of als uw bedrijf een complexe MPN-hiërarchie heeft waarin verwijzingsbeheer moet worden uitgevoerd op een specifiek locatieniveau op basis van de klantmarkt en oplossingen.

## <a name="introduction"></a>Introductie

De functionaliteit die in dit document wordt beschreven, helpt uw bedrijf bij het configureren van regels, waarmee de verkoopkansen voor co-verkoop die door Microsoft-verkopers worden verzonden, kunnen worden doorgestuurd naar de MPN-locaties van uw keuze. Standaard worden de verwijzingen van de Microsoft-verkoper verzonden naar de MPN-locatie die is gekoppeld aan de oplossing voor co-verkoop die is opgenomen in de verkoopkans. De routeringsregels die worden gemaakt, helpen uw bedrijf om de standaardroutering te overschrijven. Alleen [**verwijzingsbeheerders**](permissions-overview.md#manage-referrals) met het hele organisatiebereik kunnen routeringsregels maken en bewerken. Partners met [**de gebruikersrol Verwijzing**](permissions-overview.md#manage-referrals) kunnen alleen de routeringsregels bekijken om te begrijpen hoe verwijzingen binnen hun bedrijf worden gerouteerd.

De regels worden niet achteraf toegepast. Verwijzingen die in het verleden of met een oudere configuratie van de routeringsregel zijn gemaakt, worden niet bijgewerkt. Wijzigingen in de regels zijn onmiddellijk van toepassing.

Er zijn drie hoofd pivots voor elke regel.

- **Klantmarkt:** de markt waar het klantbedrijf zich bevindt

- **Oplossing:** oplossingen die door uw bedrijf zijn gepubliceerd via de OCP GTM-portal of commerciële marketplace

- **MPN-locatie:** de MPN-locatie waarop de verwijzing moet worden doorgeleid

Elke regel kan worden gelezen als : voor de verwijzingen die worden verzonden door Microsoft-verkopers met de oplossing(en) van mijn bedrijf, stuurt u deze naar deze **MPN-locatie**

> [!Note]
> Regels voor binnenkomende routering zijn alleen van toepassing op verkoopkansen die door Microsoft-verkopers naar uw bedrijf worden verzonden.

## <a name="navigation"></a>Navigatie

U kunt routeringsregels maken op **het tabblad Verwijzingen** op de pagina **Accountinstellingen.** Als u naar de pagina wilt navigeren, selecteert u het instellingenpictogram  naast het gebruikerspictogram in de rechterbovenhoek en selecteert u vervolgens het tabblad Verwijzingen in het linkernavigatievenster.

## <a name="initial-setup"></a>Eerste configuratie

**Het configureren van routeringsregels is niet verplicht.** Als uw bedrijf besluit de routeringsregels te gebruiken om te profiteren van de routeringslogica, kunt u beginnen met het importeren van de standaardregels die het verwijzingsbeheersysteem gebruikt om de verwijzingen te routeren. De huidige logica maakt gebruik van de MPN-id die is gekoppeld aan de oplossing om alle inkomende verwijzingen van Microsoft-verkopers door te verwijzen, ongeacht het land van de klant. Ze zijn beschikbaar voor uw referentie en **kunnen met één** klik als routeringsregels worden geïmporteerd. Zodra de importactie is voltooid, worden de regels toegepast voor alle nieuwe verwijzingen die door Microsoft-verkopers zijn verzonden. Uw bedrijf kan bestaande regels bewerken of verwijderen en zo nodig nieuwe regels maken. Alleen [**verwijzingsbeheerders**](permissions-overview.md#manage-referrals) met het globale bereik kunnen de regels importeren. Dezelfde machtiging is vereist voor alle volgende wijzigingen in de regels voor doorsturen.

> [!IMPORTANT]
> **Er zijn wijzigingen in de logica voor e-mailmeldingen.** Zodra de regels zijn geïmporteerd, worden de e-mailberichten die eerder zijn verzonden naar contactpersonen voor oplossingen die zijn geüpload op het tabblad Co-sell in de commerciële marketplace, niet meer verzonden.  **Alleen [verwijzingsbeheerders van](permissions-overview.md#manage-referrals)** de MPN-locatie waar de verkoopkans voor co-verkoop wordt verzonden, worden hiervan op de hoogte gesteld.

## <a name="override-rules"></a>Regels overschrijven

U kunt twee typen regels overschrijven en een specifieke voorwaarde van de standaardregel overschrijven. In de standaardregel kunt u alleen de MPN-locatie wijzigen waar de verwijzingen naar moeten worden gerouteerd. De andere twee regeltypen die u kunt  overschrijven, zijn die met Alle oplossingen en **Alle markten** als voorwaarden in de regels.

**Alle markten overschrijven** : ervan uitgaande dat u een regel hebt gemaakt met de melding dat de verwijzingen voor alle markten van klanten en een bepaalde oplossing A naar MPN-locatie M1 worden doorgeleid. U kunt een dergelijke regel overschrijven met een specifieke markt en dezelfde oplossingscombinatie. Een voorbeeld van overschrijven kan zijn ' voor de verwijzingen met klanten van de markt Verenigd Koninkrijk en oplossing A, routeer deze naar MPN-locatie M2.

**Alle oplossingen overschrijven** - Ervan uitgaande dat u een regel hebt gemaakt met de melding dat voor alle oplossingen en een bepaalde markt MKT1 de verwijzingen naar mpn-locatie M1 worden doorgeleid. U kunt een dergelijke regel overschrijven met een specifieke oplossing en dezelfde marktcombinatie. Een voorbeeld van overschrijven kan zijn : 'voor de verwijzingen met klanten van de markt MKT1 en oplossing B, routeer deze naar MPN-locatie M2.

In de onderstaande tabel ziet u een overzicht van de typen oplossingen die u kunt overschrijven

| **Type** | **Kunt u overschrijven?** |
|-------|-------|
|Standaard| No |
|Alle markten| Yes|
|Alle oplossingen| Yes|
|Een specifieke combinatie van een of meer oplossingen en specifieke markt(en)| No|

> [!Note]
> U kunt de MPN-locatie voor de standaardregel wijzigen, ook al kunt u niets anders in die regel wijzigen.

## <a name="rules-evaluation"></a>Evaluatie van regels

Als uw bedrijf meerdere regels heeft die kunnen worden toegepast voor een scenario, onder de gebruikte evaluatiecriteria.

- De eerste controle is voor een regel met de specifieke combinatie van oplossing en markt, die zich in de binnenkomende kans voor komend verkeer. Een rechtstreekse overeenkomst met een dergelijke regel heeft voorrang op alle andere regels.
- Als de eerste controle mislukt, controleren we of er regels zijn die de oplossing bevatten die worden vermeld in de verwijzing met de marktvoorwaarde ingesteld als alle markten.
- Als de tweede controle mislukt, controleren we of er regels zijn waarin alle oplossingen worden vermeld als oplossingscriteria voor een specifieke markt.
- Als de derde controle ook mislukt, gebruiken we de standaardregel.

> [!Note]
> U kunt geen regel maken die in strijd is met andere regels op een specifieke locatie en oplossingsniveau. De gebruikersinterface geeft een foutmelding met de naam van de regel die conflicteert met uw configuratie als u probeert een conflicterende regel te maken.

## <a name="example"></a>Voorbeeld

Regels voor binnenkomende routering worden uitgelegd met behulp van routeringsregels die zijn gemaakt voor Contoso Corporation. Voordat u begrijpt hoe de regels worden toegepast, moeten we de MPN-hiërarchie en de gebruikersset-up bij Contoso Corporation begrijpen.

#### <a name="mpn-hierarchy-of-contoso-corporation"></a>MPN-hiërarchie van Contoso Corporation

| **MPN-id** | **Type** | **Adres** |
|-------|-------|-------|
|999999| Globaal| One Contoso way, **Redmond, Verenigde Staten of America**|
|555555| Locatie| One Contoso way, **Londen, Verenigd Koninkrijk**|
|666666| Locatie| One Contoso way, **Singapore, Singapore**|
|777777| Locatie| One Contoso way, **Bengalgalgal, India**|

#### <a name="sellers-from-contoso-corporation"></a>Verkopers van Contoso Corporation

Hieronder vindt u de verkopers met hun respectieve verwijzingsrollen en bereik bij Contoso Corporation.

| **Naam** | **Role** | **Scope** |
|-------|-------|-------|
|Verkoper 1|Verwijzingsbeheerder|Hele organisatie|
|Verkoper 2|Verwijzingsbeheerder|Bengaluru|
|Verkoper drie|Verwijzingsgebruiker|Londen|
|Verkoper vier|Verwijzingsgebruiker|Singapore|

#### <a name="inbound-routing-rules-for-contoso-corporation"></a>Regels voor binnenkomende routering voor Contoso Corporation

Stel dat de onderstaande set regels is gemaakt door Verkoper 1 voor Contoso Corporation. Alleen **verkoper 1** kan deze regels maken omdat [verwijzingsbeheerder](permissions-overview.md#manage-referrals) in het hele organisatiebereik is vereist voor het maken en bewerken van regels.

| **Markten** | **Oplossingen** | **MPN-locatie** | **Naam van routeringsregel** |
|-------|-------|-------|-------|
|Alle markten|Alle oplossingen|Redmond|Standaard|
|Verenigd Koninkrijk|Alle oplossingen|Londen|UK alle oplossingen|
|Alle markten|Sol-ABC|Singapore|Sol-ABC: alle markten|
|India|Sol-PQR|Bengaluru|India-Sol-PQR|

#### <a name="summary-of-routing-for-various-scenarios-based-on-the-rules-for-contoso-corporation"></a>Samenvatting van routering voor verschillende scenario's op basis van de regels voor Contoso Corporation

| **Nee** | **Scenario** | **Klantmarkt** | **Opgenomen oplossingen** |**Regel voor doorsturen toegepast** |**MPN-toewijzing** |**Toegang tot verwijzingen** |
|-----|----------|-------|-------|-------|-------|-----------|
| 1|Geen specifieke oplossing en marktregel overeen|Verenigd Koninkrijk|SOL-PQR|Globaal|999999| Verkoper 1, Verkoper 2, Verkoper drie (indien toegevoegd aan het team), Verkoper vier (indien toegevoegd aan het team)|
| 2|Alle oplossingen en een specifieke overeenkomst met een marktregel|Verenigd Koninkrijk|SOL-PQR|UK alle oplossingen|555555| Verkoper 1, Verkoper drie (indien toegevoegd aan het team) |
| 3|Specifieke oplossing en alle marktregel komen overeen|Nigeria|SOL-ABC|SOL-ABC alle markten|666666| Verkoper 1, Verkoper vier (indien toegevoegd aan het team) |
| 4|Overeenkomst tussen specifieke oplossing en marktregel|India|SOL-PQR|India-Sol-PQR|777777| Verkoper 1, verkoper 2|
| 5|Inkomende verwijzing met een oplossing die niet eigendom is van uw bedrijf|Verenigde Staten van Amerika|SOL-XYZ|Globaal|999999| Verkoper 1, Verkoper 2, Verkoper drie (indien toegevoegd aan het team), Verkoper vier (indien toegevoegd aan het team)|

## <a name="next-steps"></a>Volgende stappen

- [Kansen voor co-verkoop beheren](manage-co-sell-opportunities.md)

- [De connector voor co-verkoop voor Dynamics 365 CRM kopen](connector-dynamics.md)

- [De connector voor co-verkoop voor Salesforce CRM op halen](connector-salesforce.md)

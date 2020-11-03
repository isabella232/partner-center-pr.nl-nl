---
title: Aanbiedingen detecteren-commerciële Marketplace
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe CSP-partners partner centrum kunnen gebruiken om de Marketplace voor SaaS-aanbiedingen of prijzen van onafhankelijke software leveranciers (Isv's) te bekijken of te doorzoeken.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cb7b4ffdb4edf75e3e121e4ddea6b9de191ddbbf
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528569"
---
# <a name="discover-offers-and-pricing-in-the-partner-center-commercial-marketplace"></a>Aanbiedingen en prijzen ontdekken in het Partner Center-Commercial Marketplace

**Van toepassing op**

- Partnercentrum
- Partners in het CSP-programma

**Juiste rollen**

- Globale beheerder
- Beheer agent

Als onafhankelijke software leveranciers (Isv's) kiezen om een aanbieding in de commerciële Marketplace te publiceren, kunnen ze ook bepalen of de aanbieding beschikbaar moet worden gesteld in het CSP-programma. Als ze ervoor kiezen om de aanbieding via het CSP-programma te verkopen, moeten CSP-partners de aanbieding zien in het Marketplace-gebied van partner centrum.

Als een ISV-aanbieding niet wordt weer gegeven zoals u verwacht in het partner centrum, kan dat zijn door:

- De ISV heeft besloten de aanbieding niet via het CSP-programma te verkopen. Sommige ISV-producten kunnen bijvoorbeeld beschikbaar zijn gesteld in andere gebieden van de commerciële Marketplace (zoals in [Microsoft AppSource](https://appsource.microsoft.com/) en [Azure Marketplace](https://azuremarketplace.microsoft.com/)), maar worden mogelijk niet weer gegeven voor Csp's in het partner centrum Marketplace.

- De ISV heeft besloten de aanbieding exclusief te maken voor een select aantal CSP-partners. Zie verderop in dit Help-onderwerp voor meer informatie over exclusieve aanbiedingen.

- Het aanbiedings type kan mogelijk niet worden gebruikt door het partner centrum of Azure Portal (bijvoorbeeld containers of sommige op gebruik gebaseerde aanbiedingen).

- Het facturerings land van uw gekoppelde klant (s) wordt mogelijk niet ondersteund voor deze ISV-aanbieding.

## <a name="view-marketplace-offers-in-partner-center"></a>Marketplace-aanbiedingen weer geven in het partner centrum

Beschik bare commerciële Marketplace-aanbiedingen weer geven in het CSP-programma: 

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum en selecteer vervolgens **CSP** in het navigatie menu aan de linkerkant.

2. Selecteer **verkopen** , gevolgd door **Marketplace** . Standaard worden producten van alle typen en categorieën weer geven.

3. Selecteer een filter op type of categorie. U kunt ook **zoeken** gebruiken om specifieke tref woorden, namen van het aanbod of de namen van ISV-uitgevers te vinden.

4. Selecteer een specifieke product aanbieding in de lijst. Hiermee gaat u naar het tabblad product overzicht, waar u meer informatie over de aanbieding kunt vinden. De informatie op dit tabblad kan het volgende omvatten: 

    - Een beschrijving van het product of de aanbieding

    - Meer informatie over de ISV-Uitgever

    - Koppelingen naar documentatie of marketing materiaal dat is geüpload door de ISV-Uitgever

    - Andere mogelijke ISV-contact personen voor klant ondersteuning, technisch of contact persoon voor het CSP-programma

5. Als u meer informatie wilt weer geven over de beschik bare abonnementen, Sku's of prijzen van een aanbieding, selecteert u het tabblad **Abonnementen en prijzen** . Op dit tabblad wordt u weer gegeven:

    - De markten waar deze aanbieding voor u beschikbaar is

    - Een lijst met Sku's of abonnementen die beschikbaar zijn voor de aanbieding

    - Prijzen voor elke SKU of abonnement beschikbaar

## <a name="view-marketplace-offers-via-partner-center-apis"></a>Marketplace-aanbiedingen via partner Center-Api's weer geven

CSP-programma partners kunnen ook Api's gebruiken om een lijst met in aanmerking komende aanbiedingen te retour neren. In aanmerking komende aanbiedingen zijn alleen de SaaS-ISV-aanbiedingen die beschikbaar zijn voor de partner om te verkopen via de Marketplace van het partner centrum. Raadpleeg de richt lijnen voor het [verkrijgen van een lijst met aanbiedingen voor een markt](/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market)voor partners die gebruikmaken van api's voor het identificeren van aanbiedingen in de catalogus.

## <a name="view-the-latest-marketplace-offer-pricing-in-partner-center"></a>Bekijk de nieuwste prijzen voor Marketplace-aanbiedingen in het partner centrum

Volg deze stappen voor de meest recente prijs informatie die is gekoppeld aan een aanbieding:

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum en selecteer vervolgens **CSP** in het navigatie menu aan de linkerkant.

2. Selecteer **verkopen** , gevolgd door **prijzen en aanbiedingen** .

3. Schuif omlaag naar het gedeelte **Marketplace** , selecteer een locatie en down load **Marketplace-prijzen** . Hiermee genereert u een spread sheet met de nieuwste prijs gegevens voor SaaS, op licenties gebaseerde aanbiedingen die beschikbaar zijn via ISV-Publishers. Enkele prijzen voor Azure-toepassingen kunnen hier ook worden weer gegeven. Deze informatie wordt dagelijks bijgewerkt, zodat u deze kunt controleren op huidige prijzen, zo vaak als u wilt.

4. Als een ISV-product een gratis proef periode bevat, worden in het werk blad twee rijen weer gegeven voor dat product:

    - In één rij wordt de prijs van de gratis proef versie van nul weer gegeven. Dit betekent dat er een gratis proef periode beschikbaar is.

    - In de andere rij worden de prijs en de voor waarden weer gegeven die van toepassing zijn nadat de gratis proef periode is verstreken.

Als CSP-programma partner komt u mogelijk in aanmerking voor andere stimulansen die zijn gekoppeld aan bepaalde commerciële Marketplace-aanbiedingen. Voor meer informatie over andere stimulansen raadpleegt u de [CSP-prikkel handleiding](https://aka.ms/partnerincentives) (hiervoor is CSP-aanmelding vereist).

## <a name="learn-about-marketplace-exclusive-offers"></a>Meer informatie over aanbiedingen voor exclusieve Marketplace

Isv's hebben de mogelijkheid om hun aanbiedingen alleen beschikbaar te maken voor specifieke partners in het CSP-programma. Dit wordt een exclusieve aanbieding genoemd. Alle partners in het CSP-programma kunnen nog steeds alle ISV-aanbiedingen bekijken in de commerciële Marketplace van partner Center, inclusief de aanbiedingen die zijn gemarkeerd als Exclusive.

Als een aanbieding **niet** is gemarkeerd als exclusief, kunnen alle partners die aanbieding kopen (ervan uitgaande dat het factuur land van de geselecteerde klant overeenkomt met de land beschikbaarheid van de aanbieding van de ISV).

Voor elke aanbieding die exclusief is gemarkeerd, kunnen echter alleen de partners die door de ISV zijn geselecteerd, de aanbieding kopen.

> [!NOTE]
> Als u een aanbieding hebt gemarkeerd als exclusief die u wilt verkopen aan uw klanten, neemt u rechtstreeks contact op met de ISV en vraagt u om toestemming om de exclusieve aanbieding te verkopen. Wanneer u de details van een exclusieve aanbieding bekijkt, ziet u mogelijk een ISV-koppeling voor **contact personen** die u kunt selecteren.

Lees [Cloud Solution Providers](/azure/marketplace/cloud-solution-providers)voor meer informatie over de ISV-ervaring in de commerciële Marketplace.

Lees voor meer informatie over de CSP-ervaring in Marketplace het onderwerp [commerciële Marketplace-overzicht](csp-commercial-marketplace-overview.md).

## <a name="next-steps"></a>Volgende stappen

- [Commerciële Marketplace-aanbiedingen kopen](csp-commercial-marketplace-purchase.md)
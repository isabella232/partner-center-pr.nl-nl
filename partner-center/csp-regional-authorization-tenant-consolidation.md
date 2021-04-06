---
title: Tenant consolidatie CSP regionale autorisatie
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik deze instructies voor het consolideren van tenants voor verschillende landen/regio's. Dit omvat stappen voor het migreren van klant accounts en klant abonnementen.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: 2171e2b10101e99bdd8d415a936ba98af65c2a1b
ms.sourcegitcommit: 3d7d5064c5e021079ed7e6f93f03869cbf425a32
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106502567"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instructies voor tenantconsolidatie voor regionale autorisatie in CSP

**Van toepassing op**

- Partnercentrum voor Microsoft Cloud for US Government

**Juiste rollen**

- Globale beheerder
- Beheer agent

\[Sommige informatie is gekoppeld aan een vooraf vrijgegeven product dat ingrijpend kan worden gewijzigd voordat het commercieel wordt uitgebracht. Microsoft biedt geen enkele expliciete of impliciete garanties met betrekking tot de informatie die hier wordt verstrekt.\]

U kunt tenants voor uw bedrijf consolideren. Gebruik deze instructies voor het consolideren van tenants voor verschillende landen/regio's.

>[!NOTE]  
>U moet rekening houden met alle ingerichte abonnementen en het aantal licenties voor elk van uw klanten in het account dat u wilt overstappen. U kunt dezelfde exacte abonnementen met dezelfde licentie aantallen onder het nieuwe centrale CSP-account opnieuw inrichten als onderdeel van het migratie proces. Gebruik de functie lijst exporteren om een lijst met klanten te maken waarmee u naar de gecentraliseerde Tenant kunt gaan.  Zodra de consolidatie is voltooid, kunt u niet terugkeren naar de vorige Tenant status. De klant actie kan ook vereist zijn.

## <a name="prepare-for-migration"></a>Voorbereiden op migratie

- Meld u aan bij het **partner centrum**  met het **overgangs** account (het abonnement dat u wilt overstappen naar het nieuwe account) en Bekijk alle klanten en alle services die voor deze klanten zijn ingericht.

- Meld u af bij dit account.

## <a name="migrate-customer-accounts"></a>Klant accounts migreren

1. Meld u aan bij het **partner centrum**  met het **overgangs** -(nieuwe) account (het abonnement dat u aan klanten overstapt).

2. Selecteer **Klanten**.

3. Selecteer **een reseller-relatie aanvragen**. Er wordt een standaard e-mail bericht weer gegeven dat u naar uw klanten kunt verzenden. Dit bericht bevat een URL met de organisatie-ID die uniek is voor uw nieuwe partner Center-account.

4. **Actie van klant:** Zorg ervoor dat alle actieve klanten die u wilt migreren, deze URL bezoeken. Bij het openen van de URL wordt de klant gevraagd zich aan te melden bij de Office 365-Portal. De klant meldt zich aan met dezelfde organisatie-ID die ze gebruiken voor toegang tot de beheer portals van Azure en Office 365.

5. Nadat u zich hebt aangemeld, wordt de globale beheerder voor het **klant account** gevraagd om een overeenkomst in te dienen die gedelegeerde beheerders bevoegdheden aan het nieuwe CSP-account verleent. Als ze akkoord gaan, selecteert de klant het selectie vakje en gaat ermee akkoord de relatie te autoriseren.

De klanten worden weer gegeven in de klanten lijst van de partner nadat ze de overeenkomst één voor één hebben ingediend.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Office 365 en niet-Azure-op gebruik gebaseerde abonnementen migreren

1. Zodra uw klant de overeenkomst heeft ondertekend, kunt u hun abonnementen opnieuw maken onder uw gecentraliseerde partner-Tenant.

2. Selecteer **klanten** in het **partner centrum**.

3. Open de bedrijfs naam voor de klant die u wilt migreren.

4. Selecteer **abonnement toevoegen**.

5. Voeg de juiste abonnementen en licentie aantallen toe vanuit de catalogus. Controleer met de informatie in de **overgang van** partner accounts.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="klanten lijst":::

6. Selecteer **verzenden.**

   De services worden nu aan de klant door gegeven van de **overgang naar** het partner account.

7. Herhaal deze stappen om abonnementen voor alle extra klanten te migreren.

Voordat u doorgaat naar de volgende sectie, moet u ervoor zorgen dat alle abonnementen van klanten die zijn gemaakt onder de **overgang van** partner accounts, opnieuw worden ingericht onder de **overgang naar** het partner account.

> [!NOTE]
> Partners moeten abonnementen opschorten voor de **overgang van** het partner Tenant account in het partner centrum op dezelfde dag dat deze abonnementen worden overgezet en ingesteld onder de **overgang naar** het Tenant account van de partner in het partner centrum om ervoor te zorgen dat dubbele facturering niet wordt uitgevoerd. Ondersteunings aanvragen worden afgewezen als gevolg van een overlap ping in de facturering, waardoor de **overgang** van abonnementen niet correct wordt uitgeschakeld.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>De Office 365-abonnementen uitschakelen onder de overgang van partner-account

Als u het CSP-abonnement uitschakelt onder de **overgang van** partner accounts, wordt een toekomstige facturering stopgezet. U hoeft Azure-abonnementen niet hand matig uit te scha kelen, omdat Azure-abonnementen tijdens het migratie proces automatisch worden uitgeschakeld.

1. Meld u aan bij het **partner centrum** met de **overgang van** het CSP-account en navigeer naar de klanten lijst.

2. Open de klant met abonnementen om uit te scha kelen en selecteer vervolgens de eerste aanbieding die u wilt uitschakelen.

3. Stel het abonnement in op **opgeschort** en selecteer vervolgens **verzenden**.

   >[!Note]
   >Het onderbreken van het abonnement zorgt ervoor dat er geen dubbele facturering plaatsvindt.

   Het abonnement wordt **uitgesteld** weer gegeven in de lijst abonnementen.

4. Herhaal deze stappen voor alle abonnementen onder de klant. Zorg ervoor dat alle weer geven zijn **onderbroken.**

5. Selecteer de volgende klant in de lijst en herhaal het proces voor het uitschakelen van alle abonnementen.

## <a name="migrating-azure-usage-based-subscriptions"></a>Op Azure-gebruik gebaseerde abonnementen migreren

In tegens telling tot de Office 365 CSP-abonnementen, hoeven Azure CSP-abonnementen op basis van gebruik niet hand matig te worden gemigreerd. Met de ondersteuning van Microsoft Azure worden de Azure-abonnementen en alle geïmplementeerde Services of resources gemigreerd van de overschakeling **van** de CSP-reseller-accounts **naar de CSP** -reseller-account. Er is geen onderbreking van de service voor de klant tijdens deze overgang.

1. Zorg ervoor dat de klant accounts die Azure-abonnementen hebben gemigreerd, de overeenkomst hebben geaccepteerd om te koppelen aan de nieuwe **overgang naar** het CSP-account.

2. U ontvangt een melding van micro soft van welke klant accounts klaar zijn om te migreren, en bieden de bedrijfs namen van die klant.

3. Micro soft migreert de op Azure-gebruik gebaseerde abonnementen en brengt u op de hoogte wanneer de migratie is voltooid.

4. U moet bevestigen dat het Azure-abonnement onder de **overstap van** het CSP-reseller-account nu is gemarkeerd als **opgeschort** in het partner centrum in het gedeelte klant abonnementen.

5. Controleer of het Azure-abonnement onder de **overgang naar** het CSP-reseller-account nu de status **actief** in Partner Center weergeeft in het gedeelte klant abonnementen.

   >[!Note]
   > Het uitschakelen van de abonnementen onder de klant heeft geen invloed op de weer gave van de klant in de lijst klanten. Er is momenteel geen optie om klanten te verwijderen uit de lijst. Partners moeten voor komen dat abonnementen worden toegevoegd aan deze klanten via hun **overgang van** account in de toekomst.

6. Herhaal deze stappen voor alle abonnementen onder al uw klanten om toekomstige kosten te stoppen voor de **overgang van** een of meer accounts. De partner ontvangt één definitieve factuur met een tegoed voor het aantal ongebruikte dagen tussen de dag van de annulering en de laatste dag van de facturerings periode. Er worden geen toekomstige facturen gegenereerd na de laatste facturerings periode.

### <a name="additional-information"></a>Aanvullende informatie

- Het uitschakelen **van het abonnement van de CSP-** account heeft geen invloed op de service van de eind klant zolang de service is ingericht van de **overgang naar** het CSP-account voordat het abonnement is uitgeschakeld.

- Abonnementen kunnen niet worden gebruikt door de klant en er worden geen kosten in rekening gebracht wanneer deze zijn onderbroken of geannuleerd.

- Er is momenteel geen manier om een klant volledig uit de lijst met **klanten** te verwijderen.
- 
    >[!Note]
    > Partners moeten abonnementen opschorten voor de **overgang van** het partner Tenant account in het partner centrum op dezelfde dag dat deze abonnementen worden overgezet en ingesteld op basis van de **overgang naar** het account om ervoor te zorgen dat dubbele facturering niet wordt uitgevoerd. Micro soft biedt geen ondersteuning voor tegoed aanvragen als gevolg van een overlap ping in de facturering, waardoor de **overgang** van abonnementen naar opgeschort niet goed kan worden ingesteld.

### <a name="simplify-migration-using-export"></a>Migratie vereenvoudigen met exporteren

Met de **functie exporteren** kunt u de abonnementen vastleggen die u moet gebruiken in de nieuwe geconsolideerde structuur:

1. Selecteer **klanten** in het partner centrum om de lijst met klanten te bekijken. 

2. Open de naam van de gewenste klant.

3. Selecteer op de pagina **abonnementen** de optie **abonnementen exporteren** om de details van abonnementen te exporteren naar een Excel-bestand.

4. Gebruik deze lijst om de abonnementen in uw nieuwe geconsolideerde Tenant opnieuw te maken.

### <a name="api-registration"></a>API-registratie

Zie [API-toegang instellen in partner centrum](/partner-center/develop/set-up-api-access-in-partner-center)voor meer informatie over API-registratie.

## <a name="next-steps"></a>Volgende stappen

- [Cloud Solution Provider-programma regionale markten en valuta's waar u CSP-aanbiedingen kunt verkopen](regional-authorization-overview.md)

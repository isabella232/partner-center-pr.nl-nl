---
title: Regionale CSP-autorisatie tenantconsolidatie
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Gebruik deze instructies om tenants te consolideren voor verschillende landen/regio's. Dit omvat stappen voor het migreren van klantaccounts en klantabonnementen.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: f4df62bddba501552eafe2142f4c0656b8eefc7c
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957672"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instructies voor tenantconsolidatie voor regionale autorisatie in CSP

**Van toepassing op**: Partner Center | Partner Center voor Microsoft Cloud for US Government

**Juiste rollen:** globale | Beheeragent

\[Sommige informatie heeft betrekking op vooraf uitgebracht product dat aanzienlijk kan worden gewijzigd voordat het commercieel wordt uitgebracht. Microsoft biedt geen enkele expliciete of impliciete garanties met betrekking tot de informatie die hier wordt verstrekt.\]

U kunt tenants consolideren voor uw bedrijf. Gebruik deze instructies om tenants te consolideren voor verschillende landen/regio's.

>[!NOTE]  
>U moet rekening houden met alle inrichtende abonnementen en het aantal licenties voor elk van uw klanten in het account van waar u over overstapt. U gaat die exacte abonnementen met dezelfde licentietellingen opnieuw inrichten onder het nieuwe centrale CSP-account als onderdeel van het migratieproces. Gebruik de exportlijstfunctie om een lijst met klanten te maken om over te gaan naar de gecentraliseerde tenant.  Zodra de consolidatie is voltooid, kunt u de vorige tenanttoestand niet meer terugdraaien. De actie van de klant kan ook vereist zijn.

## <a name="prepare-for-migration"></a>Voorbereiden op migratie

- Meld u aan **Partner Center** met het overgangsaccount  (het account dat u wilt overstappen naar het nieuwe account) en bekijk alle klanten en alle services die voor deze klanten zijn ingericht.

- Meld u af bij dit account.

## <a name="migrate-customer-accounts"></a>Klantaccounts migreren

1. Meld u aan **Partner Center**  met **het** (nieuwe) overgangsaccount (het account waarin u klanten over wilt zetten).

2. Selecteer **Klanten**.

3. Selecteer **Een resellerrelatie aanvragen.** U krijgt een standaard-e-mailbericht te zien dat u naar uw klanten kunt verzenden. Dit bericht bevat een URL met de organisatie-id die uniek is voor uw nieuwe Partner Center account.

4. **Actie van de klant:** Zorg ervoor dat elk van de actieve klanten die u wilt migreren deze URL bezoekt. Bij het openen van de URL wordt de klant gevraagd zich aan te melden bij Office 365 portal. De klant meldt zich aan met dezelfde organisatie-id die hij gebruikt voor toegang tot de Azure- en Office 365-beheerportals.

5. Na het aanmelden wordt de  globale beheerder voor het klantaccount gevraagd een overeenkomst in te dienen die gedelegeerde beheerdersbevoegdheden voor het nieuwe CSP-account biedt. Als ze akkoord gaan, selecteert de klant het selectievakje en gaat ermee akkoord om de relatie te autor toestemming te geven.

De klanten worden weergegeven in de klantenlijst van de partner nadat ze de overeenkomst één voor één hebben ingediend.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migratie van Office 365- en niet-Azure-abonnementen op basis van gebruik

1. Zodra uw klant de overeenkomst heeft ondertekend, kunt u de abonnementen opnieuw maken onder uw gecentraliseerde partnerten tenant.

2. Selecteer **Partner Center**. 

3. Open de bedrijfsnaam voor de klant die u wilt migreren.

4. Selecteer **Abonnement toevoegen.**

5. Voeg de juiste abonnementen en het aantal licenties uit de catalogus toe. Controleer met de informatie in de **overgang van** partneraccounts.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="klantenlijst.":::

6. Selecteer **Verzenden.**

   De services worden nu aan de klant geleverd vanuit het **overgangsaccount naar** het partneraccount.

7. Herhaal deze stappen om abonnementen voor alle extra klanten te migreren.

Voordat u doorgaat met de volgende sectie,  moet u ervoor zorgen dat alle bestaande klantabonnementen onder De overgang van partneraccounts opnieuw worden ingericht onder overgang naar **partneraccount.**

> [!NOTE]
> Partners moeten abonnementen op het overstappen van het **partnerten** tenantaccount in Partner Center op dezelfde dag dat deze abonnementen worden overge zetten en ingesteld onder het overstappen naar **partnerten** tenantaccount in de Partner Center om ervoor te zorgen dat dubbele facturering niet wordt uitgevoerd. Ondersteuningsaanvragen worden geweigerd voor tegoeden vanwege overlapping in de facturering  die optreedt door het niet juist uitschakelen van de overgang van abonnementen.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>De Office 365 uitschakelen onder het partneraccount overstappen

Als u het CSP-abonnement onder De overgang **van** partneraccounts uit te stellen, worden toekomstige factureringen gestopt. U hoeft Azure-abonnementen niet handmatig uit te schakelen, omdat Azure-abonnementen automatisch worden uitgeschakeld tijdens het migratieproces.

1. Meld u aan bij **Partner Center** **CSP-account en** navigeer naar de lijst met klanten.

2. Open de klant met abonnementen die u wilt uitschakelen en selecteer vervolgens de eerste aanbieding die u wilt uitschakelen.

3. Stel het abonnement in op **tijdelijk en** selecteer **verzenden.**

   >[!Note]
   >Door het abonnement op te schorten, wordt dubbele facturering niet uitgevoerd.

   Het abonnement wordt **tijdelijk in de** lijst met abonnementen weergegeven.

4. Herhaal deze stappen voor alle abonnementen onder de klant. Controleer of alles is **opgeschort.**

5. Selecteer de volgende klant in de lijst en herhaal het proces van het uitschakelen van alle abonnementen.

## <a name="migrating-azure-usage-based-subscriptions"></a>Azure-abonnementen op basis van gebruik migreren

In tegenstelling Office 365 CSP-abonnementen hoeven op gebruik gebaseerde CSP-abonnementen niet handmatig te worden gemigreerd. Microsoft Azure Met ondersteuning worden de Azure-abonnementen en alle  geïmplementeerde services of resources gemigreerd van de overgang van CSP-reselleraccounts naar het overstappen naar het CSP-reselleraccount.  Er is geen onderbreking van de service voor de klant tijdens deze overgang.

1. Zorg ervoor dat de klantaccounts met gemigreerde Azure-abonnementen de overeenkomst hebben geaccepteerd om te worden gekoppeld aan het nieuwe **Overgang** naar CSP-account.

2. U stelt Microsoft op de hoogte van welke klantaccounts gereed zijn om te worden gemigreerd en geeft de bedrijfsnamen van die klanten op.

3. Microsoft migreert de azure-abonnementen op basis van gebruik en waarschuwt u wanneer de migratie is voltooid.

4. U moet controleren of het Azure-abonnement onder het **reselleraccount** Overstappen van CSP nu is gemarkeerd als tijdelijk Partner Center onder de sectie Klantabonnementen. 

5. Controleer of in het Azure-abonnement onder het reselleraccount  Overstappen naar **CSP** nu de status actief wordt Partner Center onder de sectie Klantabonnementen.

   >[!Note]
   > Het uitschakelen van de abonnementen onder de klant verandert niet het uiterlijk van de klant in de lijst Klanten. Er is momenteel geen optie om klanten uit de lijst te verwijderen. Partners moeten voorkomen dat ze in de toekomst abonnementen weer aan deze klanten toevoegen vanuit hun **overgangsaccount.**

6. Herhaal deze stappen voor alle abonnementen onder al uw klanten om toekomstige kosten voor de overgang van **een** of meer account(en) te stoppen. De partner ontvangt één definitieve factuur met een tegoed voor het aantal ongebruikte dagen tussen de dag van annulering en de laatste dag van de factureringsperiode. Er worden geen toekomstige facturen gegenereerd na die laatste factureringsperiode.

### <a name="additional-information"></a>Aanvullende informatie

- Het uitschakelen van het  abonnement uit het CSP-account heeft geen invloed op de service van de eindklant zolang de service is ingericht vanuit het overgangsaccount naar **het** CSP-account voordat het abonnement werd uitgeschreven.

- Abonnementen kunnen niet worden gebruikt door de klant en genereren geen kosten wanneer deze worden opgeschort of geannuleerd.

- Er is momenteel geen manier om een klant volledig te verwijderen uit de **lijst met** klanten.
- 
    >[!Note]
    > Partners moeten abonnementen op het overstappen van het **tenantaccount** van de partner in Partner Center op dezelfde dag dat deze abonnementen worden overgemaakt naar en ingesteld onder het overgangsaccount naar **account,** om ervoor te zorgen dat dubbele facturering niet wordt uitgevoerd. Microsoft biedt geen ondersteuning voor aanvragen voor tegoeden vanwege overlapping  in de facturering die optreedt door het niet juist instellen van de overgang Van abonnementen naar tijdelijk opgeschort.

### <a name="simplify-migration-using-export"></a>Migratie vereenvoudigen met behulp van Exporteren

Met de **functie Exporteren** kunt u de abonnementen vastleggen die u moet gebruiken in uw nieuwe geconsolideerde structuur:

1. Selecteer **Klanten** op Partner Center om de lijst met klanten weer te geven. 

2. Open de gewenste klantnaam.

3. Selecteer op **de pagina** Abonnementen de optie **Abonnementen** exporteren om details van abonnementen naar een Excel exporteren.

4. Gebruik deze lijst om de abonnementen in uw nieuwe geconsolideerde tenant opnieuw te maken.

### <a name="api-registration"></a>API-registratie

Zie API-toegang instellen in Partner Center voor meer informatie [over API Partner Center.](/partner-center/develop/set-up-api-access-in-partner-center)

## <a name="next-steps"></a>Volgende stappen

- [Cloud Solution Provider programma regionale markten en valuta's waar u CSP-aanbiedingen kunt verkopen](regional-authorization-overview.md)

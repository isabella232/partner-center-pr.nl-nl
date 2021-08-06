---
title: Een Azure-abonnement overdragen naar een andere partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Meer informatie over het wijzigen Cloud Solution Provider partner van het programma dat is gekoppeld aan de Azure-abonnementen van een klant.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/21/2021
ms.openlocfilehash: cac2d1443fd47f45a70729bf034e65f33861e73698633938ae196e274f4a382b
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115681379"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Meer informatie over het overdragen van Azure-abonnementen van een klant naar een andere partner

**Van toepassing op**: Partner Center | Partner Center voor Microsoft Cloud for US Government

**Juiste rollen:** globale beheerder

In dit artikel wordt beschreven hoe een klant zijn Microsoft Azure-services kan overstappen van de ene Cloud Solution Provider (CSP) naar de andere wanneer hij de vorige Azure-aanbieding in CSP heeft gekocht.

Na fase 1 van de wijzigingen die we aanbrengen in de vorige [Azure-aanbieding in CSP,](https://go.microsoft.com/fwlink/p/?linkid=2164140)kan de partner voor alle bestaande resellerrelaties tussen partners en klanten in het CSP-programma doorgaan met het uitvoeren van de vorige Azure-aanbieding (MS-AZR-0145p) als de klant deze al heeft aangeschaft. Voor alle bestaande resellerrelaties tussen partners en klanten kan de partner alleen de nieuwe Azure-aanbieding uitvoeren als de klant de vorige Azure-aanbieding niet eerder heeft gekocht.

- Als zowel de huidige als de toekomstige partner actieve vorige **Azure-aanbiedingsabonnementen** met een klant heeft, blijven de vorige Overdrachten van Azure-aanbieding (MS-AZR-0145p) die in dit document worden beschreven tussen de huidige en toekomstige partner beschikbaar na fase 1, zolang beide partners actieve abonnementen op eerdere Azure-aanbiedingsabonnementen behouden. Deze overdrachtsmogelijkheid zou eindigen wanneer een toekomstige partner geen actieve abonnementen meer heeft op eerdere Azure-aanbiedingsabonnementen of wanneer de vorige Azure-aanbieding (MS-AZR-0145p) in CSP definitief in fase 3 wordt ingetrokken.

   > [!NOTE]
   > Er zijn geen geautomatiseerde hulpprogramma's beschikbaar voor dit scenario en het onderstaande proces moet worden gebruikt.

- Als alleen de huidige partner een klant heeft met een actief abonnement voor een vorige **Azure-aanbieding (MS-AZR-0145p)** en de toekomstige partner niet, is de overdracht van de vorige Azure-aanbieding tussen partners na fase 1 niet meer mogelijk. Omdat de toekomstige partner geen eerder abonnement op Azure-aanbieding (MS-AZR-0145p) voor de klant kan maken, wordt deze overdracht niet ingeschakeld. In dit geval kan dit overgangshulpprogramma worden gebruikt om het Azure-abonnement van de klant tussen partners in CSP te verplaatsen en tegelijkertijd te converteren naar een nieuw Azure-aanbiedingsabonnement.

Volg deze handmatige stappen om de Azure-services of -abonnementen van een klant over te schakelen naar een andere partner met de vorige Azure-aanbieding (MS-AZR-0145p). Zowel de partner als de klant moeten de stappen voltooien.

> [!NOTE]  
> Op dit moment kunnen alleen directe of indirecte providers abonnementen overdragen.
> U kunt partners niet wijzigen voor Cloud Solution Provider die zijn gekoppeld aan azure-abonnement, Office 365, Enterprise Mobility Suite of Microsoft Dynamics CRM abonnementen.

## <a name="transfer-azure-subscriptions-to-another-partner-with-the-previous-azure-offer"></a>Azure-abonnementen overdragen naar een andere partner met de vorige Azure-aanbieding

1. Als u een Azure-abonnement wilt overdragen naar een nieuwe partner met de vorige Azure-aanbieding, moet de klant het proces starten en contact opnemen met de huidige recordpartner.

   > [!NOTE]
   > Het is de verantwoordelijkheid van de huidige partner om het serviceticket te maken dat het overdrachtsproces start. Microsoft kan niet ingrijpen namens de klant of de nieuwe partner. De klant moet nauw samenwerken met de huidige partner om de overgang soepel te laten verlopen.

2. De partner voor het abonnement moet de volgende taken uitvoeren:

   Maak een Azure-serviceticket van Partner Center om een abonnementsoverdracht aan te vragen:

   1. Selecteer in Partner Center menu **Klanten,** selecteer uw klant in de lijst en selecteer **vervolgens Servicebeheer.**
   2. Selecteer in **de sectie Ondersteuningstickets** de **vervolgkeuzekeuzekaart** Nieuw ticket en kies **Microsoft Azure**.
   3. Selecteer in [Azure Portal](https://portal.azure.com)de optie **Nieuwe ondersteuningsaanvraag.**
   4. Kies in Stap  1 Abonnementsbeheer als het type probleem, geef de abonnements-id op die u wilt overgedragen en kies **Cloud Solution Provider** als ondersteuningsplan.
   5. Selecteer in Stap 2 **de optie C-Minimal impact** en kies Overige algemene **vragen** als het probleemtype.
   6. Download het [formulier voor CSP-abonnementsoverdracht.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)

3. De partner voor het abonnement: Vul het [formulier CSP-abonnementsoverdracht](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)in, onderteken het en verzend het vervolgens naar de klant. 

   Als u het formulier wilt invullen, hebt u de volgende informatie nodig:

   - De contactgegevens van de huidige partner en de Microsoft-id. Selecteer in Partner Center menu Accountinstellingen  Organisatieprofiel en gebruik de &gt;  **Microsoft-id,** organisatienaam en het adres die hier worden vermeld. 
   - De Microsoft-id van de klant. Selecteer in Partner Center menu Klanten **en** vouw vervolgens de vermelding van de klant uit om de **Microsoft-id weer te geven.**
   - De abonnements-id die moet worden overdragen. Selecteer in de uitgebreide lijst met klanten Abonnementen weergeven en vouw vervolgens het gekozen abonnement uit om de **abonnements-id** **te zien.**

   > [!NOTE]
   > Het overdragen van een abonnement resulteert in twee abonnements-id's die u ziet op de pagina Abonnement bewerken van het overgedragen abonnement: **1:** de Partner Center-abonnements-id wordt gebruikt voor factureringsdoeleinden.  **2:** de oorspronkelijke Azure-abonnements-id blijft behouden en wordt weergegeven in Partner Center en in de Azure Management-portal. Deze id wordt weergegeven in uw reconbestand.  **Bij het registreren van ondersteuningstickets moet u beide ID's gebruiken.**

4. De klant en de nieuwe partner voor het abonnement:

   Controleer het formulier, vul informatie over de nieuwe partner in en onderteken het. Controleer of de nieuwe klant een contractovereenkomst heeft. Verzend het formulier terug naar de huidige recordpartner.

   *Belangrijk:* als de nieuwe CSP-partner geen resellerrelatie met de klant heeft, moet deze er een maken voordat het abonnement wordt overgedragen. [U vindt hier informatie over hoe u dit doet.](request-a-relationship-with-a-customer.md)

   > [!NOTE]
   > De nieuwe CSP-partner en de tenant van de klant moeten zich in hetzelfde land hebben. 

5. Huidige partner:

   Zorg ervoor dat het formulier contactgegevens voor beide partnerbeheerders bevat. Microsoft-ondersteuning neemt contact op met beide beheerders om de overdracht te controleren. Zorg ervoor dat u alle drie de handtekeningen hebt. Gebruik vervolgens de **optie Upload** om het ingevulde formulier te koppelen aan uw bestaande serviceaanvraag. Een Ondersteuningstechnicus van Microsoft neemt binnen acht uur na ontvangst en voltooiing een ontvangstbewijs bij u op.

6. Nieuwe partner:

   Werk de azure-abonnementsinstellingen bij om de oude partner uit het account te verwijderen. Als u wilt zien welke roltoewijzingen zijn ingericht, moet u twee PowerShell-commandlets uitvoeren.

   - Voeg de nieuwe partner toe als de reseller aan het account:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     > [!NOTE]
     > De **tenant-id** van de klant wordt in Partner Center als de Microsoft-id van **de klant.** Als u de Microsoft-id (tenant-id) voor een specifieke klant wilt zoeken, moet u zich aanmelden bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard) Selecteer vervolgens **Klanten** in het menu. Zoek de klant in de lijst. Selecteer de pijl-omlaag om de aanbieding van de klant uit te vouwen. U ziet informatie over de domeinnaam van de klant *en* de **Microsoft-id van de klant.** Gebruik de Microsoft-id van **16 cijfers** in de PowerShell-commandlet.

   - Rollen voor het account weergeven, met inbegrip van eerdere CSP-partners:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Verouderde toegangsmachtigingen verwijderen:

   1. Selecteer in Partner Center menu **Klanten.**
   1. Zoek de klant in de lijst. Selecteer (dubbelklik) op de bedrijfsnaam. Met deze actie wordt de pagina **Abonnementen van de klant** geopend.
   1. Selecteer Servicebeheer in het detailmenu **van de klant.**
   1. Onder **Microsoft Azure** selecteert u de **Microsoft Azure Beheerportal** koppeling.

## <a name="next-steps"></a>Volgende stappen

- [Overdracht van Azure-abonnementen](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Azure-abonnementen overdragen onder een Azure-plan](transfer-azure-subscriptions-under-azure-plan.md)
- Het [formulier voor CSP-abonnementsoverdracht downloaden](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)
- Meer informatie [over ondersteuning voor meerdere partners](multipartner.md)
- Meer informatie [over ondersteuning voor meerdere kanalen](multichannel.md)

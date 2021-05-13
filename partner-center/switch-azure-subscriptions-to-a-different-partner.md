---
title: Een Azure-abonnement overdragen aan een andere partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het wijzigen van Cloud Solution Provider programmapartner die is gekoppeld aan de Azure-abonnementen van een klant.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856063"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Meer informatie over het overdragen van Azure-abonnementen van een klant naar een andere partner

**Van toepassing op**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Juiste rollen:** globale beheerder

In dit artikel wordt beschreven hoe een klant zijn of haar Microsoft Azure services van de ene Cloud Solution Provider (CSP) naar de andere kan overstappen.

Volg deze handmatige stappen om de Azure-services of -abonnementen van een klant over te schakelen naar een andere partner. Zowel de partner als de klant moeten de stappen voltooien.

>[!Note]  
>Op dit moment kunnen alleen directe of indirecte providers abonnementen overdragen.
>U kunt partners niet wijzigen voor Cloud Solution Provider die zijn gekoppeld aan een Azure-abonnement, Office 365-, Enterprise Mobility Suite- of Microsoft Dynamics CRM-abonnementen.

## <a name="switch-partners-for-azure-subscriptions"></a>Van partner wisselen voor Azure-abonnementen

1. Als u een Azure-abonnement wilt overdragen naar een nieuwe partner, moet de klant het proces starten en de huidige recordpartner van de klant op een schrijvende manier contact opnemen.

   >[!Note]
   > Het is de verantwoordelijkheid van de huidige partner om het serviceticket te maken dat het overdrachtsproces initieert. Microsoft kan niet ingrijpen namens de klant of de nieuwe partner. De klant moet nauw samenwerken met de huidige partner om de overgang soepel te laten verlopen.

2. De partner voor het abonnement moet de volgende taken uitvoeren:

   Maak een Azure-serviceticket van Partner Center om een abonnementsoverdracht aan te vragen:

   1. Selecteer in Partner Center menu **Klanten,** selecteer uw klant in de lijst en selecteer vervolgens **Servicebeheer.**

   2. Selecteer in **de sectie Ondersteuningstickets** de vervolgkeuzekeuzekaart Nieuw **ticket** en kies **Microsoft Azure**.
   
   3. Selecteer in [Azure Portal](https://portal.azure.com)de optie **Nieuwe ondersteuningsaanvraag.**
   
   4. Kies in Stap  1 Abonnementsbeheer als het type probleem, geef de abonnements-id op die u wilt overgedragen en kies **Cloud Solution Provider** als ondersteuningsplan.
   
   5. Selecteer in Stap 2 **de optie C-Minimal impact** en kies Overige algemene **vragen** als het probleemtype.
   
   6. Download het [formulier voor CSP-abonnementsoverdracht.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)

3. De partner voor het abonnement: Vul het [formulier CSP-abonnementsoverdracht](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)in, onderteken het en verzend het vervolgens naar de klant. 

   Als u het formulier wilt invullen, hebt u de volgende informatie nodig:

   - De contactgegevens van de huidige partner en de Microsoft-id. Selecteer in Partner Center menu Accountinstellingen  Organisatieprofiel en gebruik de &gt;  **Microsoft-id,** organisatienaam en het adres die hier worden vermeld. 

   - De Microsoft-id van de klant. Selecteer in Partner Center menu Klanten **en** vouw vervolgens de vermelding van de klant uit om de **Microsoft-id weer te geven.**

   - De abonnements-id die moet worden overdragen. Selecteer in de uitgebreide lijst met klanten Abonnementen weergeven en vouw vervolgens het gekozen abonnement uit om de **abonnements-id** **te zien.**

   >[!Note]
   >Het overdragen van een abonnement resulteert in twee abonnements-id's die u ziet op de pagina Abonnement bewerken van het overgedragen abonnement: **1:** de Partner Center-abonnements-id wordt gebruikt voor factureringsdoeleinden.  **2:** de oorspronkelijke Azure-abonnements-id blijft behouden en wordt weergegeven in Partner Center en in de Azure Management-portal. Deze id wordt weergegeven in uw reconbestand.  **Bij het registreren van ondersteuningstickets moet u beide ID's gebruiken.**

4. De klant en de nieuwe partner voor het abonnement:

   Controleer het formulier, vul informatie over de nieuwe partner in en onderteken het. Controleer of de nieuwe klant een contractovereenkomst heeft. Verzend het formulier terug naar de huidige recordpartner.

   *Belangrijk:* als de nieuwe CSP-partner geen resellerrelatie met de klant heeft, moet deze er een maken voordat het abonnement wordt overgedragen. [U vindt hier informatie over hoe u dit doet.](request-a-relationship-with-a-customer.md)

   >[!Note]
   >De nieuwe CSP-partner en de tenant van de klant moeten zich in hetzelfde land hebben. 

5. Huidige partner:

   Zorg ervoor dat het formulier contactgegevens voor beide partnerbeheerders bevat. Microsoft-ondersteuning neemt contact op met beide beheerders om de overdracht te controleren. Zorg ervoor dat u alle drie de handtekeningen hebt. Gebruik vervolgens de optie **Bestand uploaden** om het ingevulde formulier te koppelen aan uw bestaande serviceaanvraag. Een ondersteuningstechnicus van Microsoft krijgt u binnen acht werkdagen terug om ontvangst en voltooiing te valideren.

6. Nieuwe partner:

   Werk de instellingen van het Azure-abonnement bij om de oude partner uit het account te verwijderen. Voer twee PowerShell-commandlets uit om te zien welke roltoewijzingen zijn ingericht.

   - Voeg de nieuwe partner als de reseller toe aan het account:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > De **tenant-id van de klant** wordt in de Partner Center als de Microsoft-id van de **klant.** Als u de Microsoft-id (tenant-id) voor een specifieke klant wilt zoeken, meld u zich aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard). Selecteer vervolgens **Klanten** in het menu. Zoek de klant in de lijst. Selecteer de pijl-omlaag om de aanbieding van de klant uit te vouwen. U ziet informatie over de domeinnaam van de klant *en* de **Microsoft-id van de klant.** Gebruik de 16-cijferige **Microsoft-id** in de PowerShell-commandlet.

   - Rollen voor het account weergeven, met inbegrip van eerdere CSP-partners:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Verouderde toegangsmachtigingen verwijderen:

   - Selecteer in Partner Center menu **Klanten.**
   - Zoek de klant in de lijst. Selecteer (dubbelklik) op de naam van het bedrijf. Met deze actie wordt de pagina **Abonnementen van de klant** geopend.
   - Selecteer Servicebeheer in het detailmenu **van de klant.**
   - Selecteer **onder Microsoft Azure** de koppeling om naar de Microsoft Azure Management Portal. 

## <a name="next-steps"></a>Volgende stappen

- Download het [formulier voor CSP-abonnementsoverdracht.](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA)

- Meer informatie [over ondersteuning voor meerdere partners.](multipartner.md)

- [ondersteuning voor meerdere partners.](multipartner.md)
- [ondersteuning voor meerdere kanalen.](multichannel.md)
- [Overdracht van Azure-abonnementen](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
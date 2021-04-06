---
title: Azure-abonnement overdragen aan een andere partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het wijzigen van de partner van het Cloud Solution Provider-programma dat is gekoppeld aan de Azure-abonnementen van een klant.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 886c39d192316987dcb68bff4d75302cc18a1305
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441911"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Meer informatie over het overdragen van Azure-abonnementen van een klant naar een andere partner

**Van toepassing op**

- Partnercentrum voor Microsoft Cloud for US Government

In dit artikel wordt beschreven hoe een klant de Microsoft Azure Services van de ene Cloud Solution Provider (CSP) naar een andere kan overschakelen.

Als u de Azure-Services of-abonnementen van een klant wilt overschakelen naar een andere partner, volgt u deze hand matige stappen. Zowel de partner als de klant moeten de stappen volt ooien.

>[!Note]  
>Op dit moment kunnen alleen directe of indirecte providers abonnementen overdragen.
>U kunt geen partners wijzigen voor Cloud Solution Provider-abonnementen die zijn gekoppeld aan het Azure-abonnement, Office 365, Enter prise Mobility Suite of micro soft Dynamics CRM-abonnementen.

## <a name="switch-partners-for-azure-subscriptions"></a>Scha kelen tussen partners voor Azure-abonnementen

1. Als u een Azure-abonnement wilt overdragen naar een nieuwe partner, moet de klant het proces starten en contact opnemen met de huidige partner van de record.

   >[!Note]
   > Het is de verantwoordelijkheid van de huidige partner om het service ticket te maken dat het overdrachts proces initieert. Micro soft kan niet door namens de klant of de nieuwe partner worden gehandeld. De klant moet plannen om nauw keurig aan de slag te gaan met de huidige partner om de overgang soepel te laten verlopen.

2. De partner van het abonnement moet de volgende taken uitvoeren:

   Een Azure-service ticket maken van het partner centrum om een abonnements overdracht aan te vragen:

   1. Selecteer in het menu Partner Center **klanten**, selecteer uw klant in de lijst en selecteer vervolgens **Service beheer**.

   2. Selecteer in de sectie **ondersteunings tickets** de vervolg keuzelijst **nieuw ticket** en kies **Microsoft Azure**.
   
   3. Selecteer een **nieuwe ondersteunings aanvraag** in het [Azure Portal](https://portal.azure.com).
   
   4. Kies in stap 1 **abonnements beheer** als het type probleem, geef de abonnements-id op die u wilt overdragen en kies **Cloud Solution Provider** als ondersteunings plan.
   
   5. Selecteer in stap 2 **C-minimale impact** en kies **andere algemene vragen** als het probleem type.
   
   6. Down load het [formulier CSP-abonnements overdracht](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).

3. De partner van het abonnement: Vul het formulier voor de overdracht van het [CSP-abonnement](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)in, onderteken dit en stuur het vervolgens naar de klant. 

   U hebt de volgende informatie nodig om het formulier in te vullen:

   - De contact gegevens en micro soft-ID van de huidige partner. Selecteer in het menu van het partner centrum **account instellingen** &gt; **organisatie profiel** en gebruik de **micro soft-id**, de **organisatie naam** en het **adres** dat hier wordt vermeld.

   - De micro soft-ID van de klant. Selecteer **klanten** in het menu van het partner centrum en vouw vervolgens de lijst van de klant uit om de **micro soft-id** te bekijken.

   - De abonnements-ID die moet worden overgedragen. Selecteer in de lijst uitgebreide klant de optie **abonnementen weer geven** en vouw vervolgens het gekozen abonnement uit om de **abonnements-id** weer te geven.

   >[!Note]
   >Het overdragen van een abonnement resulteert in twee abonnement-Id's die u ziet op de pagina **abonnement bewerken** van het overgedragen abonnement: **1**-de abonnements-id van het partner centrum wordt gebruikt voor facturerings doeleinden. **2**-de oorspronkelijke id van het Azure-abonnement wordt bewaard en wordt in partner centrum en in de Azure-beheer portal weer gegeven. Deze ID wordt weer gegeven in het afstemmings bestand.  **Wanneer u logboek registratie tickets ondersteunt, moet u beide Id's gebruiken.**

4. De klant en de nieuwe partner voor het abonnement:

   Bekijk het formulier, vul de informatie in over de nieuwe partner en onderteken deze. Controleer of de nieuwe klant een contract overeenkomst heeft. Het formulier opnieuw verzenden naar de huidige partner van de record.

   *Belang rijk*: als de nieuwe CSP-partner geen wederverkoper-relatie met de klant heeft, moet deze een verbinding tot stand brengen voordat het abonnement wordt overgedragen. [U vindt hier informatie over hoe u dit kunt doen](request-a-relationship-with-a-customer.md).

   >[!Note]
   >De nieuwe CSP-partner en de Tenant van de klant moeten zich in hetzelfde land begaan. 

5. Huidige partner:

   Zorg ervoor dat het formulier contact gegevens voor beide partner beheerders bevat. Microsoft Ondersteuning neemt contact op met beide beheerders om de overdracht te controleren. Zorg ervoor dat u alle drie hand tekeningen hebt. Gebruik vervolgens de optie voor het **uploaden van bestanden** om het voltooide formulier aan uw bestaande service aanvraag te koppelen. Een ondersteunings technicus van micro soft zal binnen acht werk uren aan u terugkomen om de ontvangst en voltooiing te valideren.

6. Nieuwe partner:

   Werk de instellingen van het Azure-abonnement bij om de oude partner uit het account te verwijderen. Als u wilt zien welke roltoewijzingen zijn ingericht, voert u twee Power shell-Commandlets uit.

   - Voeg de nieuwe partner als wederverkoper toe aan het account:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > De **Tenant-id** van de klant wordt weer gegeven in het partner centrum als de **micro soft-id** van de klant. Als u de micro soft-ID (Tenant-ID) voor een specifieke klant wilt zoeken, meldt u zich aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum. Selecteer vervolgens **klanten** in het menu. Zoek de klant op de lijst. Selecteer de pijl-omlaag om de vermelding van de klant uit te vouwen. U ziet informatie over de *domein naam* van de klant en de **micro soft-id** van de klant. Gebruik de **micro soft-id** van 16 cijfers in de Power shell-commandlet.

   - Rollen weer geven voor het account, waaronder eerdere CSP-partners:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Verouderde toegangs machtigingen verwijderen:

   - Selecteer **klanten** in het menu van het partner centrum.
   - Zoek de klant op de lijst. Selecteer (dubbel klikken) hun bedrijfs naam. Met deze actie wordt de pagina klant **abonnementen** geopend.
   - Selecteer **Service beheer** in het detail menu van de klant.
   - Selecteer onder **Microsoft Azure** de koppeling om naar de **Microsoft Azure Management Portal** te gaan.

## <a name="next-steps"></a>Volgende stappen

- Down load het [formulier CSP-abonnements overdracht](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Meer informatie over [ondersteuning voor meerdere partners](multipartner.md).

- [ondersteuning voor meerdere partners](multipartner.md).
- [ondersteuning voor meerdere kanalen](multichannel.md).
- [Overdracht van Azure-abonnementen](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
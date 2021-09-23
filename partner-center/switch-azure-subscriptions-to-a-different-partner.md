---
title: Een Azure-abonnement overdragen naar een andere partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Meer informatie over het wijzigen van Cloud Solution Provider programmapartner die is gekoppeld aan de Azure-abonnementen van een klant.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 07/21/2021
ms.openlocfilehash: b9ce8fff5915d3d4bf42f699c5a0c9130e37814b
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322115"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-partner-without-converting-them-to-an-azure-plan"></a>De Azure-abonnementen van een klant overdragen aan een andere partner zonder deze te converteren naar een Azure-plan

**Van toepassing op**: Partner Center | Partner Center voor Microsoft Cloud for US Government

**Juiste rollen:** globale beheerder

In dit artikel wordt beschreven hoe een klant een Azure-abonnement kan overdragen van hun huidige Cloud Solution Provider (CSP) naar een andere CSP.

In de eerste sectie, Een Azure-abonnement overdragen naar een andere [partner,](#transferring-azure-subscriptions-to-another-partner)wordt beschreven hoe een klant een Microsoft Azure-abonnement kan overdragen van het ene Cloud Solution Provider (CSP) naar het andere.

In de volgende sectie, Een eerder azure-aanbiedingsabonnement overdragen zonder dit te converteren naar het [Azure-plan,](#transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan)wordt kort beschreven hoe het nieuwe Azure-plan wordt geïntroduceerd. Vervolgens wordt een speciaal geval beschreven waarin sommige abonnementen op de vorige Azure-aanbieding kunnen worden overgedragen naar een andere CSP zonder deze te converteren naar het nieuwe Azure-plan.

De klant, de huidige serviceprovider en een nieuwe serviceprovider hebben allemaal verantwoordelijkheden bij het overdragen van een klantabonnement naar [een nieuwe Azure-serviceprovider.](#responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider) Een klant moet van plan zijn nauw samen te werken met de huidige partner om de overgang soepel te laten verlopen.

 Informatie op hoog niveau om Azure-abonnees te helpen abonnementen over te dragen van en naar CSP-partners vindt u in Azure-abonnementen overdragen tussen [abonnees en CSP's.](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)

Meer informatie over hoe klanten hun Azure-abonnementen van de ene partner naar de andere kunnen wijzigen, vindt u in Azure-abonnementen van een klant overdragen naar een andere [CSP (onder een Azure-plan)](./transfer-azure-subscriptions-under-azure-plan.md)

## <a name="prerequisites"></a>Vereisten

- Een CSP-partner moet een resellerrelatie hebben met een klant voordat een abonnement kan worden overgedragen.  Zie How [to request a reseller relationship from a customer (Een resellerrelatie aanvragen](./request-a-relationship-with-a-customer.md)bij een klant) in Partner Center .
- Een partner moet een directe provider of een indirecte provider zijn om een abonnement over te dragen.
- Abonnementen die aan de volgende aanbiedingen zijn gekoppeld, kunnen niet worden overgedragen: Azure-plan, Office 365, Enterprise Mobility Suite en Microsoft Dynamics CRM.
- Een klant moet zich in hetzelfde land als een partner hebben om een abonnement over te dragen.
- Partners die in Microsoft Cloud for US Government Microsoft Cloud Duitsland werken, moeten toestemming vragen om de service of het abonnement van een klant te beheren. Zie Machtigingen verkrijgen voor het beheren van de service of het [abonnement van een klant voor meer informatie.](./customers-revoke-admin-privileges.md)

## <a name="transferring-azure-subscriptions-to-another-partner"></a>Azure-abonnementen overdragen naar een andere partner

Het overdragen van een Azure-abonnement van de ene CSP-partner naar een andere is een proces met meerdere stappen dat in verschillende fasen acties vereist door de klant, de huidige partner en de nieuwe partner. De volgende tabel is bedoeld als een sequentiediagram om te verduidelijken wie wat doet en wanneer.

### <a name="responsibilities-when-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Verantwoordelijkheden bij het overdragen van een klantabonnement naar een nieuwe Azure-serviceprovider

|Stap  |Klant  |Huidige partner  |Nieuwe partner  |
|---------|---------|---------|---------|
|1     |[De klant stelt Microsoft en de huidige partner op de de markt als ze dit schrijven](#step-1-customer-contacts-current-partner-in-writing)         |         |         |
|2     |         |[Ondersteuningsticket maken om overdracht aan te vragen](#step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer)        |         |
|3     |         |[Formulier voor voltooide overdracht naar klant verzenden](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)|         |
|4     |         |[De wijziging van het Cloud Solution Provider voltooien](#step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer)       |         |
|5     |[Formulier controleren, ondertekenen & retourneren](#step-5-the-customer-and-new-partner-review--return-the-form)       |         |[Formulier controleren, ondertekenen & retourneren](#step-5-the-customer-and-new-partner-review--return-the-form)         |
|6     |         |[Formulier controleren en koppelen aan serviceaanvraag](#step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request)        |         |
|7     |         |         |[Oude partner uit account verwijderen](#step-7-new-partner-removes-old-partner-from-account)         |
|8     |         |         |[Verouderde toegangsmachtigingen verwijderen](#step-8-new-partner-removes-outdated-access-permissions)         |

### <a name="steps-for-transferring-a-customer-subscription-to-a-new-azure-service-provider"></a>Stappen voor het overdragen van een klantabonnement naar een nieuwe Azure-serviceprovider

#### <a name="step-1-customer-contacts-current-partner-in-writing"></a>Stap 1: De klant neemt momenteel contact op met de huidige partner

De klant start het overdrachtsproces door zowel Microsoft als de huidige CSP-partner op de hoogte te stellen van hun aanvraag om een abonnement over te dragen (dus niet in woorden).

#### <a name="step-2-current-provider-creates-azure-support-ticket-to-request-a-transfer"></a>Stap 2: De huidige provider maakt ondersteuning voor Azure ticket om een overdracht aan te vragen

De huidige partner maakt een ondersteuning voor Azure om een abonnementsoverdracht aan te vragen.

> [!NOTE]
> Het is de verantwoordelijkheid van de huidige partner om het ondersteuningsticket te maken dat het overdrachtsproces start. Microsoft komt niet in actie namens de klant of de nieuwe partner.

**Een ondersteuningsticket maken om een overdracht aan te vragen:**

1. Selecteer in Partner Center menu **Klanten,** selecteer de klant in de lijst en selecteer vervolgens **Servicebeheer.**
1. Selecteer in **de sectie Ondersteuningstickets** de optie Nieuw **ticket** en klik **Microsoft Azure.**
1. Selecteer [in Azure Portal](https://portal.azure.com/)nieuwe **ondersteuningsaanvraag**.
1. Kies in Stap 1 van  de ondersteuningsaanvraag Abonnementsbeheer als het type probleem, geef de abonnements-id op die u wilt overgedragen en kies Cloud Solution Provider **als** ondersteuningsplan.
1. Selecteer in Stap 2 **de optie C-Minimal impact** en kies Overige algemene **vragen** als het probleemtype.

#### <a name="step-3-current-partner-completes-transfer-form-and-sends-it-to-the-customer"></a>Stap 3: De huidige partner voltooit het overdrachtsformulier en verzendt het naar de klant

De huidige partner downloadt en voltooit de wijziging [van Cloud Solution Provider formulier](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC), ondertekent het en verzendt het vervolgens naar de klant.

#### <a name="step-4-current-partner-completes-current-partner-fills-in-the-change-of-cloud-solution-provider-form"></a>Stap 4: Huidige partner vult het formulier Wijziging van Cloud Solution Provider in

De huidige partner voltooit de [wijziging van het Cloud Solution Provider formulier,](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)ondertekent het en verzendt het naar de klant.

Een van de informatie die nodig is om het *formulier Change of Cloud Solution Provider* in te vullen, is:

- **De contactgegevens van de huidige** partner en de Microsoft-id (te vinden in het Partner Center-menu door Accountinstellingen te selecteren **> Organisatieprofiel).**
- **De Microsoft-id van** de klant (te vinden in  het Partner Center-menu door Klanten te selecteren en vervolgens de vermelding van de klant uit te breiden om hun Microsoft-id weer te geven).
-  De abonnements-id die u wilt overdragen (te vinden in  het Partner Center-menu door Klanten te selecteren en vervolgens de aanbieding van de klant uit te breiden, Abonnementen weergeven te selecteren en vervolgens het gekozen abonnement uit te breiden om de **abonnements-id** weer te geven.

#### <a name="step-5-the-customer-and-new-partner-review--return-the-form"></a>Stap 5: de klant en de nieuwe partnerbeoordeling & formulier te retourneren

Samenwerken, de klant en de nieuwe partner:

1. Controleer het formulier, vul informatie in over de nieuwe partner en onderteken het.
1. Controleer of de nieuwe klant een contractovereenkomst heeft.
1. Verzend het formulier terug naar de huidige partner.

#### <a name="step-6-current-partner-reviews-form-and-attaches-it-to-the-service-request"></a>Stap 6: het formulier beoordelingen van de huidige partner en het formulier koppelen aan de serviceaanvraag

Wanneer de huidige partner het formulier ontvangt, gebeurt het volgende:

- Zorg ervoor dat het formulier contactgegevens voor beide partnerbeheerders bevat. (Microsoft-ondersteuning contact op met beide beheerders om de overdracht te controleren.)
- Controleer of ze alle drie de handtekeningen hebben en gebruik vervolgens de optie **Upload** ingevulde formulier bij de bestaande serviceaanvraag te koppelen. (Een ondersteuningstechnicus van Microsoft neemt binnen acht werkdagen contact met hen op om ontvangst en voltooiing te valideren.)

#### <a name="step-7-new-partner-removes-old-partner-from-account"></a>Stap 7: nieuwe partner verwijdert oude partner uit account

De nieuwe partner werkt de instellingen van het Azure-abonnement in PowerShell bij om de oude partner uit het account te verwijderen.

> [!NOTE]
> Voor de eerste PowerShell-cmdlet is de **tenant-id** van de klant vereist. Deze wordt in Partner Center weergegeven als de **Microsoft-id van de klant.** In de volgende procedure wordt beschreven hoe u de Microsoft-id (tenant-id) van de klant kunt vinden voor gebruik in de cmdlet .

Als u de Microsoft-id (tenant-id) van een klant wilt zoeken voor gebruik in de ***powershell-cmdlet Verbinding maken-AzAccount:***

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).
1. Selecteer **Klanten** in het menu.
1. Zoek de klant in de lijst die wordt weergegeven.
1. Selecteer de pijl-omlaag om de aanbieding van de klant uit te vouwen. U ziet informatie over de domeinnaam van de klant *en* de **Microsoft-id van de klant.**
1. Gebruik de 16-cijferige **Microsoft-id** in de PowerShell-cmdlet die volgt op deze procedure.

Met de eerste PowerShell-cmdlet wordt de nieuwe partner toegevoegd als de reseller voor het account:

```powershell
Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
```

De tweede cmdlet geeft de rollen voor het account weer, met inbegrip van eerdere CSP-partners:

```powershell
Get-AzRoleAssignment
```

#### <a name="step-8-new-partner-removes-outdated-access-permissions"></a>Stap 8: Nieuwe partner verwijdert verouderde toegangsmachtigingen

   **Verouderde toegangsmachtigingen verwijderen:**

   1. Selecteer in Partner Center menu **Klanten.**
   1. Zoek de klant op in de lijst met klanten.
   1. Dubbelklik op de bedrijfsnaam van de klant. De pagina **Abonnementen van de** klant wordt weergegeven.
   1. Selecteer Servicebeheer in het detailmenu **van de klant.**
   1. Selecteer **Microsoft Azure** onder **Microsoft Azure Beheerportal**.

## <a name="transferring-a-previous-azure-offer-subscription-without-converting-it-to-the-azure-plan"></a>Een eerder azure-aanbiedingsabonnement overdragen zonder dit te converteren naar het Azure-plan

In deze sectie wordt kort beschreven hoe het nieuwe Azure-plan wordt geïntroduceerd. Vervolgens wordt een speciaal geval beschreven waarin sommige abonnementen op de vorige Azure-aanbieding kunnen worden overgedragen naar een andere CSP zonder deze te converteren naar het nieuwe Azure-plan.

> [!NOTE]
> Als u de Azure-abonnementen van een klant die zijn aangeschaft via de vorige Azure-aanbieding, wilt overdragen naar een nieuwe CSP en deze wilt converteren naar het *Azure-abonnement*(dit is de standaardactie), gaat u naar de vorige sectie Een [*Azure-abonnement*](#transferring-azure-subscriptions-to-another-partner)overdragen naar een andere partner en het artikel Azure-abonnementen van een klant overdragen naar een andere [*CSP (onder een Azure-abonnement).*](./transfer-azure-subscriptions-under-azure-plan.md)

### <a name="the-azure-plan-and-the-previous-azure-offer"></a>Het Azure-plan en de vorige Azure-aanbieding

Microsoft heeft in juli [](./azure-plan-lp.md)2021 een nieuwe commerce-ervaring geïntroduceerd, het Azure-plan. Om partners de tijd te geven om nieuwe functies in hun services op te nemen en klanten over te latenstappen van de vorige Azure-aanbieding (MS-AZR-0145p) naar het Azure-plan, blijft de vorige Azure-aanbieding tijdelijk beschikbaar.

De overgang van de vorige Azure-aanbieding naar het Azure-plan bestaat uit drie fasen:

**Fase 1:** sinds de introductie van het Azure-plan in juli 2021 zijn alle nieuwe klanten Azure CSP-programma's op het Azure-plan geplaatst. Partners kunnen de vorige Azure-aanbieding blijven uitvoeren met klanten die deze al hebben aangeschaft.

**Fase 2:** op 1 februari 2022 worden incentives en de kans op marges van partners verwijderd uit de vorige Azure-aanbieding.

**Fase 3:** op een moment dat nog moet worden bepaald, wordt de vorige Azure-aanbieding ingetrokken en worden klanten die nog steeds de vorige Azure-aanbieding hebben gebruikt, gemigreerd naar het Azure-plan. (Partners worden zes maanden van tevoren op de hoogte gesteld van de pensioendatum.)

### <a name="transferring-subscriptions-without-conversion"></a>Abonnementen overdragen zonder conversie

In deze sectie wordt het speciale geval beschreven van het overdragen van een abonnement dat is gekocht via de vorige Azure-aanbieding naar een nieuwe CSP-provider, zonder dit te converteren naar *het Azure-plan*.

Het abonnement van een klant op de vorige Azure-aanbieding kan worden overgedragen naar een nieuwe CSP-partner zonder conversie naar het Azure-plan met behulp van de stappen in de vorige sectie, Azure-abonnementen overdragen naar een andere [partner,](#transferring-azure-subscriptions-to-another-partner)als:

- De vorige Azure-aanbieding is nog steeds beschikbaar.
- Zowel de huidige partner als de nieuwe partner hebben een klant met een abonnement op de vorige Azure-aanbieding.

Als alleen de huidige partner een klant heeft met een abonnement op de vorige Azure-aanbieding, kan de huidige partner het overgangshulpprogramma gebruiken om het abonnement van de klant naar de nieuwe partner te verplaatsen en tegelijkertijd te converteren naar het nieuwe Azure-plan.

> [!NOTE]
> Alleen partners die een directe factureringsrelatie met Microsoft hebben, hebben toegang tot het overgangshulpprogramma. Indirecte resellers moeten samenwerken met hun indirecte providers om het overgangshulpprogramma te kunnen gebruiken.

## <a name="next-steps"></a>Volgende stappen

- [Overdracht van Azure-abonnementen](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)
- [Azure-abonnementen overdragen onder een Azure-plan](transfer-azure-subscriptions-under-azure-plan.md)
- Het [formulier voor CSP-abonnementsoverdracht downloaden](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC)
- Meer informatie [over ondersteuning voor meerdere partners](multipartner.md)
- Meer informatie [over ondersteuning voor meerdere kanalen](multichannel.md)
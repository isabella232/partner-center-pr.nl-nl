---
title: Azure-abonnement overdragen onder een Azure-plan naar een andere CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het wijzigen van de partner van het Cloud Solution Provider-programma dat is gekoppeld aan de Azure-abonnementen van een klant onder een Azure-abonnement.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/29/2020
ms.openlocfilehash: 4213658fc131d83d6c0640552d862f4de9b5ad86
ms.sourcegitcommit: e10d2a19dea7e317d227d7fbdcf1bbc3dc4f6257
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/13/2020
ms.locfileid: "92528659"
---
# <a name="transfer-a-customers-azure-plan-subscriptions-to-a-different-partner"></a>De Azure-plan abonnementen van een klant overdragen naar een andere partner

## <a name="applies-to"></a>Van toepassing op

- Partners in het Cloud Solution Provider-programma (CSP)

In dit artikel wordt beschreven hoe een klant hun Azure-abonnementen kan veranderen onder een Azure-abonnement van één Cloud Solution Provider (CSP) naar een andere.

Voer de volgende stappen uit om de Azure-abonnementen van een klant te wisselen van een andere partner. Zowel de partner als de klant heeft stappen om te volt ooien.

>[!Note]  
>Alleen partners met een directe facturerings relatie met micro soft hebben toegang tot het hulp programma overgang. Indirecte wederverkopers moeten samen werken met hun indirecte providers om gebruik te maken van dit overgangs programma.

De klant moet in gesprek zijn met beide partners (huidige en toekomstige) voordat dit hulp programma wordt gebruikt. Er moet een offline conversatie zijn om Verwar ring en verloop te voor komen. Daarnaast moeten partners en klanten op de hoogte zijn van deze overwegingen en vereisten voordat ze een overgang initiëren:

**Belangrijkste overwegingen:**

- Azure Reservations wordt niet met het abonnement verplaatst naar een toekomstige partner
- CSP-prijzen voor Azure-Services onder huidige partner worden niet overgezet  
- De ondersteunings verantwoordelijkheden voor de klant worden verplaatst naar de volgende partner
- Facturering en facturering worden verplaatst naar de volgende partner op het moment van de overdracht
- Azure Role-Based Access Control (RBAC) is niet van invloed op de overdracht
- Beheerder namens (ADMINISTRATE) wordt niet standaard verleend aan de toekomstige partner
- Marketplace-Producten van derden worden overgezet zolang de producten de controle op Marketplace door voeren.
    - Er zijn geen speciale kortingen of regionale beperkingen
    - De producten zijn niet gebaseerd op een abonnement
    - De volgende partner moet samen werken met de uitgever om er zeker van te zijn dat ze zich op de acceptatie lijst bevinden voor de implementatie van het product
    - Als niet aan al deze voor waarden wordt voldaan om de Marketplace-producten te kunnen overdragen, moeten de Azure-abonnementen worden overgezet en vervolgens opnieuw worden gekocht van Marketplace-Producten met de nieuwe partner

**Vereisten:**

- De klant houdt de huidige CSP-partner op hun intentie om over te gaan naar overgang
- Toekomstige CSP-partner werkt samen met de klant om ervoor te zorgen dat aan de behoeften van de klant kan worden voldaan
- Toekomstige CSP-partner brengt een relatie met de klant tot stand voordat de overgang begint  
- De klant moet de klant overeenkomst van micro soft ondertekenen met een toekomstige CSP-partner
- Toekomstige CSP-partner moet de micro soft-partner overeenkomst hebben ondertekend om dit hulp programma te gebruiken

## <a name="customer-tasks-to-be-completed"></a>Klant taken die moeten worden voltooid

Als u een Azure-abonnement wilt overdragen onder een Azure-plan, moet de klant het proces starten door contact op te nemen met de huidige partner. Ze moeten hun bedrijfs naam en domein van hun huidige partner verzamelen, zodat hun toekomstige partner het aanvraag formulier voor de overdracht kan volt ooien.

De klant moet ook de abonnementen identificeren die ze willen overdragen vanaf hun huidige partner. U kunt de partners voor Office 365, Enter prise Mobility Suite of micro soft Dynamics CRM-abonnementen niet wijzigen.

>[!Note]  
>Het is de verantwoordelijkheid van de toekomstige partner om het aanvraag formulier voor de overdracht te volt ooien waarmee het overdrachts proces wordt gestart. Micro soft kan niet namens de klant of de huidige partner worden gehandeld. De klant moet plannen om nauw keurig aan de slag te gaan met hun toekomstige en huidige partner om de overgang soepel te laten verlopen.

## <a name="future-partner-tasks-to-be-completed"></a>Toekomstige partner taken die moeten worden voltooid

De volgende partner van het abonnement moet een aanvraag formulier voor de overdracht van het partner centrum volt ooien om een abonnements overdracht aan te vragen:

1.  Selecteer **klanten** in het menu van het partner centrum en selecteer de klant waarvoor u een aanvraag formulier voor de overdracht wilt uitvoeren namens.
2.  Selecteer in het menu klant **abonnementen** .
3.  Selecteer de sectie **overdrachts aanvraag** .
4.  Selecteer in de **sectie overdrachts aanvraag** de optie **nieuwe aanvraag toevoegen** .

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Sectie overdrachten":::

5.  Vul het formulier voor de **nieuwe overdrachts aanvraag** in.

6.  Selecteer verzenden **overdracht aanvraag**  >  **verzenden** .

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Sectie overdrachten":::

7.  Bevestiging van overdrachts aanvraag controleren

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Sectie overdrachten":::

    >[!Note]
    >De volgende partner kan de overdrachts aanvraag annuleren door **Aanvraag annuleren** te selecteren in de rechter bovenhoek alleen wanneer de status van de overdrachts aanvraag ' in behandeling ' is. Wanneer de status van de overdrachts aanvraag ' wordt uitgevoerd ' of ' voltooid ' is, kunnen annuleringen niet worden geannuleerd.

## <a name="current-partner-tasks-to-be-completed"></a>Huidige partner taken die moeten worden voltooid

De beheerder agent van de huidige partner van de klant ontvangt een e-mail dat de klant een overdracht van hun abonnementen heeft aangevraagd:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Sectie overdrachten":::

Bekijk en accepteer het aanvraag formulier voor de overdracht van het partner centrum om de overdracht van het abonnement te volt ooien.

>[!Note]  
>Als er binnen 30 dagen geen actie wordt ondernomen door de huidige partner, verloopt de aanvraag en zal de volgende partner een nieuwe overdrachts aanvraag maken.

1.  Selecteer **aanvraag voor overdracht controleren** van de e-mail of
1.  Selecteer **klanten** in het menu van het partner centrum en selecteer de klant voor wie een aanvraag voor de overdracht is ingediend namens.
2.  Selecteer in het menu klant **abonnementen** .
3.  Selecteer de sectie **overdrachts aanvraag** .
4.  Uitbrei ding van overdrachts gegevens door de gekozen **aanvraag-id** voor de overdracht te selecteren onder **ontvangen aanvragen**

:::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Sectie overdrachten":::

5.  Overdrachts aanvraag controleren. Selecteer de aangevraagde Azure-abonnementen om over te dragen.

>[!Note]  
> Opmerking: u hebt geen toegang meer tot de geselecteerde abonnementen voordat u doorgaat.
> U wordt niet gefactureerd voor verder gebruik.
> Azure-reserve ringen worden niet overgedragen met de abonnementen.

6.  Selecteer vervolgens **accepteren en overdragen** om het overdrachts proces te volt ooien.

:::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Sectie overdrachten":::

7.  Bevestiging van acceptatie van overdracht weer geven.

   Op dit moment wordt de volgende partner, de klant en de huidige partner op de hoogte gesteld van de geaccepteerde overdrachts aanvraag via e-mail.

   Nadat de overgang is geaccepteerd, kan de overdrachts status Maxi maal 15 minuten in behandeling blijven terwijl het systeem wordt bijgewerkt. Als het langer duurt, blijft het systeem drie dagen proberen. Als de overdrachts status nog steeds in behandeling blijft, moet de partner een service aanvraag indienen.

   Zodra de overdracht is voltooid, worden de abonnementen die zijn opgenomen in de aanvraag, weer gegeven in het Azure-abonnement van de toekomstige partner en worden ze niet meer met u vermeld.

>[!Note]  
>Voor indirecte providers: Informeer uw indirecte wederverkoper dat de overdrachts aanvraag is geaccepteerd.

### <a name="managing-your-transferred-customer-subscriptions"></a>Uw overgedragen klant abonnementen beheren
- Toegang voor bestaande gebruikers, groepen of service-principals die is toegewezen met behulp van Azure RBAC (op rollen gebaseerd toegangsbeheer) wordt niet beïnvloed tijdens de overgang. Met Azure [RBAC (](/azure/role-based-access-control/overview) op rollen gebaseerd toegangs beheer) kan uw klant beheren wie toegang heeft tot Azure-resources, wat ze kunnen doen met deze resources en op welke gebieden ze toegang hebben. Als de nieuwe partner hebt u geen RBAC-toegang tot de resources van uw klant na de overdracht van het abonnement. De vorige partner van uw klant behoudt de RBAC-toegang. Werk samen met uw klant om te begrijpen wie inzicht heeft in hun abonnementen en hoe u de gewenste wijzigingen kunt aanbrengen.

- Het is dus belang rijk dat uw klant de Azure RBAC-toegang voor hun vorige partner verwijdert en dat er toegang wordt toegevoegd voor de nieuwe partner. Zie [Wat is Azure Role-based Access Control (Azure RBAC)?](/azure/role-based-access-control/overview) voor meer informatie over de klant die nieuwe toegang geeft. Zie [een roltoewijzing verwijderen](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)voor meer informatie over uw klant bij het verwijderen van de RBAC-toegang van uw vorige partner.

- Daarnaast krijgt u niet automatisch een [beheerder namens (administrate)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) toegang tot uw abonnementen. ADMINISTRATE is nodig voor het beheren van de Azure-abonnementen van hun klanten namens de partner. Zie [machtigingen voor het beheren van de service of het abonnement van een klant verkrijgen](./customers-revoke-admin-privileges.md) voor meer informatie over de bevoegdheden van Azure.

## <a name="next-steps"></a>Volgende stappen:

- [(Azure RBAC)](/azure/role-based-access-control/overview)
- [Machtigingen verkrijgen voor het beheren van de service of het abonnement van een klant.](./customers-revoke-admin-privileges.md)
---
title: Een Azure-abonnement van een Azure-plan overdragen naar een andere CSP-partner
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over het wijzigen van Cloud Solution Provider programmapartner die is gekoppeld aan de Azure-abonnementen van een klant onder een Azure-plan.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: mckennaville
ms.author: mcville
ms.date: 07/21/2021
ms.openlocfilehash: 14f03a8eb899f7224a38b0f998edd72077b34b3b
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244714"
---
# <a name="transfer-a-customers-azure-subscriptions-to-a-different-csp-under-an-azure-plan"></a>De Azure-abonnementen van een klant overdragen naar een andere CSP (onder een Azure-plan)

**Juiste rollen:** Accountbeheerder | Verkoopagent | Factureringsagent

In dit artikel wordt beschreven hoe klanten hun Azure-abonnementen kunnen wijzigen van de ene partner in het Cloud Solution Provider(CSP)-programma naar een andere, onder een Azure-plan.

Volg deze stappen om de Azure-abonnementen van een klant over te schakelen van een andere partner. De huidige partner, de toekomstige partner en de klant hebben allemaal de stappen die moeten worden voltooid.

> [!Note]  
> Alleen partners die een directe factureringsrelatie met Microsoft hebben, hebben toegang tot het overgangshulpprogramma. Indirecte resellers moeten samenwerken met hun indirecte providers om dit overgangshulpprogramma te kunnen gebruiken.

De klant moet communiceren met zowel de huidige als de toekomstige partner voordat het overgangshulpprogramma kan worden gebruikt. Er moet een offline gesprek plaatsvinden om verwarring en verloop te voorkomen. Partners en klanten moeten de volgende overwegingen en vereisten begrijpen voordat ze een overgang starten.

## <a name="considerations"></a>Overwegingen

- Azure-reserveringen worden niet verplaatst met een abonnement naar de toekomstige partner.
- CSP-prijzen voor Azure-services onder de huidige partner worden niet over overgangen.
- Als u eerdere [Azure-aanbiedingsabonnementen (MS-AZR-0145p)](https://go.microsoft.com/fwlink/p/?linkid=2164140) overboekt, worden deze Azure-abonnementen tegelijkertijd geconverteerd naar nieuwe Azure-aanbiedingsabonnementen binnen een Azure-plan.
- Ondersteuningsverantwoordelijkheden voor de klant worden verplaatst naar de toekomstige partner.
- Facturering en facturering worden verplaatst naar de toekomstige partner wanneer het abonnement wordt overgedragen.
- Op rollen gebaseerd toegangsbeheer (RBAC) van Azure wordt niet beïnvloed door overdrachten.
- Beheerder namens (AOBO) wordt niet standaard verleend aan de toekomstige partner.
- Producten van Azure Marketplace worden overgeplaatst zolang de producten voldoen aan Azure Marketplace geschiktheidscontrole.
    - Er zijn geen speciale kortingen of regionale beperkingen.
    - De producten zijn niet gebaseerd op een abonnement.
    - De toekomstige partner moet samenwerken met de uitgever om ervoor te zorgen dat de uitgever op de toegestane lijst staat voor implementatie van het product.
    - Als niet aan een van deze voorwaarden wordt voldaan, moeten de Azure Marketplace worden geannuleerd. Vervolgens moeten de Azure-abonnementen worden overgedragen en moeten Azure Marketplace producten worden gekocht bij de nieuwe partner.

## <a name="prerequisites"></a>Vereisten

- De klant meldt de huidige CSP-partner van de intentie om over te gaan.
- De toekomstige CSP-partner werkt samen met de klant om ervoor te zorgen dat aan de behoeften van de klant kan worden voldaan.
- De toekomstige CSP-partner brengt een relatie tot leven met de klant en koopt een Azure-plan voordat de overgang begint.
- De klant ondertekent een Microsoft-klantovereenkomst met de toekomstige CSP-partner.
- De toekomstige CSP-partner ondertekent de Microsoft Partner-overeenkomst voordat het overgangshulpprogramma wordt gebruikt.

> [!NOTE]
> Het hulpprogramma voor self-serviceovergang kan worden gebruikt wanneer de huidige partner van de klant de vorige Azure-aanbieding (MS-AZR-0145p) of de nieuwe Azure-aanbieding (Azure-plan) heeft. Wanneer de overdracht is voltooid, vallen de Azure-abonnementen in beide gevallen onder een Azure-plan met de toekomstige partner.

## <a name="customer-tasks"></a>Klanttaken

Als u Azure-abonnementen wilt overdragen, moet de klant het proces starten door contact op te nemen met de huidige partner. De klant moet de bedrijfsnaam en Microsoft-id van de huidige partner verzamelen, zodat de toekomstige partner namens de klant het formulier voor de overdrachtsaanvraag kan invullen.

Klanten moeten ook de abonnementen identificeren die ze willen overdragen van de huidige partner. U kunt geen partners wijzigen voor Office 365, Enterprise Mobility Suite of Microsoft Dynamics CRM abonnementen.

> [!NOTE]  
> Het is de verantwoordelijkheid van de toekomstige partner om het formulier voor overdrachtsaanvraag in te vullen dat het overdrachtsproces initieert. Microsoft kan niet ingrijpen namens de klant of de huidige partner. De klant moet van plan zijn nauw samen te werken met de toekomstige en huidige partners om ervoor te zorgen dat de overgang soepel verloopt.

## <a name="future-partner-tasks"></a>Toekomstige partnertaken 

De toekomstige partner van het abonnement moet een overdrachtsaanvraagformulier van de Partner Center om een abonnementsoverdracht aan te vragen:

1.  Selecteer in het linkerdeelvenster Partner Center klanten **en** selecteer vervolgens de klant voor wie u de overdrachtsaanvraag wilt voltooien.
2.  Selecteer Abonnementen in het specifieke menu **van de klant.**
3.  Selecteer op **het tabblad Overdrachtsaanvragen** **de optie Nieuwe aanvraag toevoegen:**

    :::image type="content" source="images/modernazuretransfers/Transferrequestheader.png" alt-text="Schermopname van het tabblad Overdrachtsaanvragen.":::

5.  Vul het **formulier Nieuwe overdrachtsaanvraag** in:

    :::image type="content" source="images/modernazuretransfers/CompleteTrnasferRequestForm.png" alt-text="Schermopname van het formulier Nieuwe overdrachtsaanvraag.":::

6.  Selecteer **Overdrachtsaanvraag verzenden**  >  **Verzenden.**

7.  Controleer de bevestiging van de overdrachtsaanvraag:

    :::image type="content" source="images/modernazuretransfers/TransferPending.png" alt-text="Schermopname met een bevestiging van een overdrachtsaanvraag.":::

    > [!NOTE]
    > De toekomstige partner kan de overdrachtsaanvraag annuleren door **Aanvraag** annuleren alleen in de rechterbovenhoek van het venster te selecteren wanneer de status van de overdrachtsaanvraag 'in behandeling' is. Nadat de status van de overdrachtsaanvraag 'wordt uitgevoerd' of 'voltooid' is, zijn annuleringen niet mogelijk.

## <a name="current-partner-tasks"></a>Huidige partnertaken 

De beheerderagent van de huidige partner voor de klant ontvangt een e-mail met de mededeling dat een klant een overdracht van abonnementen aanvraagt:

:::image type="content" source="images/modernazuretransfers/SourceReviewEmail.png" alt-text="Schermopname van een e-mailmelding van een klantaanvraag voor overdracht.":::

De huidige partner moet het formulier voor de overdrachtsaanvraag van de Partner Center om de abonnementsoverdracht te voltooien.

> [!NOTE]  
> Als de huidige partner niet binnen 30 dagen reageert, verloopt de aanvraag en moet de toekomstige partner een nieuwe overdrachtsaanvraag maken.

1. Ga in dat geval op een van de volgende manieren te werk: 
   - Selecteer **Overdrachtsaanvraag controleren** in het e-mailbericht.

     of

    - Selecteer in het linkerdeelvenster Partner Center klanten **en** selecteer vervolgens de klant voor wie de overdrachtsaanvraag is ingediend.
      1. Selecteer Abonnementen in het specifieke menu **van de klant.**
      1. Vouw op **het tabblad Overdrachtsaanvragen** de overdrachtsgegevens uit door onder Ontvangen aanvragen de id van de **overdrachtsaanvraag** **te selecteren:**

      :::image type="content" source="images/modernazuretransfers/ReviewRequest.png" alt-text="Schermopname van het tabblad Overdrachtsaanvragen, zoals wordt weergegeven door de huidige partner.":::

5. Controleer de overdrachtsaanvraag. Selecteer de aangevraagde Azure-abonnementen die u wilt overdragen.
 
   Voordat u doorgaat, moet u het volgende weten:
   - U hebt geen toegang meer tot de geselecteerde abonnementen.
   - U wordt niet gefactureerd voor verder gebruik.
   - Azure-reserveringen worden niet overdraagt met abonnementen.

6. Selecteer **Accepteren en overdragen om** het overdrachtsproces te voltooien:

   :::image type="content" source="images/modernazuretransfers/SelectSubs.png" alt-text="Schermopname van het scherm Overdrachtsaanvraag controleren.":::

   Als u een klant hebt met eerdere Azure-aanbiedingsabonnementen (MS-AZR-0145p), gaat u  op dezelfde manier door, kiest u de abonnementen die u wilt overdragen en selecteert u Accepteren en overdragen om het overdrachtsproces te voltooien.

7. Bekijk de bevestiging dat de overdracht is geaccepteerd.

   Op dit moment worden de toekomstige partner, de klant en de huidige partner via een e-mail op de hoogte gehouden van de geaccepteerde overdrachtsaanvraag.

   Nadat de overgang is geaccepteerd, kan de overdrachtsstatus maximaal 15 minuten in behandeling blijven terwijl het systeem wordt bijgewerkt. Als dit proces langer duurt, blijft het systeem het drie dagen proberen. Als de overdrachtsstatus langer dan drie dagen in behandeling blijft, moet de partner een serviceaanvraag indienen.

   Nadat de overdracht is voltooid, worden de abonnementen die zijn opgenomen in de aanvraag weergegeven in het Azure-plan van de toekomstige partner. Deze wordt niet meer vermeld bij de huidige partner.

>[!Note]  
>Indirecte providers moeten hun indirecte resellers informeren dat de overdrachtsaanvraag is geaccepteerd.

### <a name="managing-your-transferred-customer-subscriptions"></a>Uw overgedragen klantabonnementen beheren

Toegang tot bestaande gebruikers, groepen of service-principals die zijn toegewezen via Azure RBAC wordt niet beïnvloed tijdens de overgang. [Met Azure RBAC](/azure/role-based-access-control/overview) kan uw klant beheren wie toegang heeft tot Azure-resources, wat ze kunnen doen met deze resources en tot welke gebieden ze toegang hebben. 

Als nieuwe partner hebt u geen RBAC-toegang tot de resources van uw klant na de abonnementsoverdracht. De vorige partner van uw klant behoudt RBAC-toegang. Werk samen met uw klant om te begrijpen wie inzicht heeft in de abonnementen en hoe u eventuele benodigde wijzigingen kunt aanbrengen.

Uw klant moet Azure RBAC-toegang voor de vorige partner verwijderen en toegang voor u toevoegen. Zie Wat is op rollen gebaseerd toegangsbeheer van [Azure (Azure RBAC)?](/azure/role-based-access-control/overview)voor meer informatie over het bieden van toegang. Zie Een roltoewijzing verwijderen voor meer informatie [over het verwijderen van toegang.](/azure/role-based-access-control/role-assignments-portal#remove-a-role-assignment)

Bovendien krijgt u niet automatisch [AOBO-toegang (Admin on Behalf Of)](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO) tot uw abonnementen. AOBO is nodig zodat u de Azure-abonnementen van uw klant kunt beheren. Zie voor meer informatie over Azure-machtigingen [Machtigingen verkrijgen voor het beheren van de service of het abonnement van een klant](./customers-revoke-admin-privileges.md).

## <a name="next-steps"></a>Volgende stappen

- [Azure RBAC](/azure/role-based-access-control/overview)
- [Machtigingen verkrijgen voor het beheren van de service of het abonnement van een klant](./customers-revoke-admin-privileges.md)

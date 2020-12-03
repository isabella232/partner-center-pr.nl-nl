---
title: Klanten verplaatsen van huidige Azure-aanbiedingen naar Azure-abonnement
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe CSP-partners partner centrum kunnen gebruiken om klanten te verplaatsen van bestaande CSP Azure-aanbiedingen naar Azure-Services onder het Azure-abonnement.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: 4e22386dc8bddd9662a0d80020a5c90c464e9d39
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534808"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Klanten van de overstap naar Azure plannen van bestaande CSP Azure-aanbiedingen

**Juiste rollen**

- Beheer agent
- Factureringsbeheerder
- Globale beheerder
- Helpdesk medewerker
- Verkoop agent
- Beheerder van gebruikers beheer

In dit artikel wordt uitgelegd hoe CSP-partners partner centrum kunnen gebruiken om klanten te verplaatsen van bestaande CSP Azure-aanbiedingen naar Azure-Services onder het Azure-abonnement. Indirecte providers en directe factuur partners kunnen overstappen op de nieuwe Commerce-ervaring die beschikbaar is in het Microsoft Cloud service provider-programma (CSP) voor Azure. (Indirecte wederverkopers moeten door hun indirecte providers werken.) Klanten hebben een gestroomlijnde manier om Cloud Services te kopen, of ze aankopen van partners, van micro soft-verkopers of rechtstreeks op internet.

De overgangs mogelijkheid is alleen voor klanten die overstappen naar de nieuwe Commerce-ervaring voor Azure en die de micro soft-klant overeenkomst hebben ondertekend. Het is niet voor andere aanbiedingen in CSP, zoals Office 365 of Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Bestaande CSP-aanbiedingen overzetten naar een Azure-abonnement

U kunt vanuit Partner Center een klant vanuit hun bestaande CSP Azure-aanbiedingen naar Azure-Services onder het Azure-abonnement laten overstappen in de nieuwe Commerce-ervaring van het CSP-programma. Om dit te doen, moet de partner en de klant een gevestigde wederverkoper-relatie hebben via het partner centrum en moet de klant de micro soft-klant overeenkomst hebben ondertekend.

### <a name="select-transition-to-azure-plan"></a>Overgang naar Azure-abonnement selecteren

1. Selecteer Azure-abonnement voor uw klant.

2. Selecteer **overgangs facturering naar Azure-abonnement**.

   :::image type="content" source="images/azure/transition1.png" alt-text="Scherm opname van rapport met op gebruik gebaseerde abonnementen met een optie die kan worden geselecteerd: overgang van Azure-abonnement naar Azure-plan.":::

3. Selecteer **Doorgaan**

   :::image type="content" source="images/azure/transition2.png" alt-text="Dialoog venster met de titel overgang naar Azure plan met implicaties voor het lezen van de overgang en twee opties om te selecteren, door te gaan of te annuleren.":::

   Uw klant wordt overgezet naar het Azure-abonnement.

   **De overgangs werk stroom automatiseert de vereiste stappen**:

   - Aankoop van Azure-abonnement (en)
   - Eén abonnement per klant in directe CSP-scenario's  
   - Eén abonnement per wederverkoper  

   Een partner heeft bijvoorbeeld twee Microsoft Azure-aanbiedingen aangeschaft en heeft twee verschillende POR-producten in de aankoop opgenomen. In dit geval koopt de overgangs werk stroom twee Azure-abonnementen (één per wederverkoper) en worden de betreffende Azure-abonnementen automatisch toegewezen onder de Azure-plannen.  

   **Azure-abonnement koppelen aan Azure-plan**

   Na uw aankoop van een Azure-abonnement worden de bestaande Azure-abonnementen toegewezen aan de Azure-plannen. De voortgang kan worden weer gegeven in Azure Portal en in partner centrum.

4. Ga terug naar de **abonnementen** pagina van uw klant om de budget limiet bij te werken met behulp van de lokale valuta.

   :::image type="content" source="images/azure/transition3.png" alt-text="Gedeeltelijke weer gave van de pagina Abonnementen van partner Center met budget limieten die zijn ingesteld in de lokale valuta voor een facturerings periode.":::

   >[!NOTE]
   >Het budget dat u in het partner centrum instelt, wordt niet overgedragen naar de Azure Portal. U moet ook het budget en de waarschuwing in Azure Portal instellen.

   Wanneer u naar het Azure-abonnement gaat, kunt u geen Azure-abonnementen meer kopen voor deze klant. U maakt de abonnementen onder het Azure-abonnement in de Azure Portal.

   >[!NOTE]
   > Alle Azure-abonnementen die zijn aangeschaft via RBAC onder het Azure-abonnement, worden in rekening gebracht en gefactureerd in de lokale valuta. FX-tarieven worden niet gebruikt.

### <a name="track-your-transition-details"></a>Uw overgangs gegevens bijhouden

Volg de overgangs voortgang in Azure Portal en in partner centrum.

:::image type="content" source="images/azure/details1.png" alt-text="Scherm afbeelding met een tabel met een lijst met overgangs gegevens per abonnement: bevat abonnements-I D, overgangs datum en overgangs status.":::

### <a name="billing-impact-to-partners"></a>Facturering van gevolgen voor partners

Als u een klant overstapt van een bestaande CSP Azure-aanbieding, hebt u de volgende facturerings effecten:

- U wordt gefactureerd op uw bestaande CSP-factuur voor al het gebruik tot het moment waarop het oorspronkelijke CSP Azure-abonnement wordt afgesloten.

- Als u beheerders toegangs rechten had voor het bestaande CSP-abonnement, hebt u nog steeds toegang tot het abonnement dat wordt gemigreerd.

Als u direct Enter prise agreements wilt overzetten naar CSP-en server-en Cloud registraties voor Azure-Services, raadpleegt u het [eigendom van het gebruik van Azure-abonnementen voor micro soft Partner Agreement](/azure/billing/mpa-request-ownership)

### <a name="audit-log"></a>Auditlogboek

Als u de facturering wilt afstemmen, bekijkt u de geschiedenis van de abonnementen ' Microsoft Azure ' (0145P) op de pagina **abonnementen** .

Het abonnement Microsoft Azure (0145P) bestaat uit twee delen:

1. Commerce-abonnement
2. Azure-abonnement (recht)

Wanneer de overgang is voltooid, wordt het Azure-abonnement verplaatst onder het nieuwe Azure-plan en wordt het Commerce-abonnement opgeschort zodat er geen verdere gebruik wordt gerapporteerd.  

>[!NOTE]
>Als Microsoft Azure-abonnement (0145P) wordt aangeschaft in CSP, hebben zowel het Commerce-abonnement als het Azure-abonnement (recht) dezelfde waarde. De waarde is alleen van toepassing op wijzigingen in de facturerings eigendom of overdrachten.

### <a name="transition-issues"></a>Overgangs problemen

We anticiperen geen problemen tijdens de overgangen. Als er een fout optreedt, wordt u in de overgangs werk stroom zelf bijgewerkt. Er zijn geen storingen in het gebruik van Azure.  

## <a name="next-steps"></a>Volgende stappen

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)

- [Creditering van de partner-overzicht](partner-earned-credit.md)
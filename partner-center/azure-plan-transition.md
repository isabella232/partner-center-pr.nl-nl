---
title: Klanten verplaatsen van huidige Azure-aanbiedingen naar Azure-plan
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over hoe CSP-partners Partner Center om klanten te verplaatsen van bestaande CSP Azure-aanbiedingen naar Azure-services onder het Azure-plan.
author: mowree
ms.author: mowrim
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/16/2020
ms.openlocfilehash: eb9d88935bdc339c01ac47153c3d4a23047dc406
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123956887"
---
# <a name="transition-customers-to-azure-plan-from-existing-csp-azure-offers"></a>Klanten overstappen op Een Azure-abonnement overstappen van bestaande CSP Azure-aanbiedingen

**Van toepassing op**: Partner Center 

**Juiste rollen:** beheeragent | Factureringsbeheerders | Globale | Helpdeskagent | Verkoopagent | Beheerder van gebruikersbeheer

In dit artikel wordt uitgelegd hoe CSP-partners Partner Center om klanten te verplaatsen van bestaande CSP Azure-aanbiedingen naar Azure-services onder het Azure-plan. Indirecte providers en directe factuurpartners kunnen overstappen op de nieuwe commerce-ervaring die beschikbaar is in het Microsoft Cloud Service Provider Program (CSP) voor Azure. (Indirecte resellers moeten via hun indirecte providers werken.) Klanten hebben een gestroomlijnde manier om cloudservices te kopen, of het nu gaat om aankopen van partners, microsoft-verkopers of rechtstreeks op internet.

De overgangsmogelijkheid is alleen beschikbaar voor klanten die overstappen op de nieuwe commerce-ervaring voor Azure en die de Microsoft-klantovereenkomst. Het is niet voor andere aanbiedingen in CSP, zoals Office 365 of Dynamics 365.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Bestaande CSP-aanbiedingen overstappen naar een Azure-plan

In de nieuwe commerce-ervaring van het CSP-programma kunt u een klant vanuit het CSP-programma overstappen van hun bestaande CSP Azure-aanbiedingen naar Azure-services onder het Azure-Partner Center. Hiervoor moeten de partner en de klant een bestaande resellerrelatie hebben via Partner Center en moet de klant de Microsoft-klantovereenkomst.

### <a name="select-transition-to-azure-plan"></a>Overgang naar Azure-plan selecteren

1. Selecteer Azure-plan voor uw klant.

2. Selecteer **Facturering overstappen naar Azure-abonnement.**

   :::image type="content" source="images/azure/transition1.png" alt-text="Schermopname van rapportgegevens over op gebruik gebaseerde abonnementen met een selecteerbare optie met de naam: Facturering van Azure-abonnement overstappen op Azure-abonnement.":::

3. Selecteer **Doorgaan**

   :::image type="content" source="images/azure/transition2.png" alt-text="Dialoogvenster met de titel Overgang naar Azure-plan met gevolgen voor meer informatie over de overgang en twee opties om te selecteren, Doorgaan of Annuleren.":::

   Uw klant wordt overgestappen naar het Azure-plan.

   **De overgangswerkstroom automatiseert de vereiste stappen:**

   - Aankoop van Azure-abonnement(en)
   - Eén plan per klant in directe CSP-scenario's  
   - Eén abonnement per reseller  

   Een partner heeft bijvoorbeeld twee verschillende aanbiedingen Microsoft Azure en heeft twee afzonderlijke SOORTEN in de aankoop opgenomen. In dit geval koopt de overgangswerkstroom twee Azure-abonnementen (één per reseller) en worden de respectieve Azure-abonnementen automatisch onder de Azure-abonnementen in kaart gebracht.  

   **Azure-abonnement toewijzen aan Azure-plan**

   Na de aankoop van een of meer Azure-abonnementen worden de bestaande Azure-abonnementen door ons systeem aan de Azure-abonnementen toe te staan. De voortgang kan worden bekeken in Azure Portal en in het Partnercentrum.

4. Ga terug naar de pagina met Partner Center **van uw** klant om de budgetlimiet bij te werken met behulp van hun lokale valuta.

   :::image type="content" source="images/azure/transition3.png" alt-text="Gedeeltelijke weergave van Partner Center abonnementen met budgetlimieten die zijn ingesteld in lokale valuta voor een factureringsperiode.":::

   >[!NOTE]
   >Het budget dat u in de Partner Center, wordt niet naar de Azure Portal. U moet ook het budget en de waarschuwing instellen in Azure Portal.

   Wanneer u overstapt op het Azure-abonnement, kunt u geen Azure-abonnementen meer aanschaffen voor deze klant. U maakt de abonnementen onder het Azure-plan in de Azure Portal.

   >[!NOTE]
   > Alle Azure-abonnementen die zijn aangeschaft via RBAC onder het Azure-plan, worden in lokale valuta gefactureerd. FX-tarieven worden niet gebruikt.

### <a name="track-your-transition-details"></a>Uw overgangsdetails bijhouden

Volg de voortgang van de overgang in Azure Portal en in Partner Center.

:::image type="content" source="images/azure/details1.png" alt-text="Schermopname van een tabel met een lijst met overgangsdetails per abonnement, inclusief abonnements-ID, overgangsdatum en overgangsstatus.":::

### <a name="billing-impact-to-partners"></a>Gevolgen voor de facturering voor partners

Als u een klant over overstapt van een bestaande CSP Azure-aanbieding, heeft dit de volgende gevolgen voor de facturering:

- U wordt gefactureerd op uw bestaande CSP-factuur voor al het gebruik tot het moment van afsluiten van het oorspronkelijke CSP Azure-abonnement.

- Als u beheerderstoegangsrechten voor het bestaande CSP-abonnement hebt, hebt u nog steeds toegang wanneer dat abonnement wordt gemigreerd.

Als u directe Enterprise Agreements wilt overstappen op CSP- en Server- en Cloud-inschrijvingen naar Azure-services, leest u Eigendom van facturering van [Azure-abonnementen](/azure/billing/mpa-request-ownership) Microsoft Partner-overeenkomst

### <a name="audit-log"></a>Auditlogboek

Als u facturering wilt afstemmen, bekijkt u uw geschiedenis van Microsoft Azure (0145P) abonnementen op **de pagina** Abonnementen.

Het Microsoft Azure (0145P) bestaat uit twee delen:

1. Commerce-abonnement
2. Azure-abonnement (rechten)

Wanneer de overgang is voltooid, wordt het Azure-abonnement verplaatst naar een nieuw Azure-plan en wordt het commerce-abonnement tijdelijk opgeschort, zodat er geen verder gebruik wordt gerapporteerd.  

>[!NOTE]
>Wanneer Microsoft Azure abonnement (0145P) wordt aangeschaft in CSP, hebben zowel het commerce-abonnement als het Azure-abonnement (rechten) dezelfde waarde. De waarden verschillen alleen in het geval van wijzigingen in het eigendom van facturering of overdrachten.

### <a name="transition-issues"></a>Overgangsproblemen

We verwachten geen problemen tijdens overgangen. Als er een plaatsvindt, wordt u bijgewerkt in de overgangswerkstroom zelf. Er zijn geen zorgen over het gebruik van Azure.  

## <a name="next-steps"></a>Volgende stappen

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)

- [Partnertegoed - overzicht](partner-earned-credit.md)

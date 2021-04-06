---
title: Laat klanten hun eigen services in CSP kopen
description: Meer informatie over hoe CSP-programma partners klanten hun eigen services kunnen laten kopen, zoals Azure-reserve ringen, voor een abonnement dat hiervoor is aangeschaft in Partner Center.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 4feaa8cba8ba17f553b5e936dcf892ffbf7ccc82
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441299"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Geef klanten toestemming in het partner centrum om hun eigen producten of services te kopen

**Juiste rollen**

- Beheer agent
- Verkoop agent

In dit artikel wordt uitgelegd hoe een partner in het programma Cloud Solution Provider (CSP) een klant toestemming kan geven om sommige van hun eigen services of resources te kopen.

Partners in het CSP-programma gebruiken vaak het partner centrum en de commerciële Marketplace om oplossingen en services voor hun klanten te kopen. Partners hebben vervolgens een aantal klanten de mogelijkheid om deze services rechtstreeks vanuit de Azure Portal in te richten.

Hier volgt een voorbeeld. Stel dat u een abonnement voor Azure-abonnementen aanschaft voor een klant in het partner centrum. Vervolgens besluit u andere resources of services toe te voegen aan dat abonnement namens de klant. In dit geval kunt u Azure-reserve ringen toevoegen aan het abonnement van de klant (zoals het toevoegen van gereserveerde instanties van virtuele machines). U kunt de klant vervolgens toestaan de Azure-reserve ring resources zelf in de Azure Portal in te richten.

Met de functie voor **klant machtigingen** geeft u klanten nu meer selfservice opties met Azure-resources. Door de machtigingen voor de klant in te scha kelen, kunnen klanten hun eigen resources kopen (zoals en hun eigen Azure-reserve ringen kopen).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Overzicht van klant machtigingen in partner centrum

Gebruik de pagina klant **account** om klant machtigingen in te scha kelen (of uit te scha kelen). Deze functie ondersteunt momenteel:

- **Azure-reserve ringen:** Door deze machtiging in te scha kelen, kan de klant hun eigen Azure-reserve ringen kopen voor een specifiek Azure-abonnement dat u hebt aangeschaft.

Houd rekening met de volgende belang rijke punten voordat u de machtigingen van de klant inschakelt:

- Standaard worden klant machtigingen automatisch uitgeschakeld (uitgeschakeld) in partner centrum.

- Voordat u machtigingen voor een klant kunt inschakelen of uitschakelen, moet u de rol van beheer agent in het partner centrum toewijzen.

  Partners die de rol van de verkoop agent of de helpdesk medewerker hebben toegewezen, hebben alleen-lezen toegang en kunnen geen klant machtigingen in-of uitschakelen.

- U kunt machtigingen voor elke klant die u kiest, inschakelen.

- U kunt klant machtigingen inschakelen (of uitschakelen) met behulp van het dash board van de partner centrum of het [partner centrum-api's](/partner-center/develop/manage-customers).

- Nadat u de machtigingen voor een specifieke klant hebt ingeschakeld, moet u betalen voor latere aankopen door die klant. Als klanten willen worden uitgewisseld, moet ik een aankoop annuleren of vernieuwen die ze hebben ondergaan (of het oorspronkelijke bereik van een reserve ring willen wijzigen), ze kunnen dit niet zelf doen. Ze moeten u als partner vragen om hen te helpen bij het uitwisselen, annuleren en vernieuwen van aankopen, of om later wijzigingen aan te brengen in een reserverings bereik.  

- Nadat u de machtigingen voor een specifieke klant hebt ingeschakeld, wordt u **niet** op de hoogte gesteld van latere aankopen door de klant.

- Latere aankopen door de klant worden weer gegeven in het partner centrum, samen met alle aankopen die door u zijn gedaan. U kunt deze aankopen vinden op de pagina **order geschiedenis** van de klant, de pagina **reserve ringen** of in het [**activiteiten logboek**](activity-logs.md).

>[!NOTE]
> Voor informatie over de prijzen die de klant betaalt en hoe u klanten helpt hun aankopen te beheren, [kunt u klanten helpen bij het beheren van reserve ringen die door hen worden gekocht](give-customers-permission.md#help-customers-manage-reservations-they-purchase).

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Geef klanten toestemming om hun eigen Azure-reserve ringen te kopen

Azure-reserve ringen zijn een uitstekende manier om Azure-Services te kopen tegen een kortings bedrag. Zie [Wat zijn Azure Reservations?](/azure/cost-management-billing/reservations/save-compute-costs-reservations) voor meer informatie over de voor delen van Azure-reserve ringen.

U hebt nu de keuze om Azure-reserve ringen namens uw klanten te kopen, omdat u deze mogelijk al hebt gedaan. U kunt ook klanten toestemming geven om hun eigen Azure-reserve ringen te kopen.

>[!NOTE]
> Nadat u klanten toestemming geeft om hun eigen Azure-reserve ringen te kopen, helpen ze bij het beheren van de reserve ringen die ze aanschaffen. Zie [Help klanten reserve ringen beheren die ze kopen](give-customers-permission.md#help-customers-manage-reservations-they-purchase)voor meer informatie.

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Klanten in staat stellen hun eigen Azure-reserve ringen te kopen

1. Controleer of de klant over een bestaand Azure-abonnement of een Azure Global Subscription beschikt dat u namens hen hebt gekocht.

2. Controleer of aan de klant de rol van **eigenaar** voor dit abonnement is toegewezen.

3. Schakel klant machtigingen in (Schakel deze functie **in**) om hun eigen Azure-reserve ringen te kopen.

Elke stap wordt hieronder weer gegeven.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Controleren of de klant een bestaand Azure-abonnement heeft

Voordat u klanten toestemming geeft om hun eigen Azure-reserve ringen te kopen, moet u controleren of de klant over een bestaand Azure-abonnement of een globaal Azure-abonnements beschikt. Als de klant geen huidig Azure-abonnement in het partner centrum ziet, moet u een abonnement voor hen aanschaffen voordat u de machtigingen van de klant inschakelt.

- Als u wilt weten of een klant al een Azure-abonnement heeft, meldt u zich aan bij het dash board van het partner centrum en selecteert u vervolgens **CSP** , gevolgd door **klanten**. Selecteer de specifieke klant in de lijst. Selecteer vervolgens **abonnementen** en zoek naar alle op gebruik gebaseerde abonnementen voor Azure plan of Azure Global.

- Als een klant geen bestaand Azure-abonnement heeft, kunt u een abonnement voor hen kopen. Zie [het Azure-abonnement kopen](purchase-azure-plan.md).

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Controleer of aan de klant de juiste functie is toegewezen in azure

Nadat u hebt gecontroleerd of de klant een bestaand Azure-abonnement heeft, moet u ook controleren of aan de belangrijkste gebruikers die aan uw klant zijn gekoppeld, de juiste **eigenaar** van het Azure-abonnement is toegewezen. Dit is de op rollen gebaseerde toegang (RBAC) die de klant nodig heeft om Azure-reserve ringen te kopen voor een Azure-abonnement dat u hebt aangeschaft.

Sommige partners hebben de rol van **eigenaar** mogelijk al toegewezen aan klanten die actief moeten zijn om hun eigen Azure-resources te beheren en in te richten. Als u al **eigenaars** status aan een klant hebt toegewezen voor het beheren van eerdere abonnementen die u hebt aangeschaft, kunt u deze stap overs Laan.  

> [!IMPORTANT]
> Als aan een klant niet de rol van **eigenaar** is toegewezen, wordt er een fout melding weer gegeven in de Azure portal voor komen dat ze Azure-reserve ringen kopen.

Om te controleren of de klant is toegewezen aan de rol van **eigenaar** voor een Azure-abonnement:

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.

2. Selecteer **CSP**, vervolgens **klanten** en selecteer de specifieke klant.

3. Selecteer **abonnementen** voor die klant en zoek het specifieke Azure-abonnement.

4. Selecteer de knop **beheren** naast het abonnement van de klant. Hiermee opent u de [Azure Portal](https://portal.azure.com/).

5. Als u de rol van **eigenaar** aan een specifieke gebruiker wilt toewijzen, volgt u deze stappen [om een gebruiker toe te wijzen als beheerder](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator).

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Het inschakelen of uitschakelen van de machtigingen van de klant om hun eigen Azure-reserve ringen te kopen

Nadat u hebt gecontroleerd of de klant een bestaand Azure-abonnement heeft en er gebruikers zijn toegewezen aan de rol van **eigenaar** voor dat abonnement, bent u klaar om de klant machtigingen in te scha kelen. U kunt deze stappen ook gebruiken om klant machtigingen uit te scha kelen. U kunt klant machtigingen in-of uitschakelen met behulp van het dash board van de partner centrum of het [partner centrum-api's](/partner-center/develop/manage-customers).

U kunt als volgt de toestemming van de klant in het partner centrum inschakelen (of uitschakelen):

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.

2. Selecteer in het navigatie menu aan de linkerkant **CSP** en vervolgens **klanten**. Er wordt een klanten lijst weer gegeven.

3. Selecteer een specifieke klant naam.

4. Selecteer **account** in het menu van de klant. De pagina klant **account** wordt weer gegeven.

5. Ga naar het gebied met **klant machtigingen** onder aan de pagina.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Pagina klant machtigingen op account." border="true":::

6. Zoek onder **Azure-reserve ringen** de optie **klant naar aankoop toestaan** .

7. Als u de machtigingen van de klant wilt inschakelen, verplaatst u de switch naast deze optie naar de **op** positie. Als u de machtigingen van klanten wilt uitschakelen, verplaatst u de switch naar de **uit** .

>[!NOTE]
> Voor meer informatie over wat er gebeurt wanneer u de machtigingen van een klant inschakelt om hun eigen Azure-reserve ringen te kopen, raadpleegt u [overzicht van klant machtigingen in partner centrum](give-customers-permission.md#overview-of-customer-permissions-in-partner-center).
>
>Wanneer u de klant machtigingen inschakelt (of uitschakelt), registreert het activiteiten logboek elke actie. (Dit logboek is toegankelijk wanneer u het tandwiel pictogram van de bovenkant van het dash board van partner Center selecteert). Wanneer u de machtigingen van de klant in-of uitschakelt, wordt de actie weer gegeven als ofwel **klant aankoop machtigingen maken** of **klant aankoop machtigingen verwijderen** in het activiteiten logboek.

## <a name="help-customers-manage-reservations-they-purchase"></a>Help klanten bij het beheren van reserve ringen die ze kopen

Zodra u klanten toestemming geeft om hun eigen Azure-reserve ringen te kopen, kunt u hen helpen bij het beheren van de resources die ze kopen. Klanten kunnen veel aspecten van Azure-reserve ringen zelf rechtstreeks vanuit de [Azure Portal](https://portal.azure.com/)beheren. Ze hebben uw hulp nodig bij het beheren van enkele, andere aspecten van Azure-reserve ringen die in uw CSP-abonnement worden aangeschaft.  

Help klanten meer te weten over het beheren van deze aspecten van Azure-reserve ringen:

- Prijzen klanten betalen voor Azure-reserve ringen
- Hoe klanten het gebruik van Azure-reserve ringen kunnen optimaliseren
- Wat gebeurt er wanneer klanten reserve ringen kopen met een gedeeld bereik?
- Wat gebeurt er als klanten een reserve ring willen wijzigen, annuleren en vernieuwen, of het bereik wijzigen?

**Prijzen klanten betalen voor hun reserve ringen.** Uw klant zal Azure-reserve ringen kopen op basis van een abonnement dat u eerder hebt gekocht in de facturerings account van de CSP-partner. De prijs van de klant voor alle Azure-reserve ringen die worden aangeschaft op basis van dit abonnement, wordt ook door u ingesteld. Deze prijs kan afwijken van de Web-directe prijs die de klant in de Azure Portal ziet.

**Hoe klanten hun gebruik van een reserve ring kunnen optimaliseren.** Sommige klanten kunnen profiteren van meer informatie over het optimaliseren van het gebruik van een reserve ring of het toewijzen van het oorspronkelijke bereik van een reserve ring tijdens de aankoop. Vraag klanten om de [reserve ringen voor Azure-resources te beheren](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)voor meer informatie.

**Wat gebeurt er wanneer een klant een reserve ring koopt met een gedeeld bereik?** Wanneer klanten een reserve ring kopen op basis van een voor gaande CSP-abonnement en een gedeeld bereik aan deze reserve ring toewijzen, worden eventuele kortingen die de klant heeft gegeven door de CSP, toegepast op het overeenkomende gebruik voor alle abonnementen die de CSP-partner voor die klant heeft gekocht.

**Wat moeten klanten doen als ze een aankoop willen uitwisselen, annuleren of vernieuwen, of het oorspronkelijke bereik van een reserve ring wijzigen?** Klanten moeten hun partner vragen om hen te helpen bij het wijzigen van het oorspronkelijke bereik van de reserve ring. Ze hebben ook de hulp van een partner nodig om een reserve ring uit te wisselen, te annuleren of te vernieuwen. Deze taken kunnen niet worden uitgevoerd met reserve ringen op basis van abonnementen die voor hen zijn aangeschaft door een CSP-partner.

## <a name="next-steps"></a>Volgende stappen

- [Azure-reserve ringen namens uw klanten kopen](azure-reservations-buying.md)

- [Partner centrum-micro soft-reserve ringen verkopen](azure-reservations.md)

- [Azure-reserve ringen namens uw klanten beheren](azure-reservations-manage.md)
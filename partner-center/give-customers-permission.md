---
title: Laat klanten hun eigen services kopen in CSP
description: Ontdek hoe klanten met CSP-programmapartners hun eigen services, zoals Azure-reserveringen, kunnen kopen voor een abonnement dat voor hen is gekocht in Partner Center.
ms.topic: how-to
ms.date: 05/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: aced617bbe46465d9a82478a41b2f1c4a05309be
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841416"
---
# <a name="give-customers-permission-in-partner-center-to-buy-their-own-products-or-services"></a>Klanten toestemming geven in Partner Center eigen producten of services te kopen

**Juiste rollen:** beheeragent | Verkoopagent

In dit artikel wordt beschreven hoe een partner in het Cloud Solution Provider (CSP)-programma een klant toestemming kan geven om bepaalde eigen services of resources te kopen.

Partners in het CSP-programma gebruiken vaak Partner Center en de commerciële marketplace om oplossingen en services voor hun klanten te kopen. Partners bieden sommige klanten vervolgens de mogelijkheid om deze services rechtstreeks vanuit de Azure Portal.

Hier volgt een voorbeeld. Stel dat u een Azure-abonnement koopt voor een klant in Partner Center. Vervolgens besluit u namens de klant andere resources of services aan dat abonnement toe te voegen. In dit geval kunt u Azure-reserveringen toevoegen aan het abonnement van de klant (zoals het toevoegen van gereserveerde instanties van virtuele machines). U kunt de klant vervolgens toestaan om de Azure-reserveringsbronnen zelf in te Azure Portal.

Met de functie **Klantmachtigingen** geeft u klanten nu meer selfserviceopties met Azure-resources. Door machtigingen voor de klant in te stellen, kunt u klanten toestaan om hun eigen resources te kopen (zoals het kopen van hun eigen Azure-reserveringen).  

## <a name="overview-of-customer-permissions-in-partner-center"></a>Overzicht van klantmachtigingen in Partner Center

Gebruik de pagina **Klantaccount** om klantmachtigingen in te schakelen (of uit te schakelen). Deze functie ondersteunt momenteel:

- **Azure-reserveringen:** Als u deze machtiging int, kan de klant zijn eigen Azure-reserveringen aanschaffen voor een specifiek Azure-abonnement dat u voor hen hebt aangeschaft.

Voordat u klantmachtigingen in gaat zetten, moet u rekening maken met de volgende belangrijke punten:

- Standaard worden klantmachtigingen automatisch uitgeschakeld (uitgeschakeld) in Partner Center.

- Voordat u machtigingen voor een klant kunt in- of uitschakelen, moet aan u de rol van beheerderagent zijn toegewezen in Partner Center.

  Partners die de rol verkoopagent of helpdeskmedewerker hebben toegewezen, hebben alleen-lezentoegang en kunnen geen klantmachtigingen in- of uitschakelen.

- U kunt machtigingen inschakelen (inschakelen) voor elke klant die u kiest.

- U kunt klantmachtigingen in- of uitschakelen met behulp van het Partner Center dashboard of [Partner Center API's.](/partner-center/develop/manage-customers)

- Nadat u machtigingen voor een specifieke klant hebt ingeschakeld (ingeschakeld), bent u verantwoordelijk voor het betalen voor alle volgende aankopen die door die klant zijn gedaan. Als klanten een aankoop die ze hebben gedaan willen inruilen, annuleren of vernieuwen (of als ze het initiële bereik van een reservering willen wijzigen), kunnen ze dit niet zelf doen. Ze moeten u als partner vragen om ze te helpen bij het inruilen, annuleren en vernieuwen van aankopen, of om later wijzigingen aan te brengen in het bereik van een reservering.  

- Nadat u machtigingen voor een specifieke  klant hebt in gebruik genomen, wordt u niet op de hoogte gesteld van latere aankopen van de klant.

- Latere aankopen die door de klant worden gedaan, worden weergegeven in Partner Center alle aankopen die u hebt gedaan. U vindt deze aankopen op de  pagina Ordergeschiedenis  van de klant, de pagina Reserveringen van de klant of in het [**activiteitenlogboek.**](activity-logs.md)

>[!NOTE]
> Zie Klanten helpen bij het beheren van reserveringen die ze kopen voor meer informatie over prijzen die de klant zal betalen en hoe klanten hun aankopen [kunnen beheren.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

## <a name="give-customers-permission-to-buy-their-own-azure-reservations"></a>Klanten toestemming geven om hun eigen Azure-reserveringen te kopen

Azure-reserveringen zijn een uitstekende manier om Azure-services te kopen tegen een gereduceerd tarief. Zie Wat zijn Azure-reserveringen? voor meer informatie over de voordelen [van Azure-reserveringen.](/azure/cost-management-billing/reservations/save-compute-costs-reservations)

Nu hebt u de keuze om Azure-reserveringen te kopen namens uw klanten, zoals u mogelijk al hebt gedaan. U kunt klanten ook toestemming geven om hun eigen Azure-reserveringen te kopen.

>[!NOTE]
> Nadat u klanten toestemming hebt gegeven om hun eigen Azure-reserveringen te kopen, helpt u hen bij het beheren van de reserveringen die ze aanschaffen. Zie Klanten helpen bij [het beheren van reserveringen die ze kopen voor meer informatie.](give-customers-permission.md#help-customers-manage-reservations-they-purchase)

### <a name="to-enable-customers-to-buy-their-own-azure-reservations"></a>Klanten in staat stellen hun eigen Azure-reserveringen te kopen

1. Controleer of de klant een bestaand Azure-abonnement of Azure Global-abonnement heeft dat u namens hem of haar hebt aangeschaft.

2. Controleer of aan de klant de rol Van **eigenaar is** toegewezen voor dit abonnement.

3. Schakel klantmachtigingen in (schakel deze functie **in op Aan)** om hun eigen Azure-reserveringen te kopen.

Elke stap wordt hieronder weergegeven.

### <a name="verify-the-customer-has-an-existing-azure-subscription"></a>Controleren of de klant een bestaand Azure-abonnement heeft

Voordat u klanten toestemming geeft om hun eigen Azure-reserveringen te kopen, moet u controleren of de klant een bestaand Azure-abonnement of Azure Global-abonnement heeft. Als de klant geen huidig Azure-abonnement in Partner Center, moet u een abonnement voor hem of haar kopen voordat u de klantmachtigingen in gebruik kunt nemen.

- Als u wilt zien of een klant al een Azure-abonnement heeft, meld u zich aan bij Partner Center dashboard en selecteert u **vervolgens CSP** gevolgd door **Klanten**. Selecteer de specifieke klant in de lijst. Selecteer vervolgens **Abonnementen en** zoek naar abonnementen op basis van gebruik voor Azure Plan of Azure Global.

- Als een klant geen bestaand Azure-abonnement heeft, kunt u er een abonnement voor kopen. Zie [Het Azure-abonnement kopen.](purchase-azure-plan.md)

### <a name="verify-the-customer-has-been-assigned-the-correct-role-in-azure"></a>Controleer of aan de klant de juiste rol is toegewezen in Azure

Nadat u hebt gecontroleerd of de klant een bestaand Azure-abonnement heeft, moet u  ook controleren of aan de belangrijkste gebruikers die zijn gekoppeld aan uw klant de juiste eigenaarsrol is toegewezen voor dat Azure-abonnement. Dit is de op rollen gebaseerde toegang (RBAC) die de klant nodig heeft om Azure-reserveringen te kopen voor een Azure-abonnement dat u hebt aangeschaft.

Sommige partners hebben mogelijk al de rol Eigenaar **toegewezen aan** klanten die hun eigen Azure-resources actief willen beheren en inrichten. Als u de status Eigenaar al **hebt** toegewezen aan een klant om eerdere abonnementen te beheren die u voor deze klanten hebt aangeschaft, kunt u deze stap overslaan.  

> [!IMPORTANT]
> Als aan een klant niet  de rol Eigenaar is toegewezen, ontvangt deze een foutmelding in de Azure Portal voorkomen dat ze Azure-reserveringen kopen.

Controleren of aan de klant de rol Eigenaar **is toegewezen** voor een Azure-abonnement:

1. Meld u aan bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard)

2. Selecteer **CSP**, vervolgens **Klanten** en selecteer de specifieke klant.

3. Selecteer **Abonnementen voor** die klant en zoek het specifieke Azure-abonnement.

4. Selecteer de **knop** Beheren naast het abonnement van die klant. Hiermee opent u de [Azure Portal](https://portal.azure.com/).

5. Volg deze stappen **om een** gebruiker toe te wijzen als beheerder om de rol Eigenaar toe te wijzen aan een [specifieke gebruiker.](/azure/cost-management-billing/manage/add-change-subscription-administrator#to-assign-a-user-as-an-administrator)

### <a name="turn-on-or-turn-off-customer-permissions-to-purchase-their-own-azure-reservations"></a>Klantmachtigingen in- of uitschakelen om hun eigen Azure-reserveringen te kopen

Nadat u hebt gecontroleerd of de klant een  bestaand Azure-abonnement heeft en aan gebruikers de rol Van eigenaar voor dat abonnement is toegewezen, kunt u klantmachtigingen inschakelen (inschakelen). U kunt deze stappen ook gebruiken om klantmachtigingen uit te schakelen (uit te schakelen). U kunt klantmachtigingen in- of uitschakelen met behulp van Partner Center dashboard of [Partner Center API's.](/partner-center/develop/manage-customers)

Klantmachtigingen in- of uitschakelen in Partner Center:

1. Meld u aan bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard)

2. Selecteer in het linkernavigatiemenu **CSP** en vervolgens **Klanten**. Er wordt een klantenlijst weergegeven.

3. Selecteer een specifieke klantnaam.

4. Selecteer **Account** in het menu van de klant. De pagina **Klantaccount** wordt weergegeven.

5. Zoek het **gebied Klantmachtigingen** onderaan de pagina.

   :::image type="content" source="images/give-customers-permission-reservations.png" alt-text="Klantmachtigingen op de pagina Account." border="true":::

6. Zoek **onder Azure-reserveringen** de **optie Klant toestaan om te kopen.**

7. Als u klantmachtigingen wilt inschakelen, verplaatst u de schakelaar naast deze optie naar **de positie Aan.** Als u klantmachtigingen wilt uitschakelen, verplaatst u de schakelaar naar de **positie Uit.**

>[!NOTE]
> Zie Overzicht van klantmachtigingen in Partner Center voor meer informatie over wat er nog meer gebeurt wanneer u de machtigingen van een klant [in](give-customers-permission.md#overview-of-customer-permissions-in-partner-center)Partner Center.
>
>Wanneer u klantmachtigingen in- of uit schakelen, registreert het activiteitenlogboek elke actie. (Dit logboek is toegankelijk wanneer u het tandwielpictogram bovenaan het dashboard Partner Center selecteren). Wanneer u klantmachtigingen in- of uit  schakelen, wordt de actie weergegeven als Klantaankoopmachtigingen maken of Klantaankoopmachtigingen **verwijderen** in het activiteitenlogboek.

## <a name="help-customers-manage-reservations-they-purchase"></a>Klanten helpen bij het beheren van reserveringen die ze kopen

Zodra u klanten toestemming hebt gegeven om hun eigen Azure-reserveringen te kopen, kunt u hen helpen om de resources die ze kopen beter te beheren. Klanten kunnen veel aspecten van Azure-reserveringen zelf rechtstreeks vanuit de [Azure Portal.](https://portal.azure.com/) Ze hebben uw hulp nodig bij het beheren van enkele andere aspecten van Azure-reserveringen die ze kopen binnen uw CSP-abonnement.  

Klanten meer inzicht geven in het beheren van deze aspecten van Azure-reserveringen:

- Prijzen die klanten betalen voor Azure-reserveringen
- Hoe klanten het gebruik van Azure-reserveringen kunnen optimaliseren
- Wat gebeurt er wanneer klanten reserveringen kopen met een gedeeld bereik?
- Wat gebeurt er als klanten een reservering willen wijzigen, annuleren en vernieuwen of het bereik ervan willen wijzigen?

**Prijzen die klanten betalen voor hun reserveringen.** Uw klant koopt Azure-reserveringen aan op basis van een abonnement dat u eerder hebt gekocht in uw factureringsrekening van uw CSP-partner. De prijs van de klant voor alle Azure-reserveringen die hij op basis van dit abonnement aanschaft, wordt ook door u ingesteld. Deze prijs kan verschillen van de Web Direct-prijs die de klant in de Azure Portal.

**Hoe klanten hun gebruik van een reservering kunnen optimaliseren.** Sommige klanten kunnen profiteren van meer informatie over het optimaliseren van hun gebruik van een reservering of het toewijzen van het initiële bereik van een reservering tijdens hun aankoop. Vraag klanten voor meer informatie reserveringen [voor Azure-resources beheren.](/azure/cost-management-billing/reservations/manage-reserved-vm-instance)

**Wat gebeurt er wanneer een klant een reservering met een gedeeld bereik koopt?** Wanneer klanten een reservering kopen op basis van een eerder CSP-abonnement en een gedeeld bereik aan die reservering toewijzen, zijn eventuele kortingen die de klant heeft gegeven door de CSP van toepassing op overeenkomend gebruik voor alle abonnementen die de CSP-partner voor die klant heeft aangeschaft.

**Wat moeten klanten doen als ze een aankoop die ze hebben gedaan willen inruilen, annuleren of vernieuwen, of het initiële bereik van een reservering willen wijzigen?** Klanten moeten hun partner vragen om hen te helpen bij het wijzigen van het initiële bereik van een reservering. Ze hebben ook hulp van een partner nodig bij het inruilen, annuleren of vernieuwen van een reservering. Ze kunnen deze taken niet zelf uitvoeren met reserveringen op basis van abonnementen die voor hen zijn gekocht door een CSP-partner.

## <a name="next-steps"></a>Volgende stappen

- [Azure-reserveringen kopen namens uw klanten](azure-reservations-buying.md)

- [Partner Center- Microsoft-reserveringen verkopen](azure-reservations.md)

- [Azure-reserveringen beheren namens uw klanten](azure-reservations-manage.md)
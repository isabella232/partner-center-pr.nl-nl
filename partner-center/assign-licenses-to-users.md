---
title: Gebruikers voor klant accounts beheren
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Gebruikers beheren voor uw klanten in Partner Center: gebruikers accounts maken, gebruikers licenties toevoegen of verwijderen, wacht woorden opnieuw instellen en gebruikers accounts verwijderen of herstellen.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756087"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Gebruikers en gebruikers licenties voor klant accounts beheren 

**Juiste rollen**

- Globale beheerder
- Beheerder van gebruikers beheer
- Beheer agent


U kunt nieuwe gebruikers maken en verwijderen in het account van een klant. U kunt ook een of meer gebruikers accounts die u eerder hebt verwijderd binnen 30 dagen na de verwijdering herstellen. De vorige abonnements toewijzingen van de gebruiker worden ook teruggezet (ervan uitgaande dat hun vorige toewijzing beschikbaar is).

Wanneer u nieuwe abonnementen voor een klant koopt, moet de klant u een lijst geven met alle gebruikers die accounts moeten, hun gebruikers machtigingen en welke services elke gebruiker nodig heeft.  

>[!NOTE]
>In het gedeelte **gebruikers en licenties** van het tabblad **klant** worden alle gebruikers weer gegeven die zijn gemaakt in een Tenant van een specifieke klant, met inbegrip van gebruikers die licenties hebben gekocht van een andere CSP-partner of van een ander aankoop kanaal.

U kunt [abonnementen toewijzen aan meerdere gebruikers](bulk-license-provisioning-for-multiple-users.md) tegelijk door de namen te importeren met behulp van een [Excel-compatibel CSV-werk blad bestand](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Gebruikersaccounts maken voor een klant

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.

2. Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.

3. Selecteer **gebruikers en licenties** in het menu klant.

4. Voor elke gebruiker die u toevoegt, selecteert u **abonnement toevoegen** en vult u vervolgens de informatie in, met inbegrip van machtigingen en licenties. U moet vervolgens de wijzigingen **Opslaan**.

5. Zorg ervoor dat u de gebruikers naam en het tijdelijke wacht woord noteert om naar de gebruiker te verzenden.

6. Als u meerdere gebruikers per keer toevoegt, gebruikt u **een andere gebruiker toevoegen**.

7. U kunt ook meerdere gebruikers tegelijk toevoegen door [een Excel-compatibel CSV-werkblad bestand te importeren](adding-multiple-users-to-a-customer-account.md). U kunt wachten tot u klaar bent met de hele set voordat u de namen en wacht woorden in het bevestigings scherm e-mailt of afdrukt.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Gebruikers licenties toevoegen aan of verwijderen uit een klant

De volgende stappen zijn van toepassing op het toevoegen of verwijderen van gebruikers licenties voor micro soft-producten. Zie [licenties toevoegen of verwijderen voor een SaaS-abonnement](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)om gebruikers licenties toe te voegen aan of te verwijderen voor SaaS-abonnementen op basis van licenties in de commerciële Marketplace.

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.

2. Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.

3. Selecteer **gebruikers en licenties** in het menu klant.

4. Kies een of meer gebruikers in de lijst. Als de klant bijvoorbeeld zojuist nieuwe licenties heeft aangeschaft en u deze wilt toewijzen aan mensen die deze nog niet hebben, kunt u de optie **gebruikers filteren op...** gebruiken om de juiste groep te vinden.

5. Selecteer **licenties beheren**. Breng uw wijzigingen aan en **Sla** het bestand op.

> [!NOTE]
> Voor [Azure Marketplace-Producten](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)wordt licentie toewijzing en-activering beheerd via de onafhankelijke software leverancier (ISV) die het product heeft gepubliceerd.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Het wacht woord van een gebruiker voor een klant opnieuw instellen

1. Meld u aan bij het [dashboard](https://partner.microsoft.com/dashboard) van het Partnercentrum.

2. Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.

3. Selecteer **gebruikers en licenties** in het menu klant. Kies de gebruiker in de lijst.

4. Selecteer onder aan het scherm **wacht woord opnieuw instellen**. 

5. Het nieuwe tijdelijke wacht woord naar de gebruiker verzenden.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Gebruikers accounts voor een klant verwijderen

1. Selecteer in het menu **Partner Center** **klanten**. Kies de klant in de lijst.

2. Selecteer **gebruikers en licenties** in het menu klant. Kies de gebruiker in de lijst.

3. Selecteer onder aan het scherm de optie **gebruikers account verwijderen**.

Als u dit account wilt herstellen, kunt u het vinden op het tabblad **Verwijderde gebruikers** van de lijst **gebruikers en licenties** van de klant. U hebt 30 dagen de tijd om een verwijderde gebruiker te herstellen.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Verwijderde gebruikers accounts herstellen

1. Selecteer **klanten** in het menu van het **partner centrum** en kies vervolgens de klant in de lijst.

2. Selecteer **gebruikers en licenties**.

3. Selecteer het tabblad **Verwijderde gebruikers ()** . Het moet worden gelezen **(1)** of groter wanneer er verwijderde gebruikers zijn die kunnen worden hersteld.

4. Selecteer een of meer van de selectie vakjes van de verwijderde gebruikers en selecteer vervolgens **herstellen**.

    Alle geselecteerde gebruikers accounts worden weer gegeven op de pagina **gebruikers en licenties** .

## <a name="next-steps"></a>Volgende stappen

- [Licenties toewijzen of intrekken voor meerdere gebruikers](bulk-license-provisioning-for-multiple-users.md)

- [Meerdere gebruikers voor een klant account maken](adding-multiple-users-to-a-customer-account.md)
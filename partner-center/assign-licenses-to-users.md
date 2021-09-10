---
title: Gebruikers beheren voor klantaccounts
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: 'Gebruikers voor uw klanten beheren in Partner Center: maak gebruikersaccounts, voeg gebruikerslicenties toe of verwijder deze, stel wachtwoorden opnieuw in en verwijder of herstel gebruikersaccounts.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1c346e5e680fdd0b0b82715160b238e1e6b6a9a9
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957472"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a>Gebruikers en gebruikerslicenties voor klantaccounts beheren 

**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Beheeragent


U kunt nieuwe gebruikers maken en verwijderen in het account van een klant. U kunt ook een of meer gebruikersaccounts herstellen die u eerder binnen 30 dagen na de verwijdering hebt verwijderd. De vorige abonnementstoewijzingen van de gebruiker worden ook hersteld (ervan uitgaande dat de vorige toewijzingen beschikbaar zijn).

Wanneer u nieuwe abonnementen voor een klant koopt, moet de klant u een lijst geven met alle gebruikers die accounts nodig hebben, hun gebruikersmachtigingen en welke services elke gebruiker nodig heeft.  

>[!NOTE]
>In **de sectie** Gebruikers en licenties van het tabblad Klant ziet u alle gebruikers die zijn gemaakt in de tenant van een specifieke klant, met inbegrip van gebruikers die licenties hebben aangeschaft van een andere CSP-partner of van een ander aankoopkanaal. 

U kunt [abonnementen aan meerdere gebruikers](bulk-license-provisioning-for-multiple-users.md) tegelijk toewijzen door de namen te importeren met behulp van een Excel compatibel .csv [spreadsheetbestand](adding-multiple-users-to-a-customer-account.md).

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a>Gebruikersaccounts maken voor een klant

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Selecteer gebruikers en licenties in het menu **van de klant.**

4. Voor elke gebruiker die u toevoegt, selecteert u **Abonnement toevoegen** en vult u de gegevens in, inclusief machtigingen en licenties. U moet vervolgens de wijzigingen **Opslaan**.

5. Zorg ervoor dat u de gebruikersnaam en het tijdelijke wachtwoord vast weet te stellen die u naar de gebruiker wilt verzenden.

6. Als u meerdere gebruikers één voor één toevoegt, gebruikt **u Een andere gebruiker toevoegen.**

7. U kunt ook meerdere gebruikers tegelijk toevoegen door een Excel compatibele .csv [spreadsheetbestand te importeren.](adding-multiple-users-to-a-customer-account.md) U kunt wachten totdat u klaar bent met de hele set voordat u de namen en wachtwoorden via het bevestigingsscherm per e-mail kunt afdrukken of afdrukken.

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a>Gebruikerslicenties voor een klant toevoegen of verwijderen

De volgende stappen zijn van toepassing op het toevoegen of verwijderen van gebruikerslicenties voor Microsoft-producten. Zie Licenties voor een SaaS-abonnement toevoegen of verwijderen als u gebruikerslicenties wilt toevoegen of verwijderen voor [SaaS-abonnementen](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)op basis van licenties in de commerciële marketplace.

1. Meld u aan bij Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Selecteer gebruikers en licenties in het menu **van de klant.**

4. Kies een of meer gebruikers uit de lijst. Als de klant bijvoorbeeld zojuist nieuwe licenties heeft aangeschaft en u deze wilt toewijzen aan mensen die deze nog niet hebben, kunt u de optie Gebruikers filteren **op...** gebruiken om de juiste groep te vinden.

5. Selecteer **Licenties beheren**. Maak uw wijzigingen en klik vervolgens op **Opslaan.**

> [!NOTE]
> Voor [Azure Marketplace worden](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)licentietoewijzing en activering beheerd via de ONAFHANKELIJKE softwareleverancier (ISV) die het product heeft gepubliceerd.

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a>Het wachtwoord van een gebruiker opnieuw instellen voor een klant

1. Meld u aan bij het [dashboard](https://partner.microsoft.com/dashboard) van het Partnercentrum.

2. Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.

3. Selecteer gebruikers en licenties in het menu **van de klant.** Kies de gebruiker in de lijst.

4. Selecteer wachtwoord opnieuw instellen onderaan het **scherm.** 

5. Verzend het nieuwe tijdelijke wachtwoord naar de gebruiker.

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a>Gebruikersaccounts voor een klant verwijderen

1. Selecteer klanten **Partner Center** het menu **.** Kies de klant in de lijst.

2. Selecteer gebruikers en licenties in het menu **van de klant.** Kies de gebruiker in de lijst.

3. Selecteer onderaan het scherm Gebruikersaccount **verwijderen.**

Als u dit account wilt herstellen, kunt u het vinden op het tabblad **Verwijderde** gebruikers van de lijst Gebruikers **en licenties van de** klant. U hebt 30 dagen de tijd om een verwijderde gebruiker te herstellen.

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a>Verwijderde gebruikersaccounts herstellen

1. Selecteer in **Partner Center** menu **Klanten** en kies vervolgens de klant in de lijst.

2. Selecteer **Gebruikers en licenties.**

3. Selecteer **het tabblad Verwijderde gebruikers (** ). Deze moet **(1)** of hoger lezen wanneer er verwijderde gebruikers zijn die kunnen worden hersteld.

4. Selecteer een of meer van de selectievakjes van de verwijderde gebruikers en selecteer vervolgens **Herstellen.**

    Alle geselecteerde gebruikersaccounts worden opnieuw weergegeven op **de pagina Gebruikers en** licenties.

## <a name="next-steps"></a>Volgende stappen

- [Licenties toewijzen of intrekken voor meerdere gebruikers](bulk-license-provisioning-for-multiple-users.md)

- [Meerdere gebruikers maken voor een klantaccount](adding-multiple-users-to-a-customer-account.md)
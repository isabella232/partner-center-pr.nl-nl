---
title: Problemen met het instellen van Partner Center-account of MPN-verlenging oplossen
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Problemen oplossen bij het registreren bij Partner Center. Antwoorden bieden antwoord op uitdagingen met betalingswijzen, het vergeten van wachtwoorden en meer.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a5e8a292ad8593dc0b94179d5f0ee418344ef9af
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854686"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Problemen met accountinstallatie of MPN-verlenging oplossen

**Juiste rollen:** globale | MPN-partnerbeheerder
 
Hier zijn enkele suggesties voor het oplossen van veelvoorkomende problemen bij het instellen van uw Partner Center account.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Wat gebeurt er als u migreert van Partner Membership Center en u geen velden met bedrijfsgegevens kunt bewerken

Als uw bedrijf al aanwezig is in Partner Center (bijvoorbeeld een CSP-account), wordt er een alleen-lezenscherm weergegeven. In dit scherm wordt alle informatie over uw bedrijf weergegeven zoals deze bestaat in Partner Center.

U kunt de details op dit scherm niet wijzigen. Dit is een ontwerp en geen fout.

Selecteer **Accepteren** en **Doorgaan om door** te gaan.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Als de IT-afdeling Registreren voor eenmalige **aanmelding heeft Partner Center**

U ziet dit bericht omdat virale gebruikers zijn uitgeschakeld of omdat virale aanmelding is uitgeschakeld in de Azure AD-tenant. De globale beheerder voor uw Azure AD-account kan vereiste functies inschakelen door de volgende PowerShell-opdracht uit te voeren:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Lees Registreren voor [selfservice voor meer informatie.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>U bent uw wachtwoord vergeten

Als u uw wachtwoord bent vergeten, selecteert u de koppeling Geen toegang tot uw **account?** op de aanmeldingspagina. Met deze optie kunt u uw wachtwoord opnieuw instellen of uw globale beheerder vragen om nieuwe referenties aan u toe te wijzen.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Op het scherm Vertel ons over uw bedrijf ontvangt u de fout 'Er is iets misgegaan'

Dit foutbericht wordt meestal weergegeven als u per ongeluk speciale tekens, spaties of landcode in uw bedrijfstelefoonnummer gebruikt. De waarde die is ingevoerd in het veld Telefoonnummer mag maximaal 10 tekens bevatten.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Uw creditcardaankoop ontvangt een foutbericht met de mededeling dat uw bestelling is afgewezen. Controleer uw gegevens'


Gebruik altijd het adres dat overeenkomt met uw creditcard in plaats van uw juridische entiteit. Zorg er ook voor dat de postcode juist is en overeenkomt met het adres dat u gebruikt.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>U wilt overschakelen van offline betaling naar online betalingswijze 

U moet de oorspronkelijke bestelling annuleren en de oorspronkelijke bestelling opnieuw inkopen met behulp van de betalingswijze van voorkeur.

Een order annuleren:

1. Selecteer **het tabblad Lidmaatschapsaanbiedingen** in het dashboard.

2. Selecteer **Order annuleren**

3. Er wordt een bevestigingsvenster weergegeven en u moet bevestigen om de initiële bestelling te annuleren.

## <a name="next-steps"></a>Volgende stappen

- [Uw Partner Center-account beheren](partner-center-account-setup.md)
- [Uw factuur- en reconbestand lezen](read-your-bill.md)

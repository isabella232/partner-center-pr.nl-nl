---
title: Problemen met het instellen van Partner Center-account of MPN-verlenging oplossen
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Problemen oplossen bij het registreren bij Partner Center. Antwoorden op uitdagingen met betalingswijzen, het vergeten van wachtwoorden en meer.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b84a46f20cb81a54ddf8ae13ed7156ffcf613c06a075dd597e9586e89608bc78
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115696033"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Problemen met accountinstallatie of MPN-verlenging oplossen

**Juiste rollen:** globale | MPN-partnerbeheerder
 
Hier zijn enkele suggesties voor het oplossen van veelvoorkomende problemen bij het instellen van uw Partner Center account.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Wat gebeurt er als u migreert van Partner Membership Center en u geen velden met bedrijfsgegevens kunt bewerken

Als uw bedrijf al aanwezig is in Partner Center (bijvoorbeeld een Cloud Solution Provider(CSP)-account), wordt er een alleen-lezenscherm weergegeven. In dit scherm wordt alle informatie over uw bedrijf weergegeven zoals deze bestaat in Partner Center.

U kunt de details op dit scherm niet wijzigen. Dit is een ontwerp en geen fout.

Als u wilt doorgaan, **selecteert u** Accepteren en selecteert u **vervolgens Doorgaan.**


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Als de IT-afdeling Registreren voor eenmalige **aanmelding heeft Partner Center**

U ziet dit bericht omdat virale gebruikers zijn uitgeschakeld of omdat virale aanmelding is uitgeschakeld op de Azure Active Directory (AD)-tenant. De globale beheerder voor uw Azure AD-account kan vereiste functies inschakelen door de volgende PowerShell-opdracht uit te voeren:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Lees Registreren voor [selfservice voor meer informatie.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>U bent uw wachtwoord vergeten

Als u uw wachtwoord bent vergeten, selecteert u Op de aanmeldingspagina de optie **Geen toegang tot uw account?**. Met deze optie kunt u uw wachtwoord opnieuw instellen of uw globale beheerder vragen om u nieuwe referenties toe te wijzen.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Op het scherm Vertel ons over uw bedrijf ontvangt u de fout 'Er is iets misgegaan'

Dit foutbericht wordt meestal weergegeven als u per ongeluk speciale tekens, spaties of landcode in uw bedrijfstelefoonnummer gebruikt. De waarde die is ingevoerd in Telefoon veld Getal mag maximaal 10 tekens bevatten.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Uw creditcardaankoop ontvangt een foutbericht met de mededeling dat uw bestelling is afgewezen. Controleer uw gegevens"


Gebruik altijd het adres dat overeenkomt met uw creditcard in plaats van uw juridische entiteit. Zorg er ook voor dat de postcode juist is en overeenkomt met het adres dat u gebruikt.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>U wilt overschakelen van offline betaling naar online betalingswijze 

U moet de oorspronkelijke order annuleren en de oorspronkelijke bestelling opnieuw inkopen met behulp van de gewenste betalingswijze.

Een order annuleren:

1. Selecteer in Partner Center dashboard het tabblad **Lidmaatschapsaanbiedingen.**

2. Selecteer **Order annuleren**

3. Er wordt een bevestigingsvenster weergegeven en u moet bevestigen om de initiële bestelling te annuleren.

## <a name="next-steps"></a>Volgende stappen

- [Uw Partner Center-account beheren](partner-center-account-setup.md)
- [Uw factuur- en reconbestand lezen](read-your-bill.md)

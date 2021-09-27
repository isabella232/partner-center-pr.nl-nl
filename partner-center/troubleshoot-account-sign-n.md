---
title: Problemen met het instellen van Partner Center-account of MPN-verlenging oplossen
ms.topic: how-to
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Problemen oplossen bij het registreren bij Partner Center. Antwoorden op uitdagingen met betalingswijzen, het vergeten van wachtwoorden en meer.
author: ParthP
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1f16ce1c2d765530618f8c97ccfe7e871de3c0ab
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129072961"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Problemen met accountinstallatie of MPN-verlenging oplossen

**Juiste rollen:** Globale | MPN-partnerbeheerder

Hier zijn enkele suggesties voor het oplossen van veelvoorkomende problemen die zich voordoen bij het instellen van Partner Center account.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Wat gebeurt er als u migreert van Partner Membership Center en u geen velden met bedrijfsgegevens kunt bewerken

In gevallen waarin uw bedrijf al aanwezig is in Partner Center (bijvoorbeeld een CSP-account (Cloud Solution Provider), wordt er een alleen-lezenscherm weergegeven. In dit scherm wordt alle informatie over uw bedrijf weergegeven zoals deze bestaat in Partner Center.

U kunt de details op dit scherm niet wijzigen. Dit is een ontwerp en geen fout.

Als u wilt doorgaan, **selecteert u** Accepteren en selecteert u **vervolgens Doorgaan.**

### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Als de IT-afdeling Registreren voor eenmalige **aanmelding heeft Partner Center**

U ziet dit bericht omdat virale gebruikers zijn uitgeschakeld of omdat virale aanmelding is uitgeschakeld op de Azure Active Directory (AD)-tenant. De globale beheerder voor uw Azure AD-account kan vereiste functies inschakelen door de volgende PowerShell-opdracht uit te voeren:

**Set-MsolCompanySettings -AllowEmailVerifiedUsers $true -AllowAdHocSubscriptions $true**

Lees Registreren voor [selfservice voor meer informatie.](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>U bent uw wachtwoord vergeten

Als u uw wachtwoord bent vergeten, selecteert u Op de aanmeldingspagina de optie **Geen toegang tot uw account?**. Met deze optie kunt u uw wachtwoord opnieuw instellen of uw globale beheerder vragen om nieuwe referenties aan u toe te wijzen.

## <a name="on-the-tell-us-about-your-company-screen-you-receive-a-something-went-wrong-error"></a>Op het scherm Vertel ons over uw bedrijf ontvangt u de fout 'Er is iets misgegaan'

Dit foutbericht wordt meestal weergegeven als u per ongeluk speciale tekens, spaties of landcode in uw bedrijfstelefoonnummer gebruikt. De waarde die is ingevoerd in Telefoon veld Getal mag maximaal 10 tekens bevatten.

### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Uw creditcardaankoop ontvangt een foutbericht met de mededeling dat uw bestelling is afgewezen. Controleer uw gegevens"

Gebruik altijd het adres dat overeenkomt met uw creditcard in plaats van uw juridische entiteit. Zorg er ook voor dat de postcode juist is en overeenkomt met het adres dat u gebruikt.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>U wilt overschakelen van offline betaling naar online betalingswijze

U moet de oorspronkelijke order annuleren en de oorspronkelijke bestelling opnieuw inkopen met behulp van de gewenste betalingswijze.

Een order annuleren:

> [!NOTE]
> De Partner Center preview-interface biedt u een efficiëntere en productieve gebruikerservaring via logisch gegroepeerde werkruimten. Zie Voor meer informatie over de interface van werkruimten en hoe u deze in kunt [Partner Center.](get-around-partner-center.md#turn-workspaces-on-and-off)

#### <a name="workspaces-view"></a>[Werkruimtenweergave](#tab/workspaces-view)

1. Selecteer in [Partner Center dashboard](https://partner.microsoft.com/dashboard)de **tegel** Lidmaatschap.

2. Selecteer **Lidmaatschapsaanbiedingen** en vervolgens **Order annuleren.**

3. Er wordt een bevestigingsvenster weergegeven en u moet bevestigen om de initiële bestelling te annuleren.

#### <a name="current-view"></a>[Huidige weergave](#tab/current-view)

1. Selecteer in [Partner Center dashboard](https://partner.microsoft.com/dashboard)het tabblad **Lidmaatschapsaanbiedingen.**

2. Selecteer **Order annuleren.**

3. Er wordt een bevestigingsvenster weergegeven en u moet bevestigen om de initiële bestelling te annuleren.

* * *

## <a name="next-steps"></a>Volgende stappen

- [Uw Partner Center-account beheren](partner-center-account-setup.md)
- [Uw factuur- en reconbestand lezen](read-your-bill.md)

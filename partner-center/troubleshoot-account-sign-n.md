---
title: Problemen oplossen met het instellen van uw partner Center-account of problemen met MPN-vernieuwing
ms.topic: how-to
ms.date: 08/18/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Problemen oplossen bij het registreren in het partner centrum. Beantwoordt antwoorden op uitdagingen met betalings wijzen, wacht woorden verg eten en nog veel meer.
author: ArpithaKanuganti
ms.author: v-arkanu
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: d990a2cb4dcb69dfc76e8a4f0d40fd4912b4f8a0
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92528733"
---
# <a name="troubleshoot-account-setup-or-mpn-renewal-issues"></a>Problemen met de account installatie of MPN oplossen

**Van toepassing op**

- Partnercentrum
 
**Juiste rollen**

- Globale beheerder
- MPN-partner beheerder 
 
Hier volgen enkele suggesties voor het oplossen van veelvoorkomende problemen die zich voordoen bij het instellen van uw partner centrum-account.

## <a name="what-happens-if-you-are-migrating-from-partner-membership-center-and-you-cant-edit-any-company-information-fields"></a>Wat gebeurt er als u migreert van het lidmaatschaps centrum van de partner en u geen bedrijfs gegevens velden kunt bewerken

In gevallen waarin uw bedrijf al een aanwezigheid heeft in het partner centrum (bijvoorbeeld CSP-account), wordt er een alleen-lezen scherm weer gegeven. In dit scherm worden alle gegevens van uw bedrijf weer gegeven, zoals deze in het partner centrum aanwezig zijn.

U kunt de details op dit scherm niet wijzigen. Dit is een ontwerp en geen fout.

Selecteer **accepteren** en **door gaan** om door te gaan.


### <a name="if-the-it-department-has-turned-off-sign-up-for-partner-center"></a>Als de IT-afdeling zich heeft **aangemeld voor partner centrum** .

Dit bericht wordt weer gegeven omdat er virus gebruikers zijn uitgeschakeld of omdat een virus registratie is uitgeschakeld op de Azure AD-Tenant. De globale beheerder voor uw Azure AD-account kan de vereiste functies inschakelen door de volgende Power shell-opdracht uit te voeren:

**Set-MsolCompanySettings-AllowEmailVerifiedUsers $true-AllowAdHocSubscriptions $true**

Lees voor meer informatie [self-service registreren](/azure/active-directory/users-groups-roles/directory-self-service-signup)

## <a name="you-forgot-your-password"></a>U hebt uw wacht woord verg eten

Als u uw wacht woord bent verg eten, selecteert u de koppeling **geen toegang tot uw account?** op de aanmeldings pagina. Met deze optie kunt u uw wacht woord opnieuw instellen of uw globale beheerder vragen om u nieuwe referenties toe te wijzen.

## <a name="on-the-tell-us-about-your-company-scree-you-receive-a-something-went-wrong-error"></a>Op de Scree ' vertel ons over uw bedrijf ' wordt het fout bericht ' er is iets misgegaan ' weer gegeven

Dit fout bericht wordt meestal weer gegeven als u per ongeluk speciale tekens, spaties of land code gebruikt in het telefoon nummer van uw bedrijf. De waarde die is opgegeven in het veld telefoon nummer mag Maxi maal 10 tekens bevatten.


### <a name="your-credit-card-purchase-is-receiving-an-error-message-stating-that-your-order-was-declined-please-verify-your-information"></a>Er wordt een fout bericht weer gegeven met de melding dat uw bestelling is afgewezen. Controleer uw gegevens


Gebruik altijd het adres dat overeenkomt met uw credit card in plaats van uw juridische entiteit. Zorg er ook voor dat de post code juist is en overeenkomt met het adres dat u gebruikt.

## <a name="you-want-to-switch-from-offline-payment-to-online-payment-method"></a>U wilt overschakelen van de offline betaling naar de online betalings methode 

U moet de oorspronkelijke volg orde annuleren en kopen met de gewenste Betalings wijze.

Een order annuleren:

1. Selecteer het tabblad met **lidmaatschaps aanbiedingen** in het dash board.

2. **Order annuleren** selecteren

3. Er wordt een bevestigings venster weer gegeven en u moet bevestigen om de oorspronkelijke volg orde te annuleren.

## <a name="next-steps"></a>Volgende stappen

- [Uw Partner Center-account beheren](partner-center-account-setup.md)
- [Uw factuur-en afstemmings bestand lezen](read-your-bill.md)
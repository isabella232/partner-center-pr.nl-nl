---
title: Meervoudige verificatie instellen voor uw gebruikers
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Meer informatie over het instellen van uw werknemers met MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: ee457193a23de0601b60b2291cdee985aceaaeb8
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114846108"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Meervoudige verificatie instellen voor uw gebruikers

**Juiste rollen:** globale beheerder

Betere privacybescherming en -beveiliging zijn een van onze belangrijkste prioriteiten. We weten dat de beste verdediging preventie is en dat we alleen zo sterk zijn als onze zwakste koppeling. Daarom hebben we iedereen in ons ecosysteem nodig om actie te ondernemen en ervoor te zorgen dat de juiste beveiligingsbescherming is gewaarborgd. We raden alle partners ten zeerste aan multi-factor authentication (MFA) in te schakelen voor hun gebruikers in hun partner-tenant. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Meervoudige verificatie toevoegen voor uw gebruikers

U moet de globale beheerder voor uw bedrijf zijn om deze taak te voltooien.

Het is het gemakkelijkst om MFA in teschakelen voor uw gebruikers wanneer u ze toevoegt aan uw Azure AD-tenant.

1. Meld u aan [Azure Portal](https://portal.azure.com) en ga vervolgens naar **Gebruikersbeheer.**
1. Selecteer **Multi-Factor Authentication.**
1. Selecteer de gebruiker die u wilt inschakelen en selecteer vervolgens **Inschakelen.**

Hiermee wordt MFA ingeschakeld voor deze gebruiker. Ingeschakeld betekent dat de gebruiker wordt gevraagd om de MFA-verificatie in te stellen wanneer deze zich voor de eerste keer aanmelden. Daarna wordt ze bij het aanmelden gevraagd om een code op te geven die naar hen wordt verzonden via e-mail of sms-bericht (afhankelijk van de code die ze hebben ingesteld).  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Geef op hoe u dit wilt controleren.":::

>[!NOTE]
>U kunt **afdwingen** dat gebruikers MFA gebruiken door dezelfde stappen te volgen als hierboven en Afdwingen **te selecteren.** Lees Enable [per-user Azure Multi-Factor Authentication to secure sign-in events (Azure Multi-Factor Authentication per gebruiker](/azure/active-directory/authentication/howto-mfa-userstates)inschakelen om aanmeldingsgebeurtenissen te beveiligen) voor meer informatie. 

Alle gebruikers starten **Uitgeschakeld.** Wanneer u gebruikers per gebruiker inschrijft Azure Active Directory Multi-Factor Authentication, wordt de status gewijzigd in **Ingeschakeld.** Wanneer ingeschakelde gebruikers zich aanmelden en het registratieproces voltooien, wordt de status gewijzigd in **Afgedwongen.** 

## <a name="next-steps"></a>Volgende stappen

- [Rollen en machtigingen toewijzen aan gebruikers](permissions-overview.md)
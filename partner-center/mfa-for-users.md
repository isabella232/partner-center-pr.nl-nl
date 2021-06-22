---
title: Meervoudige verificatie instellen voor uw gebruikers
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het instellen van uw werknemers met MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9cdb83c8b58b75606275c9773cba79eba75d5d0d
ms.sourcegitcommit: 7cc83714e17337b472727819243f98c84ae181ba
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/22/2021
ms.locfileid: "112450799"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Meervoudige verificatie instellen voor uw gebruikers

**Juiste rollen:** globale beheerder

Betere privacybescherming en -beveiliging zijn een van onze belangrijkste prioriteiten. We weten dat de beste verdediging preventie is en dat we alleen zo sterk zijn als onze zwakste schakel. Daarom hebben we iedereen in ons ecosysteem nodig om te handelen en ervoor te zorgen dat de juiste beveiligingsbeschermingen zijn gewaarborgd. We raden alle partners ten zeerste aan multi-factor authentication (MFA) in te schakelen voor hun gebruikers in hun partner-tenant. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Meervoudige verificatie voor uw gebruikers toevoegen

U moet de globale beheerder voor uw bedrijf zijn om deze taak te voltooien.

Het is het gemakkelijkst om MFA in te stellen voor uw gebruikers wanneer u ze toevoegt aan uw Azure AD-tenant.

1. Meld u aan [Azure Portal](https://portal.azure.com) en ga vervolgens naar **Gebruikersbeheer.**
1. Selecteer **Multi-Factor Authentication.**
1. Selecteer de gebruiker die u wilt inschakelen en selecteer vervolgens **Inschakelen.**

Hiermee wordt MFA ingeschakeld voor deze gebruiker. Ingeschakeld betekent dat de gebruiker wordt gevraagd om de MFA-verificatie in te stellen wanneer deze zich voor de eerste keer aanmelden. Daarna wordt ze bij het aanmelden gevraagd om een code op te geven die naar hen wordt verzonden via e-mail of sms-bericht (afhankelijk van de code die ze hebben ingesteld).  

:::image type="content" source="images/multi-factor-authentication/security-verification.png" alt-text="Geef op hoe u dit wilt controleren.":::

>[!NOTE]
>U kunt **afdwingen** dat gebruikers MFA gebruiken door dezelfde stappen te volgen als hierboven en Afdwingen **te selecteren.** Lees Azure [Multi-Factor Authentication per gebruiker](/azure/active-directory/authentication/howto-mfa-userstates)inschakelen om aanmeldingsgebeurtenissen te beveiligen voor meer informatie. 

Alle gebruikers starten **Uitgeschakeld.** Wanneer u gebruikers per gebruiker inschrijft Azure Active Directory Multi-Factor Authentication, verandert hun status in **Ingeschakeld.** Wanneer ingeschakelde gebruikers zich aanmelden en het registratieproces voltooien, verandert hun status in **Afgedwongen.** 

## <a name="next-steps"></a>Volgende stappen

- [Rollen en machtigingen toewijzen aan gebruikers](permissions-overview.md)
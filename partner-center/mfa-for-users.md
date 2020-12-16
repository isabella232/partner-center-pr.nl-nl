---
title: Meervoudige verificatie instellen voor uw gebruikers
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Meer informatie over het instellen van uw werk nemers met MFA
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 355258fd20f867052fa8598e688630005262bb16
ms.sourcegitcommit: ab2ca3c5990b7f920df4ecb9c611d5b1046ec111
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/16/2020
ms.locfileid: "97579976"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a>Meervoudige verificatie instellen voor uw gebruikers

**Juiste rollen**

- Globale beheerder

Grotere veiligheids maatregelen en beveiliging zijn onder de meest voorkomende prioriteiten. We weten dat de beste verdediging voor komen en dat we alleen even sterk zijn als onze zwakste koppeling. Daarom hebben we iedereen in ons ecosysteem nodig om te reageren en te zorgen dat de juiste beveiligings beveiligingen aanwezig zijn. We raden u ten zeerste aan alle partners multi-factor Authentication (MFA) in te scha kelen voor hun gebruikers in hun partner Tenant. 

## <a name="add-multi-factor-authentication-for-your-users"></a>Multi-factor Authentication voor uw gebruikers toevoegen

U moet de globale beheerder zijn voor uw bedrijf om deze taak te volt ooien.

Het is de eenvoudigste manier om MFA in te scha kelen voor uw gebruikers wanneer u deze toevoegt aan uw Azure AD-Tenant.

1. Meld u aan bij de [Azure Portal](https://portal.azure.com) en ga vervolgens naar **gebruikers beheer**.
1. Selecteer **multi-factor Authentication**.
1. Selecteer de gebruiker die u wilt inschakelen en selecteer **inschakelen**.

Hiermee wordt MFA ingeschakeld voor deze gebruiker. Ingeschakeld betekent dat de gebruiker wordt gevraagd om de MFA-verificatie in te stellen wanneer deze zich voor de eerste keer aanmeldt. Daarna wordt bij het aanmelden gevraagd om een code op te geven die naar hen wordt verzonden via een e-mail of SMS-bericht (afhankelijk van de instelling).  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Opgeven hoe moet worden gecontroleerd":::

>[!NOTE]
>U kunt uw gebruikers **afdwingen** om MFA te gebruiken met behulp van dezelfde stappen als hierboven en vervolgens **afdwingen** te selecteren. Voor meer informatie, Lees [toestaan per gebruiker Azure multi-factor Authentication om aanmeldings gebeurtenissen te beveiligen](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userstates). 

Alle gebruikers worden **uitgeschakeld**. Wanneer u gebruikers inschrijft in azure Multi-Factor Authentication per gebruiker, verandert de status in **ingeschakeld**. Wanneer ingeschakelde gebruikers zich aanmelden en het registratie proces volt ooien, wordt de status ervan gewijzigd in **afgedwongen**. 

## <a name="next-steps"></a>Volgende stappen

- [Rollen en machtigingen toewijzen aan gebruikers](permissions-overview.md)


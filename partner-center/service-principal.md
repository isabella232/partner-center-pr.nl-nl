---
title: Service-Principal van Azure AD
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het toevoegen van een service-principal aan uw Azure AD-Tenant. Dit betekent dat u een Azure AD-toepassing (Service-Principal) toevoegt in het partner centrum.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 21ef2aaa46359570bbf13c12c5fb6c1f5eab080a
ms.sourcegitcommit: 37b0b2a7141907c8d21839de3128fb8a98575886
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/05/2020
ms.locfileid: "92528153"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Een Azure AD-toepassing (Service-Principal) toevoegen in het partner centrum

**Van toepassing op**

- Partnercentrum

**Juiste rollen**

- Globale beheerder

In het Commercial Marketplace-programma in Partner Center kunt u nu een Azure AD-toepassing (Service-Principal) toevoegen als een gebruiker in uw partner centrum-account. (U kunt dit eerder doen in uw Cloud Partner-portal, of CPP, account. Nu u hebt gemigreerd naar het partner centrum, is het CPP-account alleen-lezen.)
 
>[!Note] 
>Service-Principal is synoniem met Azure AD-toepassing.

## <a name="add-an-azure-ad-application-service-principal"></a>Een Azure AD-toepassing toevoegen (Service-Principal)

1. Selecteer in het dash board van de partner centrum **instellingen** en selecteer vervolgens **instellingen voor ontwikkel aars** .

2. Selecteer **gebruikers** en selecteer vervolgens **Azure AD-toepassingen toevoegen** .

3. Selecteer een bestaande Azure AD-toepassing of maak een nieuwe.

4. Als u een nieuwe Azure AD-toepassing maakt, neemt u de volgende informatie op:  

   - **Antwoord-URL** : de URL waar gebruikers zich kunnen aanmelden om uw Azure AD-toepassing te gebruiken.

   - **App-ID-URI** : een logische id voor de Azure AD-toepassing die wordt gepresenteerd wanneer een eenmalige aanmelding wordt verzonden naar Azure AD.

   - **Beveiligings rollen** : de rollen **beheerder** (dezelfde als de rol owner in cpp) en de **ontwikkelaar** (dezelfde als de rol Inzender in cpp) is van toepassing op het commerciële Marketplace-programma in partner centrum en ze kunnen worden gekoppeld aan deze Azure AD-toepassing.  

## <a name="next-steps"></a>Volgende stappen

- [Overzicht van de commerciële Marketplace in het partner centrum](csp-commercial-marketplace-overview.md)
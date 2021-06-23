---
title: Azure AD-service-principal
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Ontdek hoe u een service-principal toevoegt aan uw Azure AD-tenant. Dit betekent dat u een Azure AD-toepassing (service-principal) toevoegt aan Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 3698032a632384e8416664c9564819d7c4da9c38
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551551"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Een Azure AD-toepassing (service-principal) toevoegen aan Partner Center

**Juiste rollen:** globale beheerder

In het commerciële Marketplace-programma in Partner Center kunt u nu een Microsoft Azure Active Directory-toepassing (Azure AD) (service-principal) als gebruiker toevoegen aan uw Partner Center-account. (U kon dit eerder doen in uw Cloud Partner-portal (CPP)-account. Nu u bent gemigreerd naar Partner Center, is het CPP-account alleen-lezen.)
 
>[!Note] 
>Service-principal is synoniem met de Azure AD-toepassing.

## <a name="add-an-azure-ad-application-service-principal"></a>Een Azure AD-toepassing toevoegen (service-principal)

1. Selecteer in Partner Center dashboard **Instellingen** en selecteer vervolgens Instellingen voor **ontwikkelaars.**

2. Selecteer **Gebruikers** en selecteer vervolgens **Azure AD-toepassingen toevoegen.**

3. Selecteer een bestaande Azure AD-toepassing of maak een nieuwe.

4. Als u een nieuwe Azure AD-toepassing maakt, moet u de volgende informatie opnemen:  

   - **Antwoord-URL:** de URL waar gebruikers zich kunnen aanmelden om uw Azure AD-toepassing te gebruiken.

   - **App-id-URI:** een logische id voor de Azure AD-toepassing die wordt weergegeven wanneer deze een aanvraag voor een een aanmelding naar Azure AD verzendt.

   - **Beveiligingsrollen:** de rollen **Manager** (hetzelfde als de rol 'Eigenaar' in CPP) en Ontwikkelaars **(dezelfde** als de rol 'Inzender' in CPP) zijn van toepassing op het commerciële marketplace-programma in Partner Center en ze kunnen worden gekoppeld aan deze Azure AD-toepassing.  

## <a name="next-steps"></a>Volgende stappen

- [Overzicht van de commerciële marketplace in Partner Center](csp-commercial-marketplace-overview.md)
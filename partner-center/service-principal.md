---
title: Azure AD-service-principal
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-enroll
description: Ontdek hoe u een service-principal toevoegt aan uw Azure AD-tenant. Dit betekent dat u een Azure AD-toepassing (service-principal) toevoegt aan Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: a7851d270ad51a5a06ebc7d7725a2ae5c803419b
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114842827"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a>Een Azure AD-toepassing (service-principal) toevoegen aan Partner Center

**Juiste rollen:** globale beheerder

In het commerciële Marketplace-programma in Partner Center kunt u nu een Microsoft Azure Active Directory-toepassing (Azure AD) (service-principal) als gebruiker toevoegen aan uw Partner Center-account. (U hebt dit eerder kunnen doen in uw Cloud Partner-portal (CPP)-account. Nu u bent gemigreerd naar Partner Center, is het CPP-account alleen-lezen.)
 
>[!Note] 
>Service-principal is synoniem met Azure AD-toepassing.

## <a name="add-an-azure-ad-application-service-principal"></a>Een Azure AD-toepassing (service-principal) toevoegen

1. Selecteer in Partner Center dashboard de **optie Instellingen** selecteer vervolgens Instellingen **voor ontwikkelaars.**

2. Selecteer **Gebruikers** en selecteer vervolgens **Azure AD-toepassingen toevoegen.**

3. Selecteer een bestaande Azure AD-toepassing of maak een nieuwe.

4. Als u een nieuwe Azure AD-toepassing maakt, moet u de volgende informatie opnemen:  

   - **Antwoord-URL:** de URL waar gebruikers zich kunnen aanmelden om uw Azure AD-toepassing te gebruiken.

   - **App-id-URI:** een logische id voor de Azure AD-toepassing die wordt weergegeven wanneer deze een aanvraag voor een een aanmelding naar Azure AD verzendt.

   - **Beveiligingsrollen:** de rollen **Manager** (hetzelfde als de rol 'Eigenaar' in CPP) en Ontwikkelaar **(dezelfde** als de rol Inzender in CPP) zijn van toepassing op het commerciële marketplace-programma in Partner Center en ze kunnen worden gekoppeld aan deze Azure AD-toepassing.  

## <a name="next-steps"></a>Volgende stappen

- [Overzicht van de commerciële marketplace in Partner Center](csp-commercial-marketplace-overview.md)
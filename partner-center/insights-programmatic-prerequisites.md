---
title: Vereisten voor programmatisch toegang tot analysegegevens
description: Vereisten voor programmatisch toegang tot analysegegevens
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.date: 07/14/2021
ms.openlocfilehash: d4c39025aa3804435dd4d2359b93cd4a2e13ccc4
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376511"
---
# <a name="prerequisites-to-programmatically-access-analytics-data"></a>Vereisten voor programmatisch toegang tot analysegegevens

**Juiste rollen:** Globale beheerder | MPN-beheerder

Voordat u programmatisch toegang kunt krijgen tot analysegegevens van partnerinzichten, moet u voldoen aan de volgende vereisten.

## <a name="mpn-program-enrollment"></a>MPN-programma-inschrijving

Als u via een programma toegang wilt krijgen tot de analysegegevens van Partner Insights, moet u zijn ingeschreven bij het MPN-programma en een Partner Center hebben. Zie Een [MPN-account maken in Partner Center](mpn-create-a-partner-center-account.md)

## <a name="create-azure-active-directory-aad-application"></a>Een Azure Active Directory (AAD)-toepassing maken

Reguliere gebruikersreferenties kunnen niet worden gebruikt voor programmatische toegang tot Partner Insights Analytics-gegevens. Een Azure Active Directory (AAD)-toepassing moet samen met een geheim (toepassing + gebruikerstoegang) worden gemaakt om toegang te krijgen tot de API's voor programmatische toegang. Zie Quickstart: Een toepassing registreren bij de Microsoft identity platform voor meer informatie over het maken van een [AAD-toepassing en -Microsoft identity platform.](/azure/active-directory/develop/quickstart-register-app)   Machtiging is vereist voor toegang tot Microsoft Partner-API. Zie Verificatie voor meer informatie over het toevoegen van [Partner-API - Partner](/partner/develop/api-authentication#application-and-user-access)

## <a name="assign-executive-report-viewer-erv-role-to-the-user"></a>De rol Executive Report Viewer (ERV) toewijzen aan de gebruiker

Als u via een programma toegang wilt krijgen tot analytische gegevens van partnerinzichten, moet u Executive Report Viewer (ERV) hebben. Zie Toegang op basis van rollen - Partner Center Insights voor meer informatie over het toewijzen van een [ERV-rol aan Partner Center](insights-roles.md)

## <a name="generate-an-aad-token"></a>Een AAD-token genereren

U moet een AAD-token genereren met behulp van de toepassings-id (client-id), het clientgeheim, uw gebruikers-id en het wachtwoord.   [Kijk hier voor](insights-programmatic-first-api-call.md#token-generation) de stappen voor het genereren van een AAD-token.

> [!Note]
> Het token is één uur geldig.

## <a name="next-steps"></a>Volgende stappen
[Programmatisch toegangsparadigma](insights-programmatic-access-paradigm.md)
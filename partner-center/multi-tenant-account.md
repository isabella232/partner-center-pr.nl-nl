---
title: Extra tenants toevoegen aan uw partner centrum-account
ms.topic: article
ms.date: 07/30/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het toevoegen, consolideren en beheren van meerdere Azure AD-tenants in uw partner centrum-account. Lees ook over een aantal van de redenen waarom u dit zou willen doen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b9379ce6b27a8ef6e5d6894a0630745794e04e04
ms.sourcegitcommit: 3c45a181ef86b3a4866e97fb50efeae8714ab3f7
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/19/2020
ms.locfileid: "92528752"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Meerdere tenants toevoegen en beheren in uw partner centrum-account

**Van toepassing op**

- Partnercentrum

**Juiste rollen**

- Globale beheerder

Met deze functie kunt u meerdere tenants voor uw bedrijf beheren en deze consolideren in uw account van het Partnercentrum. Er zijn verschillende redenen waarom u meerdere Azure AD-tenants in uw partner centrum-account moet beheren. Bijvoorbeeld:

- Uw bedrijf kan een ander bedrijf kopen en u wilt dat de werk nemers in het nieuwe bedrijf partner Center kunnen gebruiken. U wilt echter dat de twee bedrijven gescheiden blijven. In dit geval koppelt u de Azure AD-Tenant van het nieuwe bedrijf aan uw wereld wijde partner account (PGA). Met deze koppeling kunnen gebruikers in beide bedrijven werken in het partner centrum.

- Als u meer dan één Tenant hebt voor het uitvoeren van uw bedrijf (bijvoorbeeld contoso.com, contoso.uk, contoso.in), kunt u multitenancy gebruiken om ze te koppelen aan hetzelfde PC-account.

- Voor fusies en acquisities moet u met meer dan één Tenant werken (bijvoorbeeld als contoso fabrikam aanschaft, moet u zowel Constoso.com als Fabrikam.com respectieve tenants gebruiken).

- Gebruikers van een van de tenants moeten het volgende kunnen doen:
    1.  Access Partner Center voor training, digitale down loads, MCP-koppeling
    2.  Er zijn partner Center-rollen, zoals MPN-beheer, prikkel beheer enz.


## <a name="add-another-azure-ad-tenant-to-your-account"></a>Nog een Azure AD-Tenant aan uw account toevoegen

1. Meld u als globale beheerder aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum.
1. Selecteer op het pictogram **instellingen** **account instellingen** en selecteer vervolgens **tenants** .
 
:::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="tenants koppelen"::: 

3. Selecteer **een andere AD-Tenant koppelen** en geef aan welke Tenant u wilt koppelen.

1. Meld u als globale beheerder aan bij de Tenant die u wilt koppelen en bevestig de koppeling. 

:::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="tenants koppelen"::: 

5. Nadat u hebt bevestigd, ziet u de melding **alle instellingen** .  Selecteer **terug naar Tenant beheer** en de zojuist toegevoegde Tenant wordt weer gegeven. 
 

>[!NOTE]
>U kunt een Tenant niet koppelen aan een account als het al is gekoppeld aan een ander partner centrum-account.

 
## <a name="next-steps"></a>Volgende stappen

- [Gebruikers toevoegen](create-user-accounts-and-set-permissions.md)

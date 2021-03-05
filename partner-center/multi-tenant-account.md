---
title: Tenants toevoegen aan uw partner centrum-account
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het toevoegen, consolideren of beheren van meerdere Azure AD-tenants in uw partner centrum-account en waarom u dit mogelijk wilt maken.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2f3094489f65b7164b4a55804047f9a4ab5f11cb
ms.sourcegitcommit: 79d2f00c352db61252e523f45abf93fe2a2742a5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/04/2021
ms.locfileid: "102124802"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Meerdere tenants toevoegen en beheren in uw partner centrum-account


**Juiste rollen**

- Globale beheerder
- Accountbeheerder

In dit artikel wordt beschreven hoe u meerdere Azure Active Directory-tenants (Azure AD) consolideert voor uw bedrijf en deze vervolgens kunt toevoegen en beheren in uw partner centrum-account. Er zijn veel redenen om dit te doen. Bijvoorbeeld:

- Stel dat uw bedrijf, contoso, een ander bedrijf, Fabrikam heeft aangeschaft. U wilt dat de twee bedrijven gescheiden blijven, maar u wilt dat de nieuwe werk nemers partner centrum kunnen gebruiken. In dit geval koppelt u de Azure AD-Tenant van het nieuwe bedrijf aan uw wereld wijde partner account (PGA). Met deze koppeling kunnen gebruikers in beide bedrijven werken in het partner centrum.

- Als u uw bedrijf met meer dan één Tenant uitvoert (bijvoorbeeld *contoso.com*, *contoso.uk* en *contoso.in*), kunt u multitenancy gebruiken om ze te groeperen in hetzelfde PC-account.

- Als er richt lijnen voor samen voegen en acquisities nodig zijn om te werken met tenants van beide bedrijven, gebruikt u zowel de *constoso.com* -als *fabrikam.com* -tenants.

- Gebruikers van de tenants moeten het volgende kunnen doen:
    * Access Partner Center voor training, digitale down loads of de micro soft Certified Professional (MCP)-koppeling.
    * U hebt Partner Center-rollen zoals Microsoft Partner Network (MPN) beheerder of prikkel beheerder toegewezen.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Een Azure AD-Tenant toevoegen aan uw account

1. Meld u aan als globale beheerder bij het [micro soft Partner Center](https://partner.microsoft.com/dashboard).

1. Selecteer in de rechter bovenhoek **instellingen**, selecteer **account instellingen** en selecteer vervolgens **tenants**.
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Scherm afbeelding van de knop koppelen in het deel venster Azure AD-profiel."::: 

1. Selecteer **koppelen** en geef vervolgens de Tenant op die u wilt koppelen.

1. Meld u aan bij de prompt als globale beheerder voor de Tenant die u wilt koppelen en selecteer vervolgens **bevestigen**. 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Scherm afbeelding van de knop bevestigen in het deel venster nieuwe Azure AD-koppeling bevestigen."::: 

   Nadat u de koppeling hebt bevestigd, wordt een **set** -bericht weer gegeven. Als u de zojuist toegevoegde Tenant wilt weer geven, selecteert **u terug naar Tenant beheer**. 
 
>[!NOTE]
>U kunt een Tenant niet koppelen aan een account als het al is gekoppeld aan een ander partner centrum-account.


## <a name="remove-a-tenant-from-your-account"></a>Een Tenant verwijderen uit uw account
 
1. Meld u aan als globale beheerder bij het [micro soft Partner Center](https://partner.microsoft.com/dashboard).

1. Selecteer in de rechter bovenhoek het pictogram **instellingen** en selecteer vervolgens **account instellingen**.

1. Selecteer in het linkerdeel venster **tenants**. Onder **Azure AD-tenants beheren** selecteert u het tabblad **partner** .
 
1. Selecteer **verwijderen** naast de Tenant waarvan u de koppeling wilt verwijderen.

   :::image type="content" source="images/disassociate.png" alt-text="Scherm opname van de huidige Tenant koppelingen en hun koppelingen verwijderen.":::

   Zoals u in de vorige scherm afbeelding ziet, worden de koppelingen **verwijderen** ingeschakeld voor alle gekoppelde tenants, met uitzonde ring van de primaire Tenant en de Tenant waarbij u momenteel bent aangemeld. 

   > [!NOTE]   
   > Wanneer u een Tenant verwijdert, hebben de gebruikers van die Tenant geen toegang meer tot het partner centrum-account en kan het verwijderen van invloed zijn op uw vaardig heden. 

## <a name="next-steps"></a>Volgende stappen

- [Gebruikersaccounts maken](create-user-accounts-and-set-permissions.md)







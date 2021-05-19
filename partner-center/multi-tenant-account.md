---
title: Tenants toevoegen aan uw Partner Center account
ms.topic: article
ms.date: 01/11/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het toevoegen, consolideren of beheren van meerdere Azure AD-tenants in uw Partner Center-account en ontdek waarom u dit zou willen doen.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: caea2002b5edc2958c0af316762408e309bcf14a
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110151199"
---
# <a name="add-and-manage-multiple-tenants-in-your-partner-center-account"></a>Meerdere tenants toevoegen en beheren in uw Partner Center account


**Juiste rollen:** globale | Accountbeheerder

In dit artikel wordt beschreven hoe u meerdere Azure Active Directory (Azure AD)-tenants voor uw bedrijf samenvoegt en vervolgens toevoegt en beheert in uw Partner Center account. Er zijn veel redenen om dit te doen. Bijvoorbeeld:

- Stel dat uw bedrijf, Contoso, een ander bedrijf heeft overgenomen, Fabrikam. U wilt dat de twee bedrijven gescheiden blijven, maar u wilt dat de nieuwe werknemers deze kunnen Partner Center. In dit geval koppelt u de Azure AD-tenant van het nieuwe bedrijf aan uw Partner Global Account (PGA). Met deze associatie kunnen gebruikers in beide bedrijven in een Partner Center.

- Als u uw bedrijf met meer dan één tenant hebt (bijvoorbeeld *contoso.com*, *contoso.uk* en *contoso.in*), kunt u multitenancy gebruiken om ze in hetzelfde pc-account te groepen.

- Als voor fusies en overnamesrichtlijnen is vereist dat u met tenants van beide bedrijven werkt, gebruikt u zowel de constoso.com *als* *fabrikam.com* tenants.

- Gebruikers van een van de tenants moeten het volgende kunnen doen:
    * Toegang Partner Center voor training, digitale downloads of MICROSOFT Certified Professional (MCP)-associatie.
    * Worden toegewezen Partner Center zoals Microsoft Partner Network (MPN)-beheerder of incentivesbeheerder.

## <a name="add-an-azure-ad-tenant-to-your-account"></a>Een Azure AD-tenant toevoegen aan uw account

1. Meld u als globale beheerder aan [bij Microsoft Partner Center.](https://partner.microsoft.com/dashboard)

1. Selecteer in de rechterbovenhoek **Instellingen,** selecteer **Accountinstellingen** en selecteer vervolgens **Tenants.**
 
   :::image type="content" source="images/merge-accounts/multitenantNew.png" alt-text="Schermopname van de knop Koppelen in het deelvenster Azure AD-profiel."::: 

1. Selecteer **Koppelen** en geef vervolgens de tenant aan die u wilt koppelen.

1. Meld u bij de prompt aan als globale beheerder bij de tenant die u wilt koppelen en selecteer **vervolgens Bevestigen.** 

   :::image type="content" source="images/merge-accounts/multitenantNew2.png" alt-text="Schermopname van de knop Bevestigen in het deelvenster Nieuwe Azure AD-associatie bevestigen."::: 

   Nadat u de associatie hebt bevestigd, wordt het **bericht** Alle ingesteld weergegeven. Als u de zojuist toegevoegde tenant wilt weergeven, selecteert **u Terugkeren naar tenantbeheer.** 
 
>[!NOTE]
>U kunt een tenant niet koppelen aan een account als deze al is gekoppeld aan een Partner Center account.


## <a name="remove-a-tenant-from-your-account"></a>Een tenant uit uw account verwijderen
 
1. Meld u als globale beheerder aan [bij Microsoft Partner Center.](https://partner.microsoft.com/dashboard)

1. Selecteer rechtsboven het pictogram **Instellingen** en selecteer vervolgens **Accountinstellingen.**

1. Selecteer tenants in het **linkerdeelvenster.** Selecteer **onder Azure AD-tenants beheren** het tabblad **Partner.**
 
1. Selecteer **Verwijderen naast** de tenant waarvan u de associatie wilt verwijderen.

   :::image type="content" source="images/disassociate.png" alt-text="Schermopname van de huidige tenantkoppelingen en de koppelingen verwijderen.":::

   Zoals u in de vorige  schermopname ziet, zijn de koppelingen verwijderen ingeschakeld voor alle gekoppelde tenants, met uitzondering van de primaire tenant en de tenant waarmee u momenteel bent aangemeld. 

   > [!NOTE]   
   > Wanneer u een tenant verwijdert, hebben de gebruikers in die tenant niet langer toegang tot het Partner Center-account en heeft het verwijderen mogelijk invloed op uw competenties. 

## <a name="next-steps"></a>Volgende stappen

- [Gebruikersaccounts maken](create-user-accounts-and-set-permissions.md)







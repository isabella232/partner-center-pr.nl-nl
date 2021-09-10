---
title: Tenant-id, domeinnaam, gebruikersobject-id zoeken
ms.topic: how-to
ms.date: 11/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Informatie over het vinden van id's in de Azure Portal- de Azure AD-tenant-id, domeinnaam of specifieke gebruikersobject-id van een organisatie. Sommige taken hebben deze informatie nodig.
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: db730436e88118c24aa966c1023ffeeadd20548a
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957205"
---
# <a name="locate-important-ids-for-a-user"></a>Belangrijke ID's voor een gebruiker zoeken

**Juiste rollen:** globale beheerder

In dit artikel wordt beschreven hoe u de [Azure Portal](https://portal.azure.com/) om de volgende informatie voor een gebruiker te zoeken:

- De Microsoft Azure Active Directory tenant-id (Azure AD) van de organisatie of het bedrijf van de gebruiker

- De primaire domeinnaam van de organisatie of het bedrijf dat is gekoppeld aan de Azure AD-tenant

- De object-id van de gebruiker

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>De tenant Microsoft Azure AD-id en primaire domeinnaam zoeken

Volg deze stappen om de Azure AD-tenant-id of primaire domeinnaam in de Azure Portal. (Zie Tenant-id zoeken met [PowerShell](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant#find-tenant-id-with-powershell)of CLI als u programmatisch een tenant-id wilt zoeken.

> [!NOTE]
> De tenant-id kan verschillende namen worden genoemd in verschillende toepassingen of resources. De tenant-id kan bijvoorbeeld worden aangeduid als de directory-id, de Azure Active Directory-tenant (Azure AD), Microsoft ID of voor bepaalde rapporten, zelfs de *tenantguid*.

1. Meld u aan bij de [Azure-portal](https://portal.azure.com/).

2. Selecteer **Azure Active Directory** in het menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Toont Azure Portal de optie Azure Active Directory selecteren in het menu.":::

3. Er Azure Active Directory **de pagina** Overzicht weergegeven. Als u de Azure AD-tenant-id of primaire domeinnaam wilt zoeken, gaat u naar het **veld Tenant-id** en **het veld Primair** domein. Deze velden worden weergegeven in de sectie Tenantgegevens.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Toont de pagina Overzicht met twee gemarkeerde velden, tenant-id en primaire domeinnaam.":::

4. U kunt de tenant-id op een Azure Portal andere manieren vinden. Selecteer **Azure Active Directory** in het menu. Zoek vervolgens de sectie **Beheren** in het menu en selecteer **Eigenschappen.**

   Op de pagina Eigenschappen wordt ook de tenant-id van de gebruiker weergegeven.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Toont de pagina Eigenschappen met het gemarkeerde veld Tenant-id.":::

## <a name="find-the-user-object-id"></a>De object-id van de gebruiker zoeken

Alleen het vinden van de domeinnaam en tenant-id is mogelijk niet altijd voldoende. Mogelijk moet u ook de specifieke object-id zoeken die aan een gebruiker is toegewezen. Volg deze stappen om de object-id van een gebruiker te vinden in de Azure Portal:

1. Meld u aan bij de [Azure-portal](https://portal.azure.com/).

2. Selecteer **Azure Active Directory** in het menu.

3. Zoek de **sectie** Beheren in het menu en selecteer vervolgens **Gebruikers.**

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Toont Azure Active Directory menu met gemarkeerde optie Gebruikers.":::

4. Typ op de pagina Gebruikers de naam van de gebruiker in het zoekvak.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Toont de pagina Gebruikers met een zoekvak om te zoeken naar een specifieke gebruiker.":::

5. Selecteer de naam van de gebruiker waar deze wordt weergegeven in de lijst.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Toont de pagina Gebruiker met een rij voor de gezochte gebruiker.":::

6. Zoek de sectie Identiteit op de pagina Profiel van de gebruiker. Het veld Object-id wordt hier weergegeven met de unieke object-id van de gebruiker.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Toont de pagina Gebruikersprofiel met de sectie Identiteit en één gemarkeerd veld voor Object-id.":::

## <a name="next-steps"></a>Volgende stappen

- [Uw tenant-id programmatisch zoeken met PowerShell of CLI](/azure/active-directory/fundamentals/active-directory-how-to-find-tenant)
- [Meer informatie over gebruikersprofielen in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Ontdek hoe partners klantgegevens kunnen zien of exporteren in Partner Center](see-your-customer-list.md)


---
title: Tenant-ID, domein naam, gebruikers object-ID zoeken
ms.topic: how-to
ms.date: 09/16/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: "Meer informatie over het zoeken naar Id's in de Azure Portal: de Azure AD-Tenant-ID, domein naam of specifieke gebruikers object-ID van een organisatie. Sommige taken hebben deze informatie nodig."
author: varsha-sarah
ms.author: vavargh
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.openlocfilehash: 4a3695079a9d5b0b3c66b7c2eda52a31888a6660
ms.sourcegitcommit: 3158b0de261539694e37e433c763afa4067e36fb
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/17/2020
ms.locfileid: "92528397"
---
# <a name="locate-important-ids-for-a-user"></a>Belang rijke Id's voor een gebruiker zoeken

In dit artikel wordt beschreven hoe u de [Azure Portal](https://portal.azure.com/) kunt gebruiken om de volgende informatie te vinden voor een gebruiker:

- De Tenant-ID van het Microsoft Azure Active Directory (Azure AD) van de organisatie of het bedrijf van de gebruiker

- De primaire domein naam van de organisatie of het bedrijf dat is gekoppeld aan de Azure AD-Tenant

- De gebruikers object-ID

## <a name="find-the-microsoft-azure-ad-tenant-id-and-primary-domain-name"></a>De Microsoft Azure AD Tenant-ID en primaire domein naam zoeken

Volg deze stappen om de Tenant-ID van Azure AD of de primaire domein naam binnen de Azure Portal te vinden.

> [!NOTE]
> De Tenant-ID kan verschillende namen in verschillende toepassingen of bronnen worden genoemd. De Tenant-ID kan bijvoorbeeld worden aangeduid als de Directory-ID, de Azure Active Directory (Azure AD)-Tenant, micro soft-ID of voor bepaalde rapporten, zelfs het *tenantguid* .

1. Meld u aan bij [Azure Portal](https://portal.azure.com/).

2. Selecteer **Azure Active Directory** in het menu.

   :::image type="content" source="images/id/1-find-id-azure-portal-home-screen.png" alt-text="Toont Azure Portal het selecteren van de Azure Active Directory optie in het menu.":::

3. Er wordt een Azure Active Directory **overzichts** pagina weer gegeven. Als u de Tenant-ID van Azure AD of de naam van het primaire domein wilt zoeken, zoekt u naar het veld **Tenant-id** en het veld **primair domein** . Deze velden worden weer gegeven in de sectie informatie over tenants.

   :::image type="content" source="images/id/2-find-id-azure-portal-azure-ad-overview-tenant-id-partial-screen.png" alt-text="Toont Azure Portal het selecteren van de Azure Active Directory optie in het menu.":::

4. U kunt de Tenant-ID in de Azure Portal op een paar andere manieren vinden. Selecteer **Azure Active Directory** in het menu. Zoek vervolgens de sectie **beheren** in het menu en selecteer **Eigenschappen** .

   Op de pagina eigenschappen wordt ook de bijbehorende Tenant-ID van de gebruiker weer gegeven.

   :::image type="content" source="images/id/3-find-id-azure-portal-aad-properties-tenant-id-partial.png" alt-text="Toont Azure Portal het selecteren van de Azure Active Directory optie in het menu.":::

## <a name="find-the-user-object-id"></a>De gebruikers object-ID zoeken

Het is niet altijd voldoende om de domein naam en Tenant-ID te zoeken. Mogelijk moet u ook de specifieke object-ID vinden die aan een gebruiker is toegewezen. Volg deze stappen om de object-ID van een gebruiker te zoeken in de Azure Portal:

1. Meld u aan bij [Azure Portal](https://portal.azure.com/).

2. Selecteer **Azure Active Directory** in het menu.

3. Ga naar de sectie **beheren** in het menu en selecteer vervolgens **gebruikers** .

      :::image type="content" source="images/id/4-find-id-azure-portal-aad-manage-users-option.png" alt-text="Toont Azure Portal het selecteren van de Azure Active Directory optie in het menu.":::

4. Typ op de pagina gebruikers de naam van de gebruiker in het zoekvak.

      :::image type="content" source="images/id/5-find-id-azure-portal-aad-all-users-search.png" alt-text="Toont Azure Portal het selecteren van de Azure Active Directory optie in het menu.":::

5. Selecteer de naam van de gebruiker die wordt weer gegeven in de lijst.  

      :::image type="content" source="images/id/6-find-id-azure-portal-select-user-name-partial.png" alt-text="Toont Azure Portal het selecteren van de Azure Active Directory optie in het menu.":::

6. Zoek de sectie identiteit op de profiel pagina van de gebruiker. Het veld object-ID wordt hier weer gegeven met de unieke object-ID van de gebruiker.

      :::image type="content" source="images/id/7-find-id-azure-portal-aad-user-profile-object-id.png" alt-text="Toont Azure Portal het selecteren van de Azure Active Directory optie in het menu.":::

## <a name="next-steps"></a>Volgende stappen

- [Meer informatie over gebruikers profielen in Azure Active Directory](/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)
- [Ontdek hoe partners klant gegevens kunnen zien of exporteren in het partner centrum](see-your-customer-list.md)
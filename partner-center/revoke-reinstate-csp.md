---
title: Beheerders bevoegdheden voor Azure CSP opnieuw invoeren
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe u klanten helpt om de beheerders bevoegdheden van een partner te herstellen, zodat de partner de Azure CSP-abonnementen van een klant kan beheren.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: f536d975d3c644a7afa29a95a3cb45608f6b2c9f
ms.sourcegitcommit: 89be77c9f35c77463d9558826293202afc6dec56
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/13/2021
ms.locfileid: "107315844"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Beheerders bevoegdheden voor de Azure CSP-abonnementen van een klant opnieuw invoeren  

**Toepasselijke rollen**

- Globale beheerder
- Beheer agent

Als CSP-partner verwachten uw klanten vaak dat u hun Azure-gebruik en hun systemen hiervoor gaat beheren. Hiervoor moet u beheerders bevoegdheden hebben. Sommige bevoegdheden worden verleend wanneer uw reseller-relatie met de klant tot stand is gebracht. Anderen worden aan u verleend door uw klant.

## <a name="admin-privileges-for-azure-in-csp"></a>Beheerders bevoegdheden voor Azure in CSP

Er zijn twee niveaus van beheerders bevoegdheden voor Azure in CSP.

**Beheerders bevoegdheden op Tenant niveau** (**gedelegeerde beheerders bevoegdheden**): CSP-partners krijgen deze bevoegdheden bij het tot stand brengen van de leverancier van de CSP-dealer met klanten. Gedelegeerde beheerders bevoegdheden bieden CSP-partners toegang tot de tenants van hun klanten, waardoor ze beheer functies kunnen uitvoeren zoals gebruikers toevoegen/beheren, wacht woorden opnieuw instellen en gebruikers licenties beheren.

**Beheerders bevoegdheden op abonnements niveau** : CSP-partners krijgen deze bevoegdheden tijdens het maken van Azure CSP-abonnementen voor hun klanten. Met deze bevoegdheden hebben CSP-partners volledige toegang tot deze abonnementen, waardoor ze Azure-bronnen kunnen inrichten en beheren.

## <a name="reinstate-csp-partners-admin-privileges"></a>Beheerders bevoegdheden voor de CSP-partners herstellen

Uw klant kan de toewijzing van de cryptografie functie opnieuw maken zolang u de object-ID van de AdminAgents-groep aan uw klant verstrekt. Als u gedelegeerde beheerders bevoegdheden wilt herstellen, moet u samen werken met uw klant.

1. Meld u aan bij het dash board van de partner centrum en selecteer **klanten** in het menu partner centrum.

2. Selecteer de klant waarmee u werkt en **vraag een reseller-relatie aan.** Hiermee genereert u een koppeling naar de klant die Tenant beheerders rechten heeft.

3. Die klant moet de koppeling selecteren en de wederverkoper-relatie aanvraag goed keuren.

   :::image type="content" source="images/azure/revoke4.png" alt-text="Voor beeld van een reseller-relatie voor het maken van e-mail":::

4. U moet, de partner, verbinding maken met de partner-Tenant om de object-ID van de AdminAgents-groep op te halen.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Uw klant die de rol van **eigenaar of beheerder voor gebruikers toegang** heeft en gemachtigd is om roltoewijzing op het abonnements niveau te maken, doet het volgende:


    1. Hiermee maakt u verbinding met de Tenant waar het CSP-abonnement bestaat.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Maakt verbinding met het abonnement (alleen van toepassing als de gebruiker machtigingen voor roltoewijzingen heeft via meerdere abonnementen in de Tenant).
   
         PS C:\WINDOWS\system32> Set-AzContext-SubscriptionID "CSP-abonnements-ID" '


    3. Hiermee wordt de roltoewijzing gemaakt
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Als u wilt dat de machtiging rol van eigenaar wordt verleend op resource groeps niveau of op resource niveau in plaats van het abonnements bereik, kunnen de volgende opdrachten werken:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Volgende stappen

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)

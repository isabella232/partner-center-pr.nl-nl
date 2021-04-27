---
title: Beheerdersbevoegdheden voor Azure CSP
ms.topic: how-to
ms.date: 04/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Leer hoe u klanten kunt helpen de beheerdersbevoegdheden van een partner te herstellen, zodat de partner kan helpen bij het beheren van de Azure CSP van een klant.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 26768bdf33c03145a893fa445eab6ebf92ca9b1c
ms.sourcegitcommit: efd711b0e65c55f24ce5b9636abd7b5a8cc719fe
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/27/2021
ms.locfileid: "108018184"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Beheerdersbevoegdheden voor de Azure CSP van een klant herstellen  

**Juiste rollen**

- Globale beheerder
- Beheeragent

Als CSP-partner verwachten uw klanten vaak dat u hun Azure-gebruik en hun systemen voor hen beheert. Hiervoor hebt u beheerdersbevoegdheden nodig. Sommige bevoegdheden worden verleend wanneer uw resellerrelatie met de klant tot stand is gebracht. Andere worden aan u verleend door uw klant.

## <a name="admin-privileges-for-azure-in-csp"></a>Beheerdersbevoegdheden voor Azure in CSP

Er zijn twee niveaus van beheerdersbevoegdheden voor Azure in CSP.

**Beheerdersbevoegdheden op tenantniveau** **(gedelegeerde beheerdersbevoegdheden)**- CSP-partners krijgen deze bevoegdheden tijdens het tot stand brengen van een CSP-resellerrelatie met klanten. Gedelegeerde beheerdersbevoegdheden geven CSP-partners toegang tot de tenants van hun klanten, zodat ze beheerfuncties kunnen uitvoeren, zoals gebruikers toevoegen/beheren, wachtwoorden opnieuw instellen en gebruikerslicenties beheren.

**Beheerdersbevoegdheden op abonnementsniveau:** CSP-partners krijgen deze bevoegdheden tijdens het maken Azure CSP abonnementen voor hun klanten. Deze bevoegdheden bieden CSP-partners volledige toegang tot deze abonnementen, zodat ze Azure-resources kunnen inrichten en beheren.

## <a name="reinstate-csp-partners-admin-privileges"></a>Beheerdersbevoegdheden van CSP-partners herstellen

Uw klant kan de CSP-roltoewijzing opnieuw maken zolang u de object-id van de groep AdminAgents aan uw klant op geeft. Als u weer gedelegeerde beheerdersbevoegdheden wilt krijgen, moet u samenwerken met uw klant.

1. Meld u aan Partner Center dashboard en selecteer klanten in Partner Center **menu.**

2. Selecteer de klant met wie u werkt en vraag **een resellerrelatie aan.** Met deze actie wordt een koppeling gegenereerd naar de klant met tenantbeheerdersrechten.

3. Die klant moet de koppeling selecteren en de aanvraag voor de resellerrelatie goedkeuren.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-mailvoorbeeld van een resellerrelatie maken":::

4. U, de partner, moet verbinding maken met de partnerten tenant om de object-id van de groep AdminAgents op te halen.

  
    ```powershell

    PS C:\WINDOWS\system32> Connect-AzAccount -Tenant "Partner tenant"
      Get Object ID of AdminAgents group
   
    

   S C:\WINDOWS\system32> Get-AzADGroup -DisplayName AdminAgents
    ```


5. Uw klant die de rol van eigenaar **of** beheerder van gebruikerstoegang heeft en machtigingen heeft om roltoewijzing op abonnementsniveau te maken, doet het volgende:


    1. Maakt verbinding met de tenant waar het CSP-abonnement zich bevindt.
      ```powershell
        PS C:\WINDOWS\system32> Connect-AzAccount -TenantID "Customer tenant"
      ```

    2. Maakt verbinding met het abonnement (alleen van toepassing als de gebruiker roltoewijzingsmachtigingen heeft voor meerdere abonnementen in de tenant).
   
         PS C:\WINDOWS\system32> Set-AzContext -SubscriptionID "CSP Subscription ID"'


    3. Hiermee maakt u de roltoewijzing
    
    ```powershell
      PS C:\WINDOWS\system32> New-AzRoleAssignment -ObjectID "Object ID of the Admin Agents group- needs to be provided by partner" -RoleDefinitionName "Owner" -Scope "/subscriptions/CSP subscription ID"
    ```


Als u machtigingen voor de rol eigenaar wilt verlenen op het niveau van de resourcegroep of op resourceniveau in plaats van het abonnementsbereik, kunnen de volgende opdrachten worden gebruikt:


```powershell
Grant owner role at resource group level

   New-AzRoleAssignment -ObjectID "Object ID that you got from step 3" -RoleDefinitionName Owner -Scope "/subscriptions/"SubscriptionID of CSP subscription"/resourceGroups/"Resource group name"

Grant owner role at resource level

   New-AzRoleAssignment -ObjectID <Object ID that you got from step 3> -RoleDefinitionName Owner -Scope "Resource URI"
```


## <a name="next-steps"></a>Volgende stappen

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)

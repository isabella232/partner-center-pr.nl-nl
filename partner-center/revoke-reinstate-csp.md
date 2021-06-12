---
title: Beheerdersbevoegdheden voor Azure CSP
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe u klanten kunt helpen de beheerdersbevoegdheden van een partner te herstellen, zodat de partner kan helpen bij het beheren van de Azure CSP van een klant.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 90c8f413398fcb9f65f7fef402a1cdcd092abbc4
ms.sourcegitcommit: 212471150efc8fd2c30023bc6a981a7e052e79ef
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 06/11/2021
ms.locfileid: "112025952"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Beheerdersbevoegdheden voor de Azure CSP van een klant herstellen  

**Juiste rollen:** globale | Beheeragent

Als CSP-partner verwachten uw klanten vaak dat u hun Azure-gebruik en hun systemen voor hen beheert. U moet beheerdersbevoegdheden hebben om dit te doen. Sommige bevoegdheden worden verleend wanneer uw resellerrelatie met de klant tot stand is gebracht. Andere worden aan u verleend door uw klant.

## <a name="admin-privileges-for-azure-in-csp"></a>Beheerdersbevoegdheden voor Azure in CSP

Er zijn twee niveaus van beheerdersbevoegdheden voor Azure in CSP.

- **Beheerdersbevoegdheden op tenantniveau (gedelegeerde beheerdersbevoegdheden)**: CSP-partners krijgen deze bevoegdheden tijdens het tot stand brengen van een CSP-resellerrelatie met klanten. Gedelegeerde beheerdersbevoegdheden geven CSP-partners toegang tot de tenants van hun klanten. Met deze toegang kunnen ze beheerfuncties uitvoeren, zoals gebruikers toevoegen/beheren, wachtwoorden opnieuw instellen en gebruikerslicenties beheren.
- **Beheerdersbevoegdheden op abonnementsniveau:** CSP-partners krijgen deze bevoegdheden tijdens het maken Azure CSP abonnementen voor hun klanten. Deze bevoegdheden bieden CSP-partners volledige toegang tot deze abonnementen, zodat ze Azure-resources kunnen inrichten en beheren.

## <a name="reinstate-csp-a-partners-admin-privileges"></a>De beheerdersbevoegdheden van een partner opnieuw in CSP herstellen

Uw klant kan de CSP-roltoewijzing opnieuw maken als u de van de `object ID` groep AdminAgents aan uw klant verstrekt. Als u weer gedelegeerde beheerdersbevoegdheden wilt krijgen, moet u met uw klant samenwerken door de volgende stappen uit te voeren.

1. Meld u aan bij Partner Center dashboard.

2. Selecteer in Partner Center menu **Klanten.**

3. Selecteer de klant met wie u werkt en vraag **een resellerrelatie aan.** Met deze actie wordt een koppeling gegenereerd naar de klant die tenantbeheerdersrechten heeft.

4. Uw klant moet de koppeling selecteren en de aanvraag voor de resellerrelatie goedkeuren.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-mailvoorbeeld van een resellerrelatie maken":::

5. U, de partner, moet verbinding maken met de partnerten tenant om de object-id van de groep AdminAgents op te halen.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. Uw klant moet vervolgens de volgende stappen uitvoeren met behulp van PowerShell of Azure CLI. Uw klant moet het volgende hebben:

- De rol **van** eigenaar of **beheerder van gebruikerstoegang** 
- Machtigingen voor het maken van roltoewijzingen op abonnementsniveau

   a. Alleen voor PowerShell moet de klant de `Az.Resources` module bijwerken.
   ```powershell
   Update-Module Az.Resources
   ```

   b. De klant maakt verbinding met de tenant waar het CSP-abonnement zich bevindt.
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   c. De klant maakt verbinding met het abonnement. Dit is *alleen* van toepassing als de gebruiker machtigingen voor roltoewijzing heeft voor meerdere abonnementen in de tenant.

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   d. De klant maakt vervolgens de roltoewijzing.
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

In plaats van eigenaarsmachtigingen te verlenen voor het abonnementsbereik, kunt u verlenen op het niveau van de resourcegroep of resource. 

- Op het niveau van de resourcegroep

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Op resourceniveau

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

Als de bovenstaande stappen niet werken of als er fouten optreden bij het proberen, kunt u de volgende catch-all-procedure volgen om de beheerdersrechten voor uw klant te herstellen.

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a>Problemen oplossen

Als de klant stap 6 hierboven niet kan voltooien, moet u de klant de volgende opdracht laten uitvoeren:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Geef het `newRoleAssignment.log` resulterende bestand aan Microsoft op voor verdere analyse.

Als de procedure 'catch-all' mislukt tijdens `Import-Module` de , probeert u de volgende stappen:
- Als het importeren mislukt omdat de module in gebruik is, start u de PowerShell-sessie opnieuw door alle vensters te sluiten en opnieuw te openen.
- Controleer de versie `Az.Resources` van met `Get-Module Az.Resources -ListAvailable` .
- Als versie 4.1.1 niet in de beschikbare lijst staat, moet u `Update-Module Az.Resources -Force` gebruiken.
- Als de foutmelding `Az.Accounts` geeft dat een specifieke versie moet zijn, moet u die module ook bijwerken en vervangen door `Az.Resources` `Az.Accounts` . Vervolgens moet u de PowerShell-sessie opnieuw starten.


## <a name="next-steps"></a>Volgende stappen

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)

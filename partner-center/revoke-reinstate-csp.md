---
title: Beheerdersbevoegdheden voor Azure CSP opnieuw instellen
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Meer informatie over hoe u klanten kunt helpen de beheerdersbevoegdheden van een partner te herstellen, zodat de partner kan helpen bij het beheren van de Azure Cloud Solution Provider-abonnementen (CSP) van een klant.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7ec17a386e3ac6e9b41ce0582f0c55e424ce5e64
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/24/2021
ms.locfileid: "128359428"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a>Beheerdersbevoegdheden voor de Azure CSP van een klant herstellen  

**Juiste rollen:** Globale | Beheeragent

Als een Cloud Solution Provider (CSP)-programmapartner vertrouwen uw klanten vaak op u om hun Azure-gebruik en hun systemen te beheren. U hebt beheerdersbevoegdheden nodig om ze te helpen. Als u nog geen beheerdersbevoegdheden hebt, kunt u samen met uw klant deze opnieuw in gebruik nemen.

## <a name="admin-privileges-for-azure-in-the-csp-program"></a>Beheerdersbevoegdheden voor Azure in het CSP-programma

Sommige beheerdersbevoegdheden worden automatisch verleend wanneer u een resellerrelatie met de klant tot stand stelt. Andere moeten aan u worden verleend door de klant. Er zijn twee niveaus van beheerdersbevoegdheden voor Azure in CSP.

- **Beheerdersbevoegdheden op tenantniveau (dat wil zeggen gedelegeerde beheerdersbevoegdheden)** geven u toegang tot de tenants van uw klanten. Met deze toegang kunt u beheerfuncties uitvoeren, zoals gebruikers toevoegen en beheren, wachtwoorden opnieuw instellen en gebruikerslicenties beheren. U krijgt deze bevoegdheden bij het tot stand brengen van relaties tussen CSP-resellers en klanten.
- **Beheerdersbevoegdheden op abonnementsniveau** bieden u volledige toegang tot de Azure CSP van uw klanten. Met deze toegang kunt u hun Azure-resources inrichten en beheren. U krijgt deze bevoegdheden bij het maken Azure CSP abonnementen voor uw klanten.

## <a name="how-to-reinstate-your-csp-admin-privileges"></a>Uw CSP-beheerdersbevoegdheden herstellen

U kunt samenwerken met uw klant om weer gedelegeerde beheerdersbevoegdheden te krijgen.

1. Meld u aan bij [uw Partner Center dashboard](https://partner.microsoft.com/dashboard).

2. Selecteer in Partner Center menu **Klanten.**

3. Kies de klant met wie u werkt en vraag **een resellerrelatie aan.** Met deze actie wordt een koppeling naar uw klant verzonden.

   :::image type="content" source="images/azure/revoke4.png" alt-text="E-mailvoorbeeld van een resellerrelatie maken.":::

4. Zodra uw klant de aanvraag voor de resellerrelatie heeft goedgekeurd via de opgegeven koppeling, maakt u verbinding met de partnerten tenant om de van de `object ID` groep AdminAgents op te halen.
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

5. Zorg ervoor dat uw klant het volgende heeft:

   1. De rol van **eigenaar** of **beheerder van gebruikerstoegang** 
   2. Machtigingen voor het maken van roltoewijzingen op abonnementsniveau

6. Om het proces te voltooien, moet uw klant het volgende doen met behulp van PowerShell of Azure CLI. 

   1. Als u PowerShell gebruikt, moet de klant de `Az.Resources` module bijwerken.

       ```powershell
       Update-Module Az.Resources
       ```

   2. De klant moet verbinding maken met de tenant waarin het CSP-abonnement bestaat.

      ```powershell
      Connect-AzAccount -TenantID "<Customer tenant>"
      ```

      ```azurecli
      az login --tenant <Customer tenant>
      ```

   3. De klant moet vervolgens verbinding maken met het abonnement. Dit is *alleen* van toepassing als de gebruiker machtigingen voor roltoewijzing heeft voor meerdere abonnementen in de tenant.

      ```powershell
      Set-AzContext -SubscriptionID <"CSP Subscription ID">
      ```

      ```azurecli
      az account set --subscription <CSP Subscription ID>
      ```

   4. De klant kan vervolgens de roltoewijzing maken.

      ```powershell
      New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
      ```

      ```azurecli
      az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>"
      ```

In plaats van eigenaarsmachtigingen te verlenen op abonnementsniveau, kunt u deze machtigingen verlenen op het niveau van de resourcegroep of resource: 

- Op het niveau van de resourcegroep

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- Op resourceniveau

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the AdminAgents group from step 4>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object ID of the AdminAgents group from step 4> --scope "<Resource URI>"
   ```

Als de bovenstaande stappen niet werken of als u fouten krijgt bij het proberen, probeert u de volgende catch-all-procedure om de beheerdersrechten voor uw klant te herstellen:

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```
### <a name="troubleshooting"></a>Problemen oplossen
Als de klant stap 6 niet kan voltooien, stelt u de volgende opdracht voor en geeft u het resulterende bestand op `newRoleAssignment.log` aan Microsoft voor verdere analyse:

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

Als de procedure 'catch-all' mislukt tijdens `Import-Module` de , probeert u de volgende stappen:
- Als het importeren mislukt omdat de module in gebruik is, start u de PowerShell-sessie opnieuw door alle vensters te sluiten en opnieuw te openen.
- Controleer de versie van `Az.Resources` met `Get-Module Az.Resources -ListAvailable` .
- Als versie 4.1.1 niet in de beschikbare lijst staat, moet u `Update-Module Az.Resources -Force` gebruiken.
- Als de foutmelding `Az.Accounts` geeft dat een specifieke versie moet zijn, moet u die module ook bijwerken en vervangen door `Az.Resources` `Az.Accounts` . Vervolgens moet u de PowerShell-sessie opnieuw starten.


## <a name="next-steps"></a>Volgende stappen

- [Abonnementen en resources beheren onder het Azure-abonnement](azure-plan-manage.md)

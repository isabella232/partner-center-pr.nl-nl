---
title: Het formaat van Azure-VM's wijzigen voor een maximaal reserveringsgebruik
description: Meer informatie over hoe u de grootte van een virtuele machine (VM) kunt aanpassen aan de computer vereisten van uw klanten wanneer u Microsoft Azure reserve ringen voor hen aanschaft.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: 226ebd27b4ca4cdef56ce833a58a10bed89f8056
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534944"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Het formaat van Microsoft Azure-VM’s wijzigen voor een maximaal reserveringsgebruik

**Juiste rollen**

- Beheer agent
- Verkoop agent

In dit artikel wordt uitgelegd hoe u de grootte van een virtuele machine (VM) kunt aanpassen aan de computer vereisten van uw klanten wanneer u Microsoft Azure reserve ringen voor hen aanschaft.
 
> [!NOTE]
> Dit artikel is alleen van toepassing op partners in het Cloud Solution Provider-programma (CSP). Klanten die andere soorten abonnementen gebruiken (zoals betalen per gebruik, individuele, micro soft-klant overeenkomst of Enterprise Agreement-abonnementen), moeten in plaats daarvan [deze Azure rehanden documentatie](/azure/cost-management-billing/reservations)lezen.

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>De VM-grootte voor de Azure-reserve ring van een klant bepalen

Wanneer u Microsoft Azure reserve ringen namens uw klanten koopt, moet u een grootte van een virtuele machine (VM) kiezen om te voldoen aan de computer behoeften van de klant. U kunt deze informatie vinden met een van de volgende methoden:

- Azure-gebruiks-API
- De Azure-portal
- Azure PowerShell
- De Azure Resource Manager-API (ARM)

Hieronder vindt u instructies voor het gebruik van deze methoden. Nadat u een reserve ring hebt gekocht, wordt de reserverings korting automatisch toegepast op virtuele machines die overeenkomen met de kenmerken en hoeveelheid van de reserve ring. U hoeft de reserve ring niet aan een virtuele machine toe te wijzen.

>[!NOTE]
>Reserverings kortingen zijn niet van toepassing op klassieke of promotie-Vm's.

>[!IMPORTANT]
>Als u het type en de grootte van de virtuele machine die u wilt kopen namens uw klant correct wilt identificeren, moet u een van de volgende methoden gebruiken omdat het type VM-reeks niet correct wordt weer gegeven in de reconciliatie bestanden van partner Center.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>Informatie over VM-grootte ophalen met behulp van de Azure-gebruiks-API

1. Gebruik het kenmerk waarde voor service type vanuit additionalInfo in de API-reactie om de te kopen VM-grootte te identificeren.

2. Zie voor meer informatie [klant gebruiks records voor Azure ophalen](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in de [partner centrum-API](/partner-center/develop/).

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>Informatie over VM-grootte ophalen met behulp van de Microsoft Azure-portal

1. Ga in Partner Center naar uw **klanten** pagina.

2. Zoek de klant die Azure-VM-reserve ringen wil kopen en selecteer vervolgens de pijl-omlaag om de gegevens van de klant uit te breiden. Selecteer **Microsoft Azure Management Portal** om de record van de klant te openen in de Azure Portal.

3. Selecteer **virtuele machines** in het menu van de portal en selecteer vervolgens de virtuele machine waarvoor u een reserve ring wilt kopen.

4. Zoek op de detail pagina van de virtuele machine naar de informatie over de grootte en regio, zoals hieronder wordt weer gegeven, en gebruik deze informatie om de reserve ring te kopen in het partner centrum.  

   :::image type="content" source="images/usage1.png" alt-text="Informatie over grootte en regio op de detail pagina":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>Informatie over VM-grootte ophalen met behulp van Microsoft Azure PowerShell

Gebruik de informatie in de onderstaande afbeelding om de locatie en grootte van de virtuele machine op te halen waarvoor u een reserve ring wilt kopen. 

:::image type="content" source="images/usage2.png" alt-text="Locatie en grootte van virtuele machine":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>Informatie over VM-grootte ophalen met behulp van de API voor Azure Resource Manager (ARM)

1. Roep de ARM-client voor de virtuele machine waarvoor u een reserve ring wilt kopen met behulp van de ARMClient-of ARM-Api's.

2. /Subscriptions/ <Subscription ID> /ResourceGroups/ <Resource group name> /providers/Microsoft.Compute/virtualMachines/ <VM Instance Name> ? API-Version = 2017-12-01

3. De aanroep retourneert de waarden voor **vmSize** en **locatie**, zoals hieronder wordt weer gegeven.

    :::image type="content" source="images/usage3.png" alt-text="waarde vmSize":::
    :::image type="content" source="images/usage4.png" alt-text="locatie waarde":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Azure VM-gebruik en-reserverings korting controleren

Nadat u een voor Azure gereserveerde VM-instantie hebt aangeschaft namens een klant, wordt de korting voor het vooraf betalen van VM-ruimte automatisch toegepast op de virtuele machines die overeenkomen met de kenmerken en hoeveelheid van de reserve ring van de klant.

U kunt het reserverings gebruik van de klant controleren en zien op welke virtuele machines de reserverings kortingen worden toegepast met behulp van een van de volgende methoden:

- De Azure-portal
- Azure-gebruiks-API

Hieronder vindt u instructies voor het gebruik van deze methoden.

>[!NOTE]
>Alleen de Azure-gebruiks-API laat zien op welke virtuele machine de korting wordt toegepast.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Controleer het reserverings gebruik van de klant in de Microsoft Azure-portal

1. Ga in Partner Center naar uw **klanten** pagina.

2. Zoek de klant waarvan u de reserverings korting en het gebruik wilt controleren en selecteer vervolgens de pijl-omlaag om de gegevens van de klant uit te breiden. Selecteer **Microsoft Azure Management Portal** om de record van de klant te openen in de Azure Portal.
3. Selecteer **reserve ringen** in het menu van de portal en selecteer vervolgens de reserve ring waarvoor u het gebruik wilt controleren.
4. Controleer op de pagina **overzicht** de gebruiks grafiek van de reserve ring, waarin wordt weer gegeven hoeveel van de reserve ring is toegepast op virtuele machines.

    >[!NOTE]
    >Gebruiks gegevens kunnen Maxi maal acht uur worden vertraagd.

    a. Als het gebruik van de reserve ring 100% is, krijgt uw klant alle mogelijke besparingen die de aankoop van de reserve ring kan bieden.
    b. Als het gebruik van de reserve ring 0% is, wordt de korting niet toegepast op een virtuele machine.
    c. Als het gebruik van de reserve ring tussen 1% en 99% ligt, zijn er ongebruikte voor delen.

5. Om deze situatie te voor komen, bepaalt u de juiste VM-grootte voor de ondersteuning van de computer behoeften van de klant voordat u de aanschaft.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Het reserverings gebruik van de klant controleren met de Azure-gebruiks-API

>[!NOTE]
>Alleen de Azure-gebruiks-API laat zien op welke virtuele machine de korting wordt toegepast.  

U kunt gegevens over reserverings gebruik ophalen met de API voor Azure-gebruik om te controleren of de klant de reserverings korting krijgt en te zien op welke Vm's (virtuele machines) de korting wordt toegepast. Vergelijk voor beeld A met voor beeld B om te zien hoe u het reserverings gebruik van een klant kunt controleren.

:::image type="content" source="images/usage5.png" alt-text="Voor beelden van reserverings gebruik":::

- De reservationId identificeert de Azure-reserve ring die is gebruikt voor het Toep assen van de korting op de virtuele machine.
- consumptionMeter is de MeterId voor de virtuele machine waarop de reserverings korting van toepassing is.
- De ReservationMeter toont $0 kosten sinds de reserverings korting werd toegepast.

Zie voor meer informatie [klant gebruiks records voor Azure ophalen](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) in de [partner centrum-API](/partner-center/develop/).

>[!IMPORTANT]
>Software kosten, zoals micro soft Windows Server, zijn momenteel niet opgenomen in de prijs van een VM-reserve ring en worden weer gegeven als afzonderlijke regel items in de order record en op uw factuur. Als een klant echter de Azure Hybrid Use Benefit heeft, worden de software kosten niet toegepast. Zie [Windows-software kosten die niet zijn opgenomen in gereserveerde instanties](/azure/billing/billing-reserved-instance-windows-software-costs)voor meer informatie.  

## <a name="next-steps"></a>Volgende stappen

|**Voor informatie over**   |**Leest u**    |
|:-----------------------------|:-----------------|
|Overzicht van Azure-reserve ringen in CSP  | [Microsoft Azure gereserveerde VM-instanties verkopen](azure-reservations.md)
|Azure-reserve ringen voor uw klanten kopen in het partner centrum   | [Azure-reserve ringen kopen](azure-reservations-buying.md)
|Azure-reserve ringen beheren in Partner Center | [Azure-reserve ringen beheren in Partner Center](azure-reservations-manage.md)
|Azure-reserve ringen kopen in de Azure Portal | [Vooruitbetalen voor virtuele machines met Azure reserved VM instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in de Help van Azure |
|Azure-reserve ringen beheren in de Azure Portal   | [Gereserveerde VM-instanties beheren](/azure/billing/billing-manage-reserved-vm-instance) in de Help van Azure  |
|Azure-reserve ringen aanschaffen met de Partner Center-API | [Azure reserved VM instances kopen](/partner-center/develop/purchase-azure-reservations) in de ontwikkelaars documentatie van partner Center   |
|Klanten toestemming geven om hun eigen Azure-reserve ringen te kopen vanuit een abonnement dat u hebt aangeschaft. | [Geef klanten toestemming om hun eigen Azure-reserve ringen te kopen](give-customers-permission.md)   |
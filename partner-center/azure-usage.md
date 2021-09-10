---
title: Het formaat van Azure-VM's wijzigen voor een maximaal reserveringsgebruik
description: Leer hoe u de grootte van een virtuele machine (VM) aan de computerbehoeften van uw klanten kunt aanmeten wanneer u Microsoft Azure voor hen koopt.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOJULY.20
ms.date: 08/06/2020
ms.openlocfilehash: dc9b9100e01191c24c03c76e9a9ff5a6ffe335d1
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123956872"
---
# <a name="microsoft-azure-vm-sizing-for-maximum-reservation-usage"></a>Het formaat van Microsoft Azure-VM’s wijzigen voor een maximaal reserveringsgebruik

**Juiste rollen:** beheeragent | Verkoopagent

In dit artikel wordt uitgelegd hoe u de grootte van een virtuele machine (VM) kunt inbouwen in de rekenbehoeften van uw klanten wanneer u Microsoft Azure voor hen koopt.
 
> [!NOTE]
> Dit artikel is alleen van toepassing op partners in Cloud Solution Provider (CSP)-programma. Klanten die andere typen abonnementen gebruiken (zoals betalen per gebruik, individueel, Microsoft-klantovereenkomst of Enterprise Agreement-abonnementen), moeten in plaats daarvan deze documentatie voor [Azure-reserveringen lezen.](/azure/cost-management-billing/reservations)

## <a name="determine-the-vm-size-for-a-customers-azure-reservation"></a>De VM-grootte voor de Azure-reservering van een klant bepalen

Wanneer u Microsoft Azure namens uw klanten reserveringen koopt, moet u een virtuele machine (VM) kiezen die is geformatteerd om te voldoen aan de computerbehoeften van de klant. U vindt deze informatie op een van de volgende manieren:

- Api voor Azure-gebruik
- Azure Portal
- Azure PowerShell
- De Azure Resource Manager API (ARM)

Instructies voor het gebruik van elk van deze methoden vindt u hieronder. Nadat u een reservering hebt gekocht, wordt de reserveringskorting automatisch toegepast op virtuele machines die overeenkomen met de kenmerken en hoeveelheid van de reservering. U hoeft de reservering niet toe te wijzen aan een VM.

>[!NOTE]
>Reserveringskortingen zijn niet van toepassing op klassieke of aanbiedings-VM's.

>[!IMPORTANT]
>Als u het type en de grootte van de VM die u namens uw klant wilt kopen correct wilt identificeren, moet u een van de onderstaande methoden gebruiken, omdat het type VM-serie niet correct wordt weergegeven in Partner Center-afstemmingsbestanden.

### <a name="get-vm-sizing-information-using-the-azure-utilization-api"></a>VM-formaatgegevens op halen met behulp van de Azure-gebruiks-API

1. Gebruik de waarde voor het kenmerk ServiceType uit additionalInfo in het API-antwoord om de te kopen VM-grootte te identificeren.

2. Zie Get [a customer's utilization records for Azure (Gebruiksrecords](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) van een klant voor Azure verkrijgen) in [Partner Center API voor meer informatie.](/partner-center/develop/)

### <a name="get-vm-sizing-information-using-the-microsoft-azure-portal"></a>VM-formaatgegevens verkrijgen met behulp van de Microsoft Azure portal

1. Ga Partner Center naar de **pagina** Klanten.

2. Zoek de klant die Azure VM-reserveringen wil kopen en selecteer vervolgens de pijl-omlaag om de gegevens van de klant uit te vouwen. Selecteer **Microsoft Azure Beheerportal** om de record van de klant in de Azure Portal.

3. Selecteer **Virtuele machines** in het portalmenu en selecteer vervolgens de VM waarvoor u een reservering wilt kopen.

4. Zoek op de detailpagina van de VM de grootte en regiogegevens, zoals hieronder wordt weergegeven, en gebruik deze informatie om de reservering aan te schaffen in Partner Center.  

   :::image type="content" source="images/usage1.png" alt-text="Grootte en regio-informatie op de detailpagina.":::

### <a name="get-vm-sizing-information-using-microsoft-azure-powershell"></a>VM-formaatgegevens op halen met behulp van Microsoft Azure PowerShell

Gebruik de informatie in de onderstaande afbeelding om de locatie en grootte op te vragen van de VM waarvoor u een reservering wilt kopen. 

:::image type="content" source="images/usage2.png" alt-text="VM-locatie en -grootte.":::

### <a name="get-vm-sizing-information-using-the-azure-resource-manager-arm-api"></a>VM-formaatgegevens op halen met behulp van Azure Resource Manager API (ARM)

1. Gebruik de ARMClient of de ARM-API's om de ARM-client aan te roepen voor de VM waarvoor u een reservering wilt kopen.

2. `/subscriptions/<Subscription ID>/resourceGroups/<Resource group name>/providers/Microsoft.Compute/virtualMachines/<VM Instance Name>?api-version=2017-12-01`

3. De aanroep retourneert de waarden voor **vmSize** en **locatie**, zoals hieronder wordt geïllustreerd.

    :::image type="content" source="images/usage3.png" alt-text="vmSize-waarde.":::
    :::image type="content" source="images/usage4.png" alt-text="locatiewaarde.":::

## <a name="verify-azure-vm-usage-and-reservation-discount"></a>Gebruik en reserveringskorting voor Azure-VM's controleren

Nadat u namens een klant een gereserveerde VM-instantie voor Azure hebt aangeschaft, wordt de korting voor het vooraf betalen voor VM-ruimte automatisch toegepast op de virtuele machines die overeenkomen met de kenmerken en hoeveelheid van de reservering van de klant.

U kunt het reserveringsgebruik van de klant controleren en op een van de volgende manieren zien op welke virtuele machines de reserveringskortingen worden toegepast:

- Azure Portal
- Api voor Azure-gebruik

Instructies voor het gebruik van elk van deze methoden vindt u hieronder.

>[!NOTE]
>Alleen de API voor Azure-gebruik laat zien op welke virtuele machine de korting wordt toegepast.  

### <a name="verify-the-customers-reservation-usage-in-the-microsoft-azure-portal"></a>Controleer het reserveringsgebruik van de klant in de Microsoft Azure portal

1. Ga Partner Center naar de **pagina** Klanten.

2. Zoek de klant van wie u de reserveringskorting en het gebruik wilt controleren en selecteer vervolgens de pijl-omlaag om de gegevens van de klant uit te vouwen. Selecteer **Microsoft Azure Beheerportal** om de record van de klant in de Azure Portal.
3. Selecteer **Reserveringen in het** portalmenu en selecteer vervolgens de reservering waar u het gebruik voor wilt controleren.
4. Controleer op **de pagina** Overzicht de grafiek met het gebruik van de reservering, waarin wordt weergegeven hoeveel van de reservering is toegepast op virtuele machines.

    >[!NOTE]
    >Gebruiksgegevens kunnen maximaal acht uur worden vertraagd.

    a. Als het gebruik van de reservering 100% is, krijgt uw klant alle mogelijke besparingen die de reserveringsaankoop kan bieden.
    b. Als het gebruik van de reservering 0% is, wordt de korting niet toegepast op een virtuele machine.
    c. Als het gebruik van de reservering tussen 1% en 99% ligt, zijn er ongebruikte voordelen.

5. Om deze situatie te voorkomen, moet u de juiste grootte van de VM bepalen om de computerbehoeften van de klant te ondersteunen voordat u de aankoop doet.

### <a name="verify-the-customers-reservation-usage-with-the-azure-utilization-api"></a>Het reserveringsgebruik van de klant controleren met de AZURE-gebruiks-API

>[!NOTE]
>Alleen de API voor Azure-gebruik laat zien op welke virtuele machine de korting wordt toegepast.  

U kunt reserveringsgebruiksgegevens verkrijgen met de Azure-gebruiks-API om te controleren of de klant de reserveringskorting krijgt en om te zien op welke VM's (virtuele machines) de korting wordt toegepast. Vergelijk voorbeeld A met voorbeeld B om te zien hoe u het reserveringsgebruik van een klant kunt controleren.

:::image type="content" source="images/usage5.png" alt-text="Voorbeelden van reserveringsgebruik.":::

- De reservationId identificeert de Azure-reservering die is gebruikt om de korting op de VM toe te passen.
- consumptionMeter is de MeterId voor de VM waar de reserveringskorting op is toegepast.
- De ReservationMeter toont $ 0 kosten sinds de reserveringskorting is toegepast.

Zie Get [a customer's utilization records for Azure (Gebruiksrecords](/partner-center/develop/get-a-customer-s-utilization-record-for-azure) van een klant voor Azure verkrijgen) in [Partner Center API voor meer informatie.](/partner-center/develop/)

>[!IMPORTANT]
>Softwarekosten, zoals Microsoft Windows Server, zijn momenteel niet opgenomen in de prijs van een VM-reservering en worden weergegeven als afzonderlijke regelitems in de orderrecord en op uw factuur. Als een klant echter azure Hybrid Use Benefit heeft, worden de softwarekosten niet toegepast. Zie voor meer informatie Windows [softwarekosten die niet zijn opgenomen in gereserveerde instanties.](/azure/billing/billing-reserved-instance-windows-software-costs)  

## <a name="next-steps"></a>Volgende stappen

|**Voor informatie over**   |**Leest u**    |
|:-----------------------------|:-----------------|
|Overzicht van Azure-reserveringen in CSP  | [Verkopen Microsoft Azure gereserveerde VM-instanties](azure-reservations.md)
|Azure-reserveringen kopen voor uw klanten in Partner Center   | [Azure-reserveringen kopen](azure-reservations-buying.md)
|Azure-reserveringen beheren in Partner Center | [Azure-reserveringen beheren in Partner Center](azure-reservations-manage.md)
|Azure-reserveringen kopen in de Azure Portal | [Vooruitbetalen voor virtuele machines met Azure Reserved VM Instances](/azure/virtual-machines/windows/prepay-reserved-vm-instances) in de Help van Azure |
|Azure-reserveringen beheren in de Azure Portal   | [Gereserveerde VM-instanties beheren](/azure/billing/billing-manage-reserved-vm-instance) in de Help van Azure  |
|Azure-reserveringen kopen met behulp van Partner Center API | [Aankoop Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in de documentatie Partner Center ontwikkelaars   |
|Klanten toestemming geven om hun eigen Azure-reserveringen te kopen bij een abonnement dat u voor hen hebt aangeschaft. | [Klanten toestemming geven om hun eigen Azure-reserveringen te kopen](give-customers-permission.md)   |
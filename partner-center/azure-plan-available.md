---
title: Beschikbare Azure-services in Azure CSP
description: In dit artikel worden de Azure-services besproken die wel en niet beschikbaar zijn in het programma Azure Cloud Solution Provider (CSP).
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: amitravat
ms.author: amrava
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: 6037044a72bd9bd71131ddbc66fec0555bbd5f86
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244757"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Azure-services die beschikbaar zijn in het Azure Cloud Solution Provider (CSP)-programma

**Juiste rollen:** beheeragent | Factureringsbeheerders | Globale | Helpdeskagent | Verkoopagent | Beheerder van gebruikersbeheer

## <a name="available-azure-services-in-azure-csp"></a>Beschikbare Azure-services in Azure CSP

In dit artikel vindt u een overzicht van de Azure-services die wel en niet beschikbaar zijn in het Programma Azure Cloud Solution Provider (CSP). Ook wordt de beschikbaarheid van de service in de nationale clouds [Microsoft Azure Duitsland](https://azure.microsoft.com/overview/clouds/germany/) en Microsoft Azure [Government besproken.](https://azure.microsoft.com/overview/clouds/government/)

>[!Note]
> [Azure China](https://www.azure.cn/) is niet beschikbaar in het Azure CSP programma.

## <a name="global-cloud"></a>Wereldwijde cloud

Alle services op basis van Azure Resource Manager model zijn beschikbaar in het CSP-programma.  Niet-Azure Resource Manager services zoals klassieke implementatiemodelservices zijn niet beschikbaar in het CSP-programma.  

## <a name="csp-specific-service-configurations"></a>CSP-Specific serviceconfiguraties

Voor de volgende services zijn speciale configuraties in CSP vereist:

- [StorSimple](/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/) Alleen gebruikers van de tenant van de klant hebben toegang tot gegevens in hun Time Series Insights omgeving. Partners kunnen de Time Series-Insights-omgeving van hun klant standaard beheren, maar als ze toegang nodig hebben tot de gegevens in de omgeving, moeten ze worden toegevoegd aan de tenant van de klant.

- Beheercertificaten voor het authenticeren van Azure SDK-bibliotheken via een certificaat worden niet ondersteund in het CSP-model.  Gebruik in plaats daarvan azure AD-service-principalverificatie en de Azure.Identity-bibliotheek.  Referentie [verifiëren met de Azure SDK voor .NET](/dotnet/azure/sdk/authentication)

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

U kunt de onderstaande items nu kopen via Visual Studio Marketplace, met uitzondering van extensies van derden.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Visual Studio abonnementen](https://www.visualstudio.com/subscriptions/)

- [Xamarin University training](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Om u op weg te helpen, hebben we video's en documentatie gemaakt over het instellen, kopen en beheren van [Azure DevOps](/vsts/billing/csp/set-up-csp-customer) in CSP.

## <a name="azure-marketplace-items-in-azure-csp"></a>Azure Marketplace-items in Azure CSP

Niet alle Azure Marketplace zijn momenteel beschikbaar in Azure CSP abonnementen.

- Op Microsoft gebaseerde Azure-services: deze services zijn beschikbaar. Bekijk de vorige tabel en opmerkingen.

- BYOL-items (Bring Your Own License) : Deze items zijn beschikbaar. Een volledige lijst met BYOL-Azure Marketplace-items is beschikbaar op de [pagina Azure Marketplace BYOL.](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol)

- Items van derden met betalen per Azure Marketplace: deze items zijn beschikbaar als de provider naar het CSP-kanaal heeft gepubliceerd. Zie Abonnementen verkopen voor Azure Marketplace [producten voor meer informatie.](csp-commercial-marketplace-overview.md)

- Citrix XenApp Essentials: Partners kunnen XenApp Essentials aanschaffen voor klanten in CSP. Zie voor meer informatie de volgende Citrix-blog: [Distributie van XenApp Essentials nu beschikbaar via Microsoft Cloud Solution Provider Kanaal](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/).

## <a name="national-clouds"></a>Nationale clouds

In de volgende tabel ziet u een regelmatig bijgewerkte lijst met de beschikbare eigen Azure-producten, -services en -functies voor CSP in nationale clouds.

| Azure-product, -service of -functie | Amerikaanse overheid | Duitsland |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  Virtual Machines  |  X  |  X  |
|  Cloud Services  |    |    |
|  Virtuele-machineschaalsets  |  X  |  X  |
|  Functions  |    |    |
|  Azure Container Service  |    |    |
|  **Netwerken**  |    |    |
|  Azure DNS  |    |    |
|  Content Delivery Network  |    |    |
|  Traffic Manager  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Virtual Network  |  X  |  X  |
|  Load Balancer  |  X  |  X  |
|  VPN Gateway  |  X  |  X  |
|  Application Gateway  |  X  |  X  |
|  Network Watcher  |  X  |  X  |
|  **Storage**  |    |    |
|  Storage  |  X  |  X  |
|  Backup  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Siteherstel  |  X  |  X  |
|  Data Lake Store  |    |    |
|  Managed Disks  |  X  |  X  |
|  **Web en mobiel**  |    |    |
|  App Service  |  X  |  X  |
|  App Service op Linux  |    |  X  |
|  API Management  |  X  |    |
|  Content Delivery Network  |    |    |
|  Media Services  |  X  |  X  |
|  Notification Hubs  |  X  |  X  |
|  Azure Search  |    |    |
|  Logic Apps functie van Azure App Service  |    |    |
|  **Containers**  |    |    |
|  App Service  |  X  |  X  |
|  App Service op Linux  |    |  X  |
|  Batch  |  X  |  X  |
|  Container Registry  |    |    |
|  Container Instances  |    |    |
|  Service Fabric  |  X  |  X  |
|  Container Service  |    |    |
|  **Databases**  |    |    |
|  SQL Database  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Redis Cache  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Azure Database for MySQL  |    |    |
|  Azure Database for PostgreSQL  |    |    |
|  **Gegevens en analyse**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Data Catalog  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **AI en Cognitive Services**  |    |    |
|  Machine Learning  |    |  X  |
|  Azure Bot Service  |    |    |
|  Cognitive Services  |    |    |
|  Azure Batch AI  |    |    |
|  **Internet of Things**  |    |    |
|  IoT Hub  |  X  |  X  |
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Event Hubs  |  X  |  X  |
|  Location-Based Services  |    |    |
|  Notification Hubs  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Bedrijfsintegratie**  |    |    |
|  StorSimple  |  X  |    |
|  API Management  |    |    |
|  Event Grid  |    |    |
|  Data Factory  |    |    |
|  Service Bus  |  X  |  X  |
|  Data Catalog  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Logic Apps functie van Azure App Service  |    |    |
|  **Beveiliging en identiteit**  |    |    |
|  Azure Active Directory  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Multi-Factor Authentication  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Beveiligingscentrum  |  X  |  X  |
|  **Hulpprogramma's voor ontwikkelaars**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **Controle en beheer**  |    |    |
|  Advisor  |    |    |
|  Backup  |  X  |  X  |
|  Siteherstel  |  X  |  X  |
|  Scheduler  |  X  |  X  |
|  Automation  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Azure-Managed toepassingen  |    |    |
|  Azure Migrate  |    |    |
|  Beheergroepen  |    |  

## <a name="next-steps"></a>Volgende stappen

- [Meer](/azure/cloud-solution-provider/overview/partner-center-overview) informatie over de beschikbare mogelijkheden voor Azure in Partner Center.

- [Maak](/azure/cloud-solution-provider/customer-management/create-new-customer) uw eerste klant in Azure CSP en implementeer Azure-services.

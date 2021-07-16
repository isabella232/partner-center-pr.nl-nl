---
title: Voorbeeldtoepassing
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Gebruik de voorbeeldtoepassing om uw eigen toepassing te bouwen om programmatisch toegang te krijgen tot partnerinzichtgegevens.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: 6f334b9047c38e8b7763a4ba96d21d987c252682
ms.sourcegitcommit: 4f1702683336d54f24c0ba283f7d13dda581923d
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/16/2021
ms.locfileid: "114376508"
---
# <a name="sample-application"></a><span data-ttu-id="36d08-103">Voorbeeldtoepassing</span><span class="sxs-lookup"><span data-stu-id="36d08-103">Sample Application</span></span>

<span data-ttu-id="36d08-104">Voorbeeldtoepassingen worden gemaakt in C# en JAVA en zijn beschikbaar op [GitHub](https://github.com/partneranalytics)</span><span class="sxs-lookup"><span data-stu-id="36d08-104">Sample applications are created in C# and JAVA languages and are available on [GitHub](https://github.com/partneranalytics)</span></span>

- [<span data-ttu-id="36d08-105">C#-voorbeeldtoepassing</span><span class="sxs-lookup"><span data-stu-id="36d08-105">C# Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [<span data-ttu-id="36d08-106">JAVA-voorbeeldtoepassing</span><span class="sxs-lookup"><span data-stu-id="36d08-106">JAVA Sample Application</span></span>](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

<span data-ttu-id="36d08-107">U kunt ervoor kiezen om zich te laten inspireren door de voorbeeldtoepassing en uw eigen toepassing in elke taal te bouwen.</span><span class="sxs-lookup"><span data-stu-id="36d08-107">You can choose to take inspiration from the sample application and build your own application in any language.</span></span>

<span data-ttu-id="36d08-108">De voorbeeldtoepassing bereikt de volgende doelstellingen:</span><span class="sxs-lookup"><span data-stu-id="36d08-108">The sample application achieves the following objectives:</span></span>

- <span data-ttu-id="36d08-109">Genereert een Azure Active Directory (Azure AD)-token.</span><span class="sxs-lookup"><span data-stu-id="36d08-109">Generates an Azure Active Directory (Azure AD) Token.</span></span>
- <span data-ttu-id="36d08-110">Haalt beschikbare gegevenssets op.</span><span class="sxs-lookup"><span data-stu-id="36d08-110">Gets available datasets.</span></span>
- <span data-ttu-id="36d08-111">Hiermee maakt u door de gebruiker gedefinieerde query's.</span><span class="sxs-lookup"><span data-stu-id="36d08-111">Creates user defined queries.</span></span>
- <span data-ttu-id="36d08-112">Haalt door de gebruiker gedefinieerde en systeemquery's op.</span><span class="sxs-lookup"><span data-stu-id="36d08-112">Gets user defined and system queries.</span></span>
- <span data-ttu-id="36d08-113">Een rapport plannen.</span><span class="sxs-lookup"><span data-stu-id="36d08-113">Schedules a report.</span></span>

<span data-ttu-id="36d08-114">De voorbeeldtoepassing heeft geen betrekking op de methode voor het aanroepen van API's voor andere functies.</span><span class="sxs-lookup"><span data-stu-id="36d08-114">The sample application doesn't cover the method of calling APIs for other functionalities.</span></span> <span data-ttu-id="36d08-115">Het proces voor het aanroepen van andere API's blijft echter hetzelfde als hierboven wordt beschreven.</span><span class="sxs-lookup"><span data-stu-id="36d08-115">However, the process of calling other APIs remains the same as outlined above.</span></span>

## <a name="how-to-run-the-application"></a><span data-ttu-id="36d08-116">De toepassing uitvoeren</span><span class="sxs-lookup"><span data-stu-id="36d08-116">How to run the application</span></span>

- <span data-ttu-id="36d08-117">Kloon de opslagplaats naar een lokaal systeem met behulp van deze opdracht:</span><span class="sxs-lookup"><span data-stu-id="36d08-117">Clone the repository to a local system using this command:</span></span>

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> <span data-ttu-id="36d08-118">Raadpleeg het bestand ProgrammaticExportSampleAppMPN/README.md in de opslagplaats GitHub [lezen voor meer instructies.](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)</span><span class="sxs-lookup"><span data-stu-id="36d08-118">For more instructions, refer to the ProgrammaticExportSampleAppMPN/README.md file in the GitHub [repository](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java).</span></span>

- <span data-ttu-id="36d08-119">Als u de app snel wilt uitvoeren, moet u de client-id en het clientgeheim in de **appsettings.Development.jsop**</span><span class="sxs-lookup"><span data-stu-id="36d08-119">To quickly run the app, update the client id and client secret in the **appsettings.Development.json**</span></span>

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="JSON voor appsetting-ontwikkeling illustreren":::

<span data-ttu-id="36d08-121">Als de app wordt uitgevoerd, wordt een lokale webserver geopend en wordt een pagina geopend ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).</span><span class="sxs-lookup"><span data-stu-id="36d08-121">Running the app will start a local web server and a page will open (`https://localhost:44365/ProgrammaticExportSampleApp/sample`).</span></span>
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="De gebruikersinterface van de voorbeeldtoepassing illustreren":::

<span data-ttu-id="36d08-123">Op deze pagina worden API-aanroepen naar de webserver uitgevoerd op de lokale computer, die op zijn beurt de werkelijke API-aanroepen voor programmatische toegang maakt.</span><span class="sxs-lookup"><span data-stu-id="36d08-123">This page will make API calls to the webserver running on the local machine, which in turn will make the actual programmatic access API calls.</span></span>

## <a name="code-snippets"></a><span data-ttu-id="36d08-124">Codefragmenten</span><span class="sxs-lookup"><span data-stu-id="36d08-124">Code Snippets</span></span>

<span data-ttu-id="36d08-125">De basisstructuur van de C#-code voor het uitvoeren van api-aanroepen voor programmatische toegang is als volgt:</span><span class="sxs-lookup"><span data-stu-id="36d08-125">The basic structure of the C# code for doing the programmatic access API calls is as follows:</span></span>
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Codefragment illustreren":::

## <a name="next-steps"></a><span data-ttu-id="36d08-127">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="36d08-127">Next steps</span></span>

[<span data-ttu-id="36d08-128">API's voor toegang tot analysegegevens van partnerinzichten</span><span class="sxs-lookup"><span data-stu-id="36d08-128">APIs for accessing partner insights analytics data</span></span>](insights-programmatic-analytics-available-api.md)

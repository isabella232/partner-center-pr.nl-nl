---
title: Voorbeeldtoepassing
ms.topic: article
ms.date: 07/14/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-insights
description: Gebruik de voorbeeldtoepassing om uw eigen toepassing te bouwen om programmatisch toegang te krijgen tot partnerinzichtgegevens.
author: shganesh-dev
ms.author: shganesh
ms.localizationpriority: medium
ms.openlocfilehash: c558852b7c2af7243187a856067d17a2137cfac867149b80e9c852a1d08d780a
ms.sourcegitcommit: 121f1b9cbd88faeba60dc9b475f9c0647cdc933c
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/06/2021
ms.locfileid: "115683756"
---
# <a name="sample-application"></a>Voorbeeldtoepassing

Voorbeeldtoepassingen worden gemaakt in C# en JAVA en zijn beschikbaar op [GitHub](https://github.com/partneranalytics)

- [C#-voorbeeldtoepassing](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN)
- [JAVA-voorbeeldtoepassing](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

U kunt ervoor kiezen om zich te laten inspireren door de voorbeeldtoepassing en uw eigen toepassing in elke taal te bouwen.

De voorbeeldtoepassing bereikt de volgende doelstellingen:

- Genereert een Azure Active Directory (Azure AD)-token.
- Haalt beschikbare gegevenssets op.
- Hiermee maakt u door de gebruiker gedefinieerde query's.
- Haalt door de gebruiker gedefinieerde en systeemquery's op.
- Een rapport plannen.

De voorbeeldtoepassing heeft geen betrekking op de methode voor het aanroepen van API's voor andere functies. Het proces voor het aanroepen van andere API's blijft echter hetzelfde als hierboven wordt beschreven.

## <a name="how-to-run-the-application"></a>De toepassing uitvoeren

- Kloon de opslagplaats naar een lokaal systeem met behulp van deze opdracht:

```cli
git clone https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN.git
```

> [!Note]
> Raadpleeg het bestand ProgrammaticExportSampleAppMPN/README.md in de opslagplaats GitHub lezen voor [meer instructies.](https://github.com/partneranalytics/ProgrammaticExportSampleAppMPN_Java)

- Als u de app snel wilt uitvoeren, moet u de client-id en het clientgeheim in de **appsettings.Development.jsop**

:::image type="content" source="images/insights/prog-acc-appsetting-development.png" alt-text="JSON voor appsetting-ontwikkeling illustreren":::

Als de app wordt uitgevoerd, wordt een lokale webserver geopend en wordt een pagina geopend ( `https://localhost:44365/ProgrammaticExportSampleApp/sample` ).
  
:::image type="content" source="images/insights/prog-acc-sample-application.png" alt-text="De gebruikersinterface van de voorbeeldtoepassing illustreren":::

Op deze pagina worden API-aanroepen naar de webserver uitgevoerd op de lokale computer, die op zijn beurt de werkelijke API-aanroepen voor programmatische toegang maakt.

## <a name="code-snippets"></a>Codefragmenten

De basisstructuur van de C#-code voor het uitvoeren van api-aanroepen voor programmatische toegang is als volgt:
 
:::image type="content" source="images/insights/prog-acc-code-snippet.png" alt-text="Codefragment illustreren":::

## <a name="next-steps"></a>Volgende stappen

[API's voor toegang tot analysegegevens van partnerinzichten](insights-programmatic-analytics-available-api.md)

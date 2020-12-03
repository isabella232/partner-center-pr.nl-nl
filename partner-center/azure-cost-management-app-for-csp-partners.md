---
title: Azure Cost Management van Cloudyn voor CSP's
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over het registreren van de Cloudyn-web-app en het gebruik van een geheime sleutel voor IT in het partner centrum, zodat u de app kunt gebruiken om het Azure-gebruik en de kosten van klanten bij te houden.
author: aparnagkrishnan
ms.author: aparnag
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: defa691a3bc70cbda45f01cb447d89364a49e3b8
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534982"
---
# <a name="track-customer-azure-usage-and-costs-with-the-azure-cost-management-app-for-csp-partners"></a>Het Azure-gebruik en de kosten van klanten bijhouden met de Azure cost management-app voor CSP-partners  

**Juiste rollen**

- Globale beheerder
- Beheer agent

[Meer informatie over Azure Cost Management](https://go.microsoft.com/fwlink/p/?linkid=857893)

## <a name="before-you-begin"></a>Voordat u begint
Zorg ervoor dat u voldoet aan de volgende vereisten voordat u Azure Cost Management kunt gebruiken:

- U bent een partner in het Cloud Solution Provider-programma.
- U hebt de mogelijkheid om een partner centrum API-Web-app te maken.

## <a name="overview"></a>Overzicht

Cloudyn is een web-app waarmee u kunt bijhouden en beheren hoeveel uw klanten Azure gebruiken en wat de kosten voor dat gebruik zijn. U gebruikt dit via de partner centrum-API.

## <a name="register-your-web-app-in-the-partner-center"></a>Uw web-app registreren in het partner centrum
Wanneer u een Azure Active Directory Web-app registreert in het partner centrum, schakelt u de toegang tot de partner centrum-API in. 
1.  Meld u aan bij [partner centrum](https://partnercenter.microsoft.com/pcv/dashboard/overview) met een [account voor globale beheerders of beheerders agenten](create-user-accounts-and-set-permissions.md).
2.  Selecteer in het **partner centrum** **account instellingen** &gt; **[app-beheer](https://partnercenter.microsoft.com/pcv/apiintegration/appmanagement)**.
3.  Klik in de sectie **Web-app** op **nieuwe web-app toevoegen**.
<br> **Opmerking**: als u eerder een web-app hebt gemaakt, kunt u stap 3 overs Laan.
4.  Kopieer en sla de **Commerce ID-** GUID en de **App-ID-** GUID voor uw web-app op. U hebt beide Id's nodig om de gratis proef versie van 30 dagen van de Azure cost management-app te kunnen gebruiken.

## <a name="add-a-secret-key-to-your-app"></a>Een geheime sleutel toevoegen aan uw app
1. Selecteer in de vervolg keuzelijst naast de knop **sleutel toevoegen** een duur van 1 of 2 jaar.
2. Klik op **sleutel toevoegen**. 
3. Kopieer de waarde van de geheime sleutel en sla deze op. Dit hebt u nodig voor de gratis proef versie van 30 dagen.<br>
   > [!NOTE]  
   > De geheime sleutels van de toepassing zijn net als wacht woorden met langere verval datums. Sla de sleutel waarde op een veilige locatie op voor toekomstig gebruik.

## <a name="next-steps"></a>Volgende stappen
Start een [gratis proef versie van 30 dagen](https://go.microsoft.com/fwlink/?linkid=857895).
U hebt de volgende gegevens nodig om de proef versie te starten:
- Aanmeldings referenties Partner Center
- Commerce ID-GUID
- App-ID-GUID
- Waarde van geheime sleutel van toepassing

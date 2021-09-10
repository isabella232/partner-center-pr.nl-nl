---
title: Rollen, machtigingen voor partnertegoed
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over de rollen en machtigingen voor partners om partnertegoeden (PEC) te kunnen verdienen. Deze verschillen van rollen om in een Partner Center.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ca9cd1b09c840531c3652f71afbd9c66f657f877
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123956836"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Rollen en machtigingen die vereist zijn om partnertegoed te verdienen

De volgende rollen worden toewijzen aan machtigingsniveaus die bepalen of een partner in aanmerking komt voor partnertegoeden.

>[!Important]
>Deze rollen en machtigingen zijn niet hetzelfde als de rollen en machtigingen die een gebruiker nodig heeft om in de Partner Center.

|**Role**   |**Beschrijving**   |**In aanmerking komend voor PEC**   |
|-----------------|:------------------|:--------------|
|Eigenaar  |U beheert alles, inclusief toegang tot resources.|Yes|
|Inzender |U beheert alles behalve het verlenen van toegang tot resources.|Yes|
|Lezer|U kunt alles bekijken, maar geen wijzigingen aanbrengen|No|
|ACRDelete|acr delete|Yes|
|ACRImageSigner|acr image signer|Yes|
|ACRPull|acr pull|Yes|
|AcrPush|acr push|Yes|
|AcrQuarantineReader|acr quarantine data reader|No|
|AcrQuarantineWriter| acr quarantine data writer|Yes|
|inzender API Management-service|Kan de service en de API's beheren|Yes|
|API Management rol serviceoperator|Kan de service beheren, maar niet de API's|Yes|
|API Management rol servicelezer|Alleen-lezentoegang tot service en API's|No|
|Inzender Insights toepassingsonderdeel|Toepassingsonderdelen Insights beheren|Yes|
|Toepassings Insights Snapshot Debugger|Geeft de gebruiker toestemming om momentopnamen voor foutopsporing weer te geven en te downloaden die zijn verzameld met application Insights Snapshot Debugger. Houd er rekening mee dat deze machtigingen niet zijn opgenomen in de rollen Eigenaar of Inzender.|Yes|
Automation-taakoperator | Taken maken en beheren met Automation-runbooks. | Yes | 
Automation-operator | Automation-operators kunnen taken starten, stoppen, opschorten en hervatten | Yes | 
Automation-runbookoperator | Runbookeigenschappen lezen: om taken van het runbook te kunnen maken. | Yes | 
Avere-inzender | Kan een cluster met Avere vFXT maken en beheren. | Yes | 
Avere-operator | Wordt gebruikt door het Avere vFXT cluster om het cluster te beheren | Yes | 
Azure Event Hubs gegevenseigenaar | Biedt volledige toegang tot Azure Event Hubs resources. | Yes | 
Azure Event Hubs-ontvanger | Hiermee krijgt u toegang tot Azure Event Hubs resources. | Yes | 
Azure Event Hubs Afzender van gegevens | Hiermee kunt u toegang tot Azure Event Hubs verzenden. | Yes | 
Azure Kubernetes Service rol clusterbeheerder | De actie Clusterbeheerderreferenties opsommen. | Yes | 
Azure Kubernetes Service clustergebruikersrol | Lijst met gebruikersreferenties voor cluster. | Yes | 
Azure Kaarten-gegevenslezer (preview) | Verleent toegang tot het lezen van kaartgerelateerde gegevens uit een Azure Maps-account. | No | 
Azure Service Bus-gegevenseigenaar | Biedt volledige toegang tot Azure Service Bus resources. | Yes | 
Azure Service Bus-gegevensontvanger | Hiermee kunt u toegang krijgen tot Azure Service Bus resources. | Yes | 
Azure Service Bus Data Sender | Hiermee kunt u toegang tot Azure Service Bus verzenden. | Yes | 
Azure Stack registratie-eigenaar | Hiermee kunt u Azure Stack beheren. | Yes | 
Back-upbijdrager | Hiermee kunt u de back-upservice beheren, maar u kunt geen kluizen maken en toegang verlenen aan anderen | Yes | 
Back-upoperator | Hiermee kunt u back-upservices beheren, behalve het verwijderen van back-up, het maken van de kluis en het verlenen van toegang aan anderen | Yes | 
Back-uplezer | Kan back-upservices weergeven, maar kan geen wijzigingen aanbrengen | No | 
Lezer voor facturering | Hiermee staat u leestoegang tot factureringsgegevens toe | No | 
BizTalk Contributor | Hiermee kunt u BizTalk Services beheren, maar geen toegang krijgen tot deze services. | Yes | 
Toegang tot blockchain-lid-knooppunt (preview) | Hiermee kunt u toegang krijgen tot blockchain-lidknooppunten | Yes | 
Blauwdrukinzender | Blauwdrukinzenders kunnen blauwdrukdefinities beheren, maar deze niet toewijzen. | Yes | 
Blauwdrukoperator | Kan bestaande gepubliceerde blauwdrukken toewijzen, maar kan geen nieuwe blauwdrukken maken. OPMERKING: dit werkt alleen als de toewijzing wordt uitgevoerd met een door de gebruiker toegewezen beheerde identiteit. | Yes | 
CDN Inzender voor eindpunten | Kan CDN eindpunten beheren, maar kan geen toegang verlenen aan andere gebruikers. | Yes | 
CDN Eindpuntlezer | Kan CDN eindpunten weergeven, maar kan geen wijzigingen aanbrengen. | No | 
CDN Profielbijdrager | Kan CDN en hun eindpunten beheren, maar kan geen toegang verlenen aan andere gebruikers. | Yes | 
CDN Profiellezer | Kan de CDN en hun eindpunten weergeven, maar kan geen wijzigingen aanbrengen. | No | 
Inzender voor klassieke netwerken | Hiermee kunt u klassieke netwerken beheren, maar geen toegang tot deze netwerken. | Yes | 
Inzender Storage klassieke Storage account | Hiermee kunt u klassieke opslagaccounts beheren, maar geen toegang tot deze accounts. | Yes | 
Klassieke Storage servicerol Sleuteloperator voor account | Klassieke Storage-accountsleuteloperators mogen sleutels op klassieke en klassieke Storage accounts | Yes | 
Inzender voor klassieke virtuele machines | Hiermee kunt u klassieke virtuele machines beheren, maar geen toegang tot deze machines, en niet tot het virtuele netwerk of opslagaccount waarmee ze zijn verbonden. | Yes | 
Cognitive Services inzender | Hiermee kunt u sleutels van de Cognitive Services. | Yes | 
Cognitive Services Gegevenslezer (preview) | Hiermee kunt u Cognitive Services lezen. | No | 
Cognitive Services gebruiker | Hiermee kunt u sleutels van de Cognitive Services. | No | 
Cosmos DB rol accountlezer | Kan de Azure Cosmos DB lezen. Zie Inzender voor DocumentDB-accounts voor het beheren Azure Cosmos DB accounts. | No | 
Cosmos DB Operator | Hiermee kunt u Azure Cosmos DB beheren, maar geen toegang krijgen tot gegevens in deze accounts. Hiermee voorkomt u toegang tot accountsleutels en verbindingsreeksen. | Yes | 
CosmosBackupOperator | Kan een herstelaanvraag indienen voor een Cosmos DB database of een container voor een account | Yes | 
Cost Management-inzender | Kan kosten bekijken en de kostenconfiguratie beheren (bijvoorbeeld budgetten, exports) | Yes | 
Cost Management Reader | Kan kostengegevens en -configuraties weergeven (bijvoorbeeld budgetten, exports) | No | 
Data Box Inzender | Hiermee kunt u alles beheren onder Data Box Service, behalve toegang te verlenen aan anderen. | Yes | 
Data Box Lezer | Hiermee kunt u de Data Box beheren, behalve het maken van order- of bewerkingsgegevens en het verlenen van toegang aan anderen. | No | 
Data Factory-inzender | Maak en beheer gegevensfabrieken en onderliggende resources in deze resources. | Yes | 
Data Lake Analytics Developer | Hiermee kunt u uw eigen taken verzenden, bewaken en beheren, maar geen Data Lake Analytics maken of verwijderen. | Yes | 
Gegevens ops purger | Kan analysegegevens opseen | Yes | 
DevTest Labs-gebruiker | Hiermee kunt u uw virtuele machines in uw omgeving verbinden, starten, opnieuw opstarten en afsluiten Azure DevTest Labs. | Yes | 
Inzender voor DNS-zone | Hiermee kunt u DNS-zones en -recordsets in Azure DNS beheren, maar kunt u niet bepalen wie er toegang toe heeft. | Yes | 
Inzender voor DocumentDB-account | Kan uw Azure Cosmos DB beheren. Azure Cosmos DB staat voorheen bekend als DocumentDB. | Yes | 
EventGrid EventSubscription Contributor | Hiermee kunt u eventgrid-gebeurtenisabonnementbewerkingen beheren. | Yes | 
EventGrid EventSubscription Reader | Hiermee kunt u EventGrid-gebeurtenisabonnementen lezen. | No | 
HDInsight-clusteroperator | Hiermee kunt u HDInsight-clusterconfiguraties lezen en wijzigen. | Yes | 
Inzender voor HDInsight Domain Services | Kan domain services-gerelateerde bewerkingen lezen, maken, wijzigen en verwijderen die nodig zijn voor HDInsight-Enterprise Security Package | Yes | 
Inzender voor Intelligent Systems-account | Hiermee kunt u Intelligent Systems-accounts beheren, maar geen toegang tot deze accounts. | Yes | 
Key Vault Inzender | Hiermee kunt u sleutelkluizen beheren, maar geen toegang tot deze kluizen. | Yes | 
Labmaker | Hiermee kunt u uw beheerde labs maken, beheren en verwijderen onder uw Azure Lab-accounts. | Yes | 
Inzender van Log Analytics | Log Analytics-inzender kan alle bewakingsgegevens lezen en bewakingsinstellingen bewerken. Het bewerken van bewakingsinstellingen omvat het toevoegen van de VM-extensie aan VM's; lezen van opslagaccountsleutels om het verzamelen van logboeken van de Azure Storage; Automation-accounts maken en configureren; oplossingen toevoegen; en azure diagnostics configureren voor alle Azure-resources. | Yes | 
Lezer van Log Analytics | Log Analytics-lezer kan alle bewakingsgegevens bekijken en doorzoeken, evenals bewakingsinstellingen, inclusief het bekijken van de configuratie van diagnostische gegevens van Azure voor alle Azure-resources. | No | 
Inzender voor logische apps | Hiermee kunt u logische apps beheren, maar de toegang tot deze apps niet wijzigen. | Yes | 
Logische app-operator | Hiermee kunt u logische apps lezen, inschakelen en uitschakelen, maar niet bewerken of bijwerken. | Yes | 
Operatorrol voor beheerde toepassingen | Hiermee kunt u acties lezen en uitvoeren op resources van beheerde toepassingen | Yes | 
Lezer voor beheerde toepassingen | Hiermee kunt u resources in een beheerde app lezen en JIT-toegang aanvragen. | No | 
Inzender voor beheerde identiteit | Door de gebruiker toegewezen identiteit maken, lezen, bijwerken en verwijderen | Yes | 
Operator voor beheerde identiteit | Door de gebruiker toegewezen identiteit lezen en toewijzen | Yes | 
Inzender voor beheergroep | Rol inzender voor beheergroep | Yes | 
Lezer van beheergroep | Rol van lezer van beheergroep | No | 
Controlebijdrager | Kan alle bewakingsgegevens lezen en bewakingsinstellingen bewerken. Zie ook Aan de slag met rollen, machtigingen en beveiliging met Azure Monitor. | Yes | 
Monitoring Metrics Publisher | Hiermee kunt u metrische gegevens publiceren op Basis van Azure-resources | Yes | 
Lezer voor bewaking | Kan alle bewakingsgegevens (metrische gegevens, logboeken, enzovoort) lezen. Zie ook Aan de slag met rollen, machtigingen en beveiliging met Azure Monitor. | No | 
Inzender voor netwerken | Hiermee kunt u netwerken beheren, maar geen toegang tot deze netwerken. | Yes | 
New Relic APM-account inzender | Hiermee kunt u New Relic Application Performance Management accounts en toepassingen beheren, maar geen toegang tot deze accounts. | Yes | 
Lezer en gegevenstoegang | Hiermee kunt u alles weergeven, maar u kunt geen opslagaccount of ingesloten resource verwijderen of maken. Het biedt ook lees-/schrijftoegang tot alle gegevens in een opslagaccount via toegang tot opslagaccountsleutels. | Yes | 
Redis Cache-inzender | Hiermee kunt u Redis-caches beheren, maar geen toegang tot deze caches. | Yes | 
Inzender voor resourcebeleid (preview) | (Preview) Backfilled gebruikers van EA, met rechten voor het maken/wijzigen van resourcebeleid, het maken van ondersteuningstickets en het lezen van resources/hiërarchie. | Yes | 
Inzender voor Scheduler-taakverzamelingen | Hiermee kunt u Scheduler-taakverzamelingen beheren, maar geen toegang tot deze verzamelingen. | Yes | 
Inzender voor search-service | Hiermee kunt u zoekservices beheren, maar geen toegang tot deze services. | Yes | 
Beveiligingsbeheerder | Alleen Security Center: Kan beveiligingsbeleid weergeven, beveiligingswaarschuwingen bekijken, beveiligingsbeleid bewerken, waarschuwingen en aanbevelingen bekijken, waarschuwingen en aanbevelingen afwijzen | Yes | 
Security Manager (verouderd) | Dit is een verouderde rol. Gebruik in plaats daarvan Beveiligingsbeheerder | Yes | 
Beveiligingslezer | Alleen Security Center: Kan aanbevelingen en waarschuwingen bekijken, beveiligingsbeleid weergeven, beveiligingswaarschuwingen bekijken, maar geen wijzigingen aanbrengen | No | 
Site Recovery-inzender | Hiermee kunt u Site Recovery beheren, behalve het maken van een kluis en roltoewijzing | Yes | 
Site Recovery-operator | Hiermee kunt u failover en failback uitvoeren, maar geen andere beheerbewerkingen Site Recovery uitvoeren | Yes | 
Site Recovery-lezer | Hiermee kunt u de Site Recovery weergeven, maar geen andere beheerbewerkingen uitvoeren | No | 
Spatial Anchors accountbijdrager | Hiermee kunt u spatial anchors in uw account beheren, maar niet verwijderen | Yes | 
Spatial Anchors accounteigenaar | Hiermee kunt u ruimtelijke ankers in uw account beheren, inclusief het verwijderen ervan | Yes | 
Spatial Anchors-accountlezer | Hiermee kunt u eigenschappen van ruimtelijke ankers in uw account zoeken en lezen | No | 
SQL Inzender voor db | Hiermee kunt u SQL databases beheren, maar geen toegang tot deze databases. U kunt ook hun beveiligingsbeleid of hun bovenliggende SQL beheren. | Yes | 
SQL Inzender voor beheerd exemplaar | Hiermee kunt u SQL beheerde exemplaren en de vereiste netwerkconfiguratie beheren, maar kunt u geen toegang verlenen aan anderen. | Yes | 
SQL-beveiligingsbeheerder | Hiermee kunt u het beveiligingsbeleid van SQL servers en databases beheren, maar geen toegang tot deze servers. | Yes | 
SQL Server Inzender | Hiermee kunt u SQL servers en databases beheren, maar geen toegang krijgen tot deze servers en niet het bijbehorende beveiligingsbeleid. | Yes | 
Inzender voor opslagaccounts | Staat beheer van opslagaccounts toe. Biedt toegang tot de accountsleutel, die kan worden gebruikt voor toegang tot gegevens via gedeelde sleutelautorisatie. | Yes | 
Storage Servicerol accountsleuteloperator | Maakt het mogelijk om toegangssleutels voor opslagaccounts weer te geven en opnieuw te gebruiken. | Yes | 
Inzender voor Storage Blob-gegevens | Lees, schrijf en verwijder Azure Storage containers en blobs. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Yes | 
Eigenaar van opslagblobgegevens | Biedt volledige toegang tot Azure Storage blobcontainers en -gegevens, inclusief het toewijzen van POSIX-toegangsbeheer. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Yes | 
Lezer voor opslagblobgegevens | Lees en vermeld Azure Storage containers en blobs. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | No | 
Storage Blob-delegator | Haal een sleutel voor gebruikersdelegatie op, die vervolgens kan worden gebruikt om een Shared Access Signature te maken voor een container of blob die is ondertekend met Azure AD-referenties. Zie Create a user delegation SAS (Een SAS voor gebruikersdelegatie maken) voor meer informatie. | Yes | 
Inzender voor opslagbestandsgegevens via SMB-share | Hiermee kunt u lezen, schrijven en verwijderen van toegang in Azure Storage via SMB | Yes | 
Inzender met verhoogde bevoegdheden voor opslagbestandsgegevens via SMB-share | Staat toegang tot NTFS-machtigingen voor lezen, schrijven, verwijderen en wijzigen toe in Azure Storage via SMB | Yes | 
Lezer voor opslagbestandgegevens via SMB-share | Staat leestoegang tot Azure-bestands delen via SMB toe | No | 
Storage Inzender voor wachtrijgegevens | Lees, schrijf en verwijder Azure Storage wachtrijen en wachtrijberichten. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Yes | 
Storage Wachtrijgegevensberichtprocessor | Een bericht bekijken, ophalen en verwijderen uit een Azure Storage wachtrij. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Yes | 
Storage Afzender van wachtrijgegevensbericht | Berichten toevoegen aan een Azure Storage wachtrij. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Yes | 
Storage Lezer van wachtrijgegevens | Lees en vermeld Azure Storage wachtrijen en wachtrijberichten. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | No | 
Inzender voor ondersteuningsaanvraag | Hiermee kunt u ondersteuningsaanvragen maken en beheren | Yes | 
Traffic Manager Inzender | Hiermee kunt u Traffic Manager beheren, maar kunt u niet bepalen wie er toegang tot heeft. | Yes | 
Beheerder van gebruikerstoegang | Hiermee kunt u gebruikerstoegang tot Azure-resources beheren. | Yes | 
Aanmeldgegevens van de beheerder van de virtuele machine | Uw Virtual Machines weergeven in de portal en u aanmelden als beheerder | Yes | 
Inzender voor virtuele machines | Hiermee kunt u virtuele machines beheren, maar geen toegang krijgen tot deze machines, en niet tot het virtuele netwerk of opslagaccount waarmee ze zijn verbonden. | Yes | 
Gebruikersmelding voor virtuele machine | Bekijk Virtual Machines in de portal en meld u aan als een gewone gebruiker. | Yes | 
Inzender voor webplannen | Hiermee kunt u de webplannen voor websites beheren, maar geen toegang tot de websites. | Yes | 
Inzender voor websites | Hiermee kunt u websites beheren (geen webplannen), maar geen toegang tot websites | Ja |

## <a name="next-steps"></a>Volgende stappen

- [Partnertegoed: een overzicht van hoe het werkt in de nieuwe commerce-ervaring in CSP](partner-earned-credit.md)

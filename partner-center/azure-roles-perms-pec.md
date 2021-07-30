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
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114840379"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Rollen en machtigingen die vereist zijn om partnertegoed te verdienen

De volgende rollen worden toewijzen aan machtigingsniveaus die bepalen of een partner in aanmerking komt voor partnertegoeden.

>[!Important]
>Deze rollen en machtigingen zijn niet hetzelfde als de rollen en machtigingen die een gebruiker nodig heeft om te werken in Partner Center.

|**Role**   |**Beschrijving**   |**In aanmerking komend voor PEC**   |
|-----------------|:------------------|:--------------|
|Eigenaar  |U beheert alles, inclusief toegang tot resources.|Ja|
|Inzender |U beheert alles behalve het verlenen van toegang tot resources.|Ja|
|Lezer|U kunt alles bekijken, maar geen wijzigingen aanbrengen|Nee|
|ACRDelete|acr delete|Ja|
|ACRImageSigner|acr image signer|Ja|
|ACRPull|acr pull|Ja|
|AcrPush|acr push|Ja|
|AcrQuarantineReader|acr quarantine data reader|Nee|
|AcrQuarantineWriter| acr quarantine data writer|Ja|
|API Management-servicebijdrager|Kan de service en de API's beheren|Ja|
|API Management Rol serviceoperator|Kan de service beheren, maar niet de API's|Ja|
|API Management rol servicelezer|Alleen-lezentoegang tot service en API's|Nee|
|Inzender Insights toepassingsonderdeel|Toepassingsonderdelen Insights beheren|Ja|
|Toepassings Insights Snapshot Debugger|Geeft de gebruiker toestemming om momentopnamen voor foutopsporing weer te geven en te downloaden die zijn verzameld met application Insights Snapshot Debugger. Houd er rekening mee dat deze machtigingen niet zijn opgenomen in de rollen Eigenaar of Inzender.|Ja|
Automation-taakoperator | Taken maken en beheren met Automation-runbooks. | Ja | 
Automation-operator | Automation-operators kunnen taken starten, stoppen, opschorten en hervatten | Ja | 
Automation-runbookoperator | Runbookeigenschappen lezen: om taken van het runbook te kunnen maken. | Ja | 
Avere-inzender | Kan een cluster met Avere vFXT maken en beheren. | Ja | 
Avere-operator | Wordt gebruikt door het Avere vFXT cluster om het cluster te beheren | Ja | 
Azure Event Hubs gegevenseigenaar | Biedt volledige toegang tot Azure Event Hubs resources. | Ja | 
Azure Event Hubs Ontvanger van gegevens | Hiermee krijgt u toegang tot Azure Event Hubs resources. | Ja | 
Azure Event Hubs Afzender van gegevens | Hiermee kunt u toegang tot Azure Event Hubs resources verzenden. | Ja | 
Azure Kubernetes Service rol clusterbeheerder | De actie Clusterbeheerderreferenties opsommen. | Ja | 
Azure Kubernetes Service clustergebruikersrol | Lijst met gebruikersreferenties voor cluster. | Ja | 
Azure Kaarten Data Reader (preview) | Verleent toegang tot het lezen van kaartgerelateerde gegevens uit een Azure Maps-account. | Nee | 
Azure Service Bus-gegevenseigenaar | Biedt volledige toegang tot Azure Service Bus resources. | Ja | 
Azure Service Bus-gegevensontvanger | Hiermee kunt u toegang krijgen tot Azure Service Bus resources. | Ja | 
Azure Service Bus Data Sender | Hiermee kunt u toegang tot Azure Service Bus verzenden. | Ja | 
Azure Stack registratie-eigenaar | Hiermee kunt u Azure Stack beheren. | Ja | 
Back-upbijdrager | Hiermee kunt u de back-upservice beheren, maar geen kluizen maken en toegang verlenen aan anderen | Ja | 
Back-upoperator | Hiermee kunt u back-upservices beheren, behalve het verwijderen van back-ups, het maken van een kluis en het verlenen van toegang aan anderen | Ja | 
Back-uplezer | Kan back-upservices weergeven, maar kan geen wijzigingen aanbrengen | Nee | 
Lezer voor facturering | Hiermee staat u leestoegang tot factureringsgegevens toe | Nee | 
BizTalk Contributor | Hiermee kunt u BizTalk Services beheren, maar geen toegang krijgen tot deze services. | Ja | 
Toegang tot blockchain-lid-knooppunt (preview) | Hiermee kunt u toegang krijgen tot knooppunten die lid zijn van blockchain | Ja | 
Blauwdrukinzender | Blauwdrukinzenders kunnen blauwdrukdefinities beheren, maar deze niet toewijzen. | Ja | 
Blauwdrukoperator | Kan bestaande gepubliceerde blauwdrukken toewijzen, maar kan geen nieuwe blauwdrukken maken. OPMERKING: dit werkt alleen als de toewijzing wordt uitgevoerd met een door de gebruiker toegewezen beheerde identiteit. | Ja | 
CDN Inzender voor eindpunten | Kan CDN eindpunten beheren, maar kan geen toegang verlenen aan andere gebruikers. | Ja | 
CDN Eindpuntlezer | Kan CDN eindpunten weergeven, maar kan geen wijzigingen aanbrengen. | Nee | 
CDN Profielbijdrager | Kan CDN en hun eindpunten beheren, maar kan geen toegang verlenen aan andere gebruikers. | Ja | 
CDN Profiellezer | Kan de CDN en hun eindpunten weergeven, maar kan geen wijzigingen aanbrengen. | Nee | 
Inzender voor klassieke netwerken | Hiermee kunt u klassieke netwerken beheren, maar geen toegang tot deze netwerken. | Ja | 
Inzender Storage klassieke Storage account | Hiermee kunt u klassieke opslagaccounts beheren, maar geen toegang tot deze accounts. | Ja | 
Klassieke Storage servicerol Sleuteloperator voor het account | Klassieke Storage-accountsleuteloperators mogen sleutels op klassieke Storage-accounts in een lijst en opnieuw Storage. | Ja | 
Inzender voor klassieke virtuele machines | Hiermee kunt u klassieke virtuele machines beheren, maar geen toegang krijgen tot deze machines, en niet het virtuele netwerk of het opslagaccount waarmee ze zijn verbonden. | Ja | 
Cognitive Services-inzender | Hiermee kunt u sleutels van de Cognitive Services. | Ja | 
Cognitive Services Gegevenslezer (preview) | Hiermee kunt u Cognitive Services lezen. | Nee | 
Cognitive Services gebruiker | Hiermee kunt u sleutels van de Cognitive Services. | Nee | 
Cosmos DB rol accountlezer | Kan de Azure Cosmos DB lezen. Zie Inzender voor DocumentDB-accounts voor het beheren van Azure Cosmos DB accounts. | Nee | 
Cosmos DB Operator | Hiermee kunt u Azure Cosmos DB accounts beheren, maar geen toegang krijgen tot gegevens in deze accounts. Hiermee voorkomt u toegang tot accountsleutels en verbindingsreeksen. | Ja | 
CosmosBackupOperator | Kan een herstelaanvraag indienen voor een Cosmos DB database of een container voor een account | Ja | 
Cost Management-inzender | Kan kosten bekijken en kostenconfiguratie beheren (bijvoorbeeld budgetten, exports) | Ja | 
Cost Management Reader | Kan kostengegevens en -configuratie weergeven (bijvoorbeeld budgetten, exports) | Nee | 
Data Box-inzender | Hiermee kunt u alles beheren onder Data Box Service, behalve toegang te verlenen aan anderen. | Ja | 
Data Box Reader | Hiermee kunt u de Data Box beheren, behalve het maken van order- of bewerkingsgegevens en het verlenen van toegang aan anderen. | Nee | 
Data Factory-inzender | Maak en beheer gegevensfabrieken en onderliggende resources in deze resources. | Ja | 
Data Lake Analytics Developer | Hiermee kunt u uw eigen taken verzenden, bewaken en beheren, maar geen Data Lake Analytics maken of verwijderen. | Ja | 
Gegevens ops purgeren | Kan analysegegevens opseen | Ja | 
DevTest Labs-gebruiker | Hiermee kunt u uw virtuele machines in uw virtuele machine verbinden, starten, opnieuw opstarten en afsluiten Azure DevTest Labs. | Ja | 
Inzender voor DNS-zone | Hiermee kunt u DNS-zones en recordsets beheren in Azure DNS, maar kunt u niet beheren wie er toegang toe heeft. | Ja | 
Inzender voor DocumentDB-account | Kan uw Azure Cosmos DB beheren. Azure Cosmos DB staat voorheen bekend als DocumentDB. | Ja | 
EventGrid EventSubscription Contributor | Hiermee kunt u gebeurtenisabonnementbewerkingen voor EventGrid beheren. | Ja | 
EventGrid EventSubscription Reader | Hiermee kunt u EventGrid-gebeurtenisabonnementen lezen. | Nee | 
HDInsight-clusteroperator | Hiermee kunt u HDInsight-clusterconfiguraties lezen en wijzigen. | Ja | 
Inzender voor HDInsight Domain Services | Kan domain services-gerelateerde bewerkingen lezen, maken, wijzigen en verwijderen die nodig zijn voor HDInsight-Enterprise Security Package | Ja | 
Inzender voor Intelligent Systems-account | Hiermee kunt u Intelligent Systems-accounts beheren, maar geen toegang tot deze accounts. | Ja | 
Key Vault-inzender | Hiermee kunt u sleutelkluizen beheren, maar geen toegang tot deze kluizen. | Ja | 
Labmaker | Hiermee kunt u uw beheerde labs maken, beheren en verwijderen onder uw Azure Lab-accounts. | Ja | 
Inzender van Log Analytics | Log Analytics-inzender kan alle bewakingsgegevens lezen en bewakingsinstellingen bewerken. Het bewerken van bewakingsinstellingen omvat het toevoegen van de VM-extensie aan VM's; opslagaccountsleutels lezen om het verzamelen van logboeken van de Azure Storage; Automation-accounts maken en configureren; oplossingen toevoegen; en azure diagnostics configureren voor alle Azure-resources. | Ja | 
Lezer van Log Analytics | De Log Analytics-lezer kan alle bewakingsgegevens bekijken en doorzoeken, evenals bewakingsinstellingen, waaronder het weergeven van de configuratie van diagnostische Azure-gegevens op alle Azure-resources. | Nee | 
Inzender voor logische apps | Hiermee kunt u logische apps beheren, maar de toegang tot deze apps niet wijzigen. | Ja | 
Logische app-operator | Hiermee kunt u logische apps lezen, inschakelen en uitschakelen, maar niet bewerken of bijwerken. | Ja | 
Operatorrol voor beheerde toepassingen | Hiermee kunt u acties lezen en uitvoeren op resources van beheerde toepassingen | Ja | 
Lezer voor beheerde toepassingen | Hiermee kunt u resources in een beheerde app lezen en JIT-toegang aanvragen. | Nee | 
Inzender voor beheerde identiteit | Door de gebruiker toegewezen identiteit maken, lezen, bijwerken en verwijderen | Ja | 
Operator voor beheerde identiteit | Door de gebruiker toegewezen identiteit lezen en toewijzen | Ja | 
Inzender voor beheergroep | Rol inzender beheergroep | Ja | 
Lezer beheergroep | Rol van lezer van beheergroep | Nee | 
Controlebijdrager | Kan alle bewakingsgegevens lezen en bewakingsinstellingen bewerken. Zie ook Aan de slag met rollen, machtigingen en beveiliging met Azure Monitor. | Ja | 
Bewaking van metrische Publisher | Hiermee kunt u metrische gegevens publiceren op Basis van Azure-resources | Ja | 
Lezer voor bewaking | Kan alle bewakingsgegevens (metrische gegevens, logboeken, enzovoort) lezen. Zie ook Aan de slag met rollen, machtigingen en beveiliging met Azure Monitor. | Nee | 
Inzender voor netwerken | Hiermee kunt u netwerken beheren, maar geen toegang tot deze netwerken. | Ja | 
New Relic APM-account inzender | Hiermee kunt u New Relic Application Performance Management accounts en toepassingen beheren, maar geen toegang tot deze accounts. | Ja | 
Lezer en gegevenstoegang | Hiermee kunt u alles bekijken, maar u kunt geen opslagaccount of ingesloten resource verwijderen of maken. Het biedt ook lees-/schrijftoegang tot alle gegevens in een opslagaccount via toegang tot opslagaccountsleutels. | Ja | 
Redis Cache-inzender | Hiermee kunt u Redis-caches beheren, maar geen toegang tot deze caches. | Ja | 
Inzender voor resourcebeleid (preview) | (Preview) Backfilled gebruikers van EA, met rechten voor het maken/wijzigen van resourcebeleid, het maken van een ondersteuningsticket en het lezen van resources/hiërarchie. | Ja | 
Inzender voor Scheduler-taakverzamelingen | Hiermee kunt u Scheduler-taakverzamelingen beheren, maar geen toegang tot deze verzamelingen. | Ja | 
Inzender voor zoekservice | Hiermee kunt u zoekservices beheren, maar geen toegang tot deze services. | Ja | 
Beveiligingsbeheerder | Alleen Security Center: Kan beveiligingsbeleid weergeven, beveiligingsbeleid weergeven, beveiligingsbeleid bewerken, waarschuwingen en aanbevelingen weergeven, waarschuwingen en aanbevelingen weg | Ja | 
Security Manager (verouderd) | Dit is een verouderde rol. Gebruik in plaats daarvan Beveiligingsbeheerder | Ja | 
Beveiligingslezer | Alleen Security Center: Kan aanbevelingen en waarschuwingen bekijken, beveiligingsbeleid weergeven, beveiligingswaarschuwingen bekijken, maar geen wijzigingen aanbrengen | Nee | 
Site Recovery-inzender | Hiermee kunt u een Site Recovery beheren, behalve het maken van een kluis en het toewijzing van rollen | Ja | 
Site Recovery-operator | Hiermee kunt u failover en failback uitvoeren, maar geen andere Site Recovery uitvoeren | Ja | 
Site Recovery-lezer | Hiermee kunt u de Site Recovery weergeven, maar geen andere beheerbewerkingen uitvoeren | Nee | 
Spatial Anchors-account inzender | Hiermee kunt u spatial anchors in uw account beheren, maar niet verwijderen | Ja | 
Spatial Anchors accounteigenaar | Hiermee kunt u ruimtelijke ankers in uw account beheren, inclusief het verwijderen ervan | Ja | 
Spatial Anchors-accountlezer | Hiermee kunt u eigenschappen van ruimtelijke ankers in uw account zoeken en lezen | Nee | 
SQL Inzender voor db | Hiermee kunt u SQL databases beheren, maar geen toegang tot deze databases. U kunt ook hun beveiligingsbeleid of hun bovenliggende serverservers SQL beheren. | Ja | 
SQL Inzender voor beheerd exemplaar | Hiermee kunt u SQL beheerde exemplaren en de vereiste netwerkconfiguratie beheren, maar u kunt geen toegang verlenen aan anderen. | Ja | 
SQL-beveiligingsbeheerder | Hiermee kunt u het beveiligingsbeleid van SQL servers en databases beheren, maar geen toegang tot deze servers. | Ja | 
SQL Server Inzender | Hiermee kunt u SQL servers en databases beheren, maar geen toegang krijgen tot deze servers en niet het bijbehorende beveiligingsbeleid. | Ja | 
Inzender voor opslagaccounts | Staat beheer van opslagaccounts toe. Biedt toegang tot de accountsleutel, die kan worden gebruikt voor toegang tot gegevens via gedeelde sleutelautorisatie. | Ja | 
Storage Servicerol accountsleuteloperator | Maakt het mogelijk om toegangssleutels voor opslagaccounts weer te geven en opnieuw te gebruiken. | Ja | 
Inzender voor Storage Blob-gegevens | Lees, schrijf en verwijder Azure Storage containers en blobs. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Ja | 
Eigenaar van opslagblobgegevens | Biedt volledige toegang tot Azure Storage blobcontainers en -gegevens, waaronder het toewijzen van POSIX-toegangsbeheer. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Ja | 
Lezer voor opslagblobgegevens | Lees en vermeld Azure Storage containers en blobs. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Nee | 
Storage Blob-delegator | Haal een sleutel voor gebruikersdelegatie op, die vervolgens kan worden gebruikt om een Shared Access Signature te maken voor een container of blob die is ondertekend met Azure AD-referenties. Zie Create a user delegation SAS (Een SAS voor gebruikersdelegatie maken) voor meer informatie. | Ja | 
Inzender voor opslagbestandsgegevens via SMB-share | Hiermee kunt u lezen, schrijven en verwijderen van toegang in Azure Storage via SMB | Ja | 
Inzender met verhoogde bevoegdheden voor opslagbestandsgegevens via SMB-share | Staat toegang tot NTFS-machtigingen voor lezen, schrijven, verwijderen en wijzigen toe in Azure Storage via SMB | Ja | 
Lezer voor opslagbestandgegevens via SMB-share | Staat leestoegang tot Azure-bestands delen via SMB toe | Nee | 
Storage Inzender voor wachtrijgegevens | Lees, schrijf en verwijder Azure Storage wachtrijen en wachtrijberichten. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Ja | 
Storage Wachtrijgegevensberichtprocessor | Een bericht bekijken, ophalen en verwijderen uit een Azure Storage wachtrij. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Ja | 
Storage Afzender van wachtrijgegevensbericht | Berichten toevoegen aan een Azure Storage wachtrij. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Ja | 
Storage Lezer van wachtrijgegevens | Lees en vermeld Azure Storage wachtrijen en wachtrijberichten. Zie Machtigingen voor het aanroepen van blob- en wachtrijgegevensbewerkingen voor meer informatie over welke acties vereist zijn voor een bepaalde gegevensbewerking. | Nee | 
Inzender voor ondersteuningsaanvraag | Hiermee kunt u ondersteuningsaanvragen maken en beheren | Ja | 
Traffic Manager Inzender | Hiermee kunt u Traffic Manager beheren, maar kunt u niet bepalen wie er toegang toe heeft. | Ja | 
Beheerder van gebruikerstoegang | Hiermee kunt u gebruikerstoegang tot Azure-resources beheren. | Ja | 
Aanmeldgegevens van de beheerder van de virtuele machine | De Virtual Machines in de portal weergeven en u aanmelden als beheerder | Ja | 
Inzender voor virtuele machines | Hiermee kunt u virtuele machines beheren, maar geen toegang krijgen tot deze machines, en niet tot het virtuele netwerk of opslagaccount waarmee ze zijn verbonden. | Ja | 
Gebruikersmelding voor virtuele machine | Bekijk Virtual Machines in de portal en meld u aan als een gewone gebruiker. | Ja | 
Inzender voor webplannen | Hiermee kunt u de webplannen voor websites beheren, maar geen toegang tot de websites. | Ja | 
Inzender voor websites | Hiermee kunt u websites beheren (geen webplannen), maar geen toegang tot websites | Ja |

## <a name="next-steps"></a>Volgende stappen

- [Partnertegoed: een overzicht van hoe het werkt in de nieuwe commerce-ervaring in CSP](partner-earned-credit.md)

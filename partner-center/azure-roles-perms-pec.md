---
title: Rollen, machtigingen voor het tegoed van een partner
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over de rollen en machtigingen voor partners voor het verdienen van de door de partner aangehaalde tegoeden (PEC). Deze verschillen van functies die u kunt gebruiken in het partner centrum.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8c36883dc7d12b7ea0ce8f2644dbac86595ab131
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534587"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Rollen en machtigingen die zijn vereist voor het verdienen van het tegoed van de partner

De volgende rollen zijn gekoppeld aan de machtigings niveaus die bepalen of een partner in aanmerking komt voor het tegoed van de partner.

>[!Important]
>Deze rollen en machtigingen zijn niet hetzelfde als de rollen en machtigingen die een gebruiker nodig heeft om in het partner centrum te werken.

|**Role**   |**Beschrijving**   |**In aanmerking komende PEC**   |
|-----------------|:------------------|:--------------|
|Eigenaar  |U beheert alles, inclusief toegang tot resources.|Ja|
|Inzender |U beheert alles behalve het verlenen van toegang tot resources.|Ja|
|Lezer|U kunt alles weer geven, maar geen wijzigingen aanbrengen|Nee|
|ACRDelete|ACR verwijderen|Ja|
|ACRImageSigner|ACR-installatie kopie ondertekenaar|Ja|
|ACRPull|ACR pull|Ja|
|AcrPush|ACR-push|Ja|
|AcrQuarantineReader|ACR quarantaine gegevens lezer|Nee|
|AcrQuarantineWriter| ACR quarantaine gegevens schrijver|Ja|
|Inzender van API Management-service|Kan de service en de Api's beheren|Ja|
|Functie API Management service operator|Kan de service beheren, maar niet de Api's|Ja|
|API Management functie Service lezer|Alleen-lezen toegang tot de service en Api's|Nee|
|Inzender voor Application Insights onderdelen|Beheert Application Insights onderdelen|Ja|
|Application Insights Snapshot Debugger|Geeft gebruikers machtigingen voor het weer geven en downloaden van moment opnamen van fout opsporing die zijn verzameld met de Application Insights Snapshot Debugger. Houd er rekening mee dat deze machtigingen niet zijn opgenomen in de rollen eigenaar of Inzender.|Ja|
Automation-taak operator | Maak en beheer taken met behulp van Automation-Runbooks. | Ja | 
Automation-operator | Automatiserings operatoren kunnen taken starten, stoppen, onderbreken en hervatten | Ja | 
Automation-Runbook-operator | Runbook-eigenschappen lezen: om taken van het Runbook te kunnen maken. | Ja | 
AVERE-bijdrager | Kan een avere vFXT-cluster maken en beheren. | Ja | 
AVERE-operator | Wordt gebruikt door het avere vFXT-cluster voor het beheren van het cluster | Ja | 
Eigenaar van Azure Event Hubs-gegevens | Hiermee krijgt u volledige toegang tot Azure Event Hubs-resources. | Ja | 
Gegevens ontvanger van Azure Event Hubs | Hiermee krijgt u toegang tot Azure Event Hubs-resources. | Ja | 
Afzender van Azure Event Hubs gegevens | Hiermee wordt toegang tot Azure Event Hubs-resources verzonden. | Ja | 
Rol van Cluster beheerder voor Azure Kubernetes-service | Lijst met actie voor cluster beheer referenties. | Ja | 
Gebruikersrol Azure Kubernetes service-cluster | Geef een lijst actie voor de gebruikers referenties van het cluster op. | Ja | 
Azure Maps gegevens lezer (preview-versie) | Hiermee wordt toegang verleend om gerelateerde gegevens te lezen vanuit een Azure Maps-account. | Nee | 
Gegevens eigenaar Azure Service Bus | Hiermee krijgt u volledige toegang tot Azure Service Bus-resources. | Ja | 
Gegevens ontvanger Azure Service Bus | Hiermee krijgt u toegang tot Azure Service Bus-resources. | Ja | 
Afzender van Azure Service Bus gegevens | Hiermee kunt u toegang tot Azure Service Bus resources verzenden. | Ja | 
Registratie-eigenaar Azure Stack | Hiermee kunt u Azure Stack registraties beheren. | Ja | 
Back-upinzender | Hiermee kunt u de back-upservice beheren, maar geen kluizen maken en anderen toegang verlenen | Ja | 
Back-upoperator | Hiermee kunt u back-upservices beheren, behalve het verwijderen van back-ups, het maken van een kluis en het verlenen van toegang | Ja | 
Back-uplezer | Kan back-upservices weer geven, maar kan geen wijzigingen aanbrengen | Nee | 
Lezer voor facturering | Hiermee staat u lees toegang tot facturerings gegevens toe | Nee | 
BizTalk-bijdrager | Hiermee kunt u BizTalk Services beheren, maar niet de toegang tot de service. | Ja | 
Toegang tot Block Chain-leden knooppunt (preview-versie) | Hiermee wordt toegang tot Block Chain-leden knooppunten toegestaan | Ja | 
Blauwdrukinzender | Blauwdrukinzenders kunnen blauwdrukdefinities beheren, maar deze niet toewijzen. | Ja | 
Blauwdrukoperator | Kan bestaande gepubliceerde blauw drukken toewijzen, maar kan geen nieuwe blauw drukken maken. Opmerking: dit werkt alleen als de toewijzing wordt uitgevoerd met een door de gebruiker toegewezen beheerde identiteit. | Ja | 
Inzender voor CDN-eind punten | Kan CDN-eind punten beheren, maar kan geen toegang verlenen aan andere gebruikers. | Ja | 
CDN-eindpunt lezer | Kan CDN-eind punten weer geven, maar kan geen wijzigingen aanbrengen. | Nee | 
Inzender voor CDN-profiel | Kan CDN-profielen en de bijbehorende eind punten beheren, maar kan geen toegang verlenen aan andere gebruikers. | Ja | 
CDN-profiel lezer | Kan CDN-profielen en de bijbehorende eind punten weer geven, maar kan geen wijzigingen aanbrengen. | Nee | 
Inzender voor klassieke netwerken | Hiermee beheert u klassieke netwerken, maar hebt u geen toegang tot de netwerk bestanden. | Ja | 
Inzender voor klassieke opslag accounts | Hiermee kunt u klassieke opslag accounts beheren, maar niet de toegang tot de account. | Ja | 
Service functie voor de sleutel operator voor klassieke opslag accounts | De sleutel operators voor klassieke opslag accounts zijn toegestaan om sleutels weer te geven en opnieuw te genereren voor klassieke opslag. | Ja | 
Inzender voor klassieke virtuele machines | Hiermee beheert u klassieke virtuele machines, maar kunt u niet de toegang tot ze en niet het virtuele netwerk of opslag account waarmee ze zijn verbonden. | Ja | 
Inzender Cognitive Services | Hiermee kunt u sleutels van Cognitive Services maken, lezen, bijwerken, verwijderen en beheren. | Ja | 
Cognitive Services gegevens lezer (preview-versie) | Hiermee kunt u Cognitive Services gegevens lezen. | Nee | 
Cognitive Services gebruiker | Hiermee kunt u de sleutels van Cognitive Services lezen en weer geven. | Nee | 
Rol van Cosmos DB-account lezer | Kan gegevens van Azure Cosmos DB-account lezen. Zie DocumentDB account Inzender voor het beheren van Azure Cosmos DB accounts. | Nee | 
Cosmos DB-operator | Hiermee kunt u Azure Cosmos DB accounts beheren, maar geen toegang tot gegevens. Hiermee voor komt u toegang tot account sleutels en verbindings reeksen. | Ja | 
CosmosBackupOperator | Kan een terugzet aanvraag indienen voor een Cosmos DB-Data Base of een container voor een account | Ja | 
Inzender Cost Management | Kan kosten bekijken en kosten configuratie beheren (bijvoorbeeld budgetten, exports) | Ja | 
Cost Management lezer | Kan kosten gegevens en-configuratie weer geven (bijvoorbeeld budgetten, exports) | Nee | 
Inzender Data Box | Hiermee kunt u alles beheren onder Data Box Service, behalve dat anderen toegang verlenen. | Ja | 
Data Box lezer | Met kunt u de Data Box-Service beheren, met uitzonde ring van order gegevens maken of bewerken en anderen toegang verlenen. | Nee | 
Inzender Data Factory | Het maken en beheren van gegevens fabrieken, evenals onderliggende resources. | Ja | 
Data Lake Analytics-ontwikkelaar | Hiermee kunt u uw eigen taken verzenden, bewaken en beheren, maar geen Data Lake Analytics accounts maken of verwijderen. | Ja | 
Gegevens opschoner | Kan Analytics-gegevens verwijderen | Ja | 
DevTest Labs-gebruiker | Met kunt u verbinding maken met uw virtuele machines in uw Azure DevTest Labs, deze starten, opnieuw opstarten en afsluiten. | Ja | 
Inzender DNS-zone | Met kunt u DNS-zones en-record sets beheren in Azure DNS, maar kunt u niet bepalen wie toegang heeft tot de groepen. | Ja | 
Inzender voor DocumentDB-accounts | Kan Azure Cosmos DB accounts beheren. Azure Cosmos DB is voorheen bekend als DocumentDB. | Ja | 
EventGrid EventSubscription-bijdrager | Hiermee kunt u bewerkingen voor EventGrid-gebeurtenis abonnementen beheren. | Ja | 
EventGrid EventSubscription-lezer | Hiermee kunt u EventGrid-gebeurtenis abonnementen lezen. | Nee | 
HDInsight-cluster operator | Hiermee kunt u HDInsight-cluster configuraties lezen en wijzigen. | Ja | 
Inzender voor HDInsight Domain Services | Kan gerelateerde bewerkingen die betrekking hebben op domein services lezen, maken, wijzigen en verwijderen die nodig zijn voor HDInsight-Enterprise Security Package | Ja | 
Inzender voor Intelligent Systems-account | Hiermee kunt u intelligente Systems-accounts beheren, maar niet de toegang tot ze. | Ja | 
Inzender Key Vault | Hiermee kunt u sleutel kluizen beheren, maar niet de toegang tot de kluis. | Ja | 
Lab-Maker | Met kunt u uw beheerde Labs maken, beheren en verwijderen in uw Azure Lab-accounts. | Ja | 
Inzender van Log Analytics | Log Analytics Inzender kan alle bewakings gegevens lezen en controle-instellingen bewerken. Het bewerken van bewakings instellingen omvat het toevoegen van de VM-extensie aan Vm's; lezen van opslag account sleutels om het verzamelen van logboeken van Azure Storage te kunnen configureren. Automation-accounts maken en configureren; oplossingen toevoegen; en het configureren van Azure Diagnostics voor alle Azure-resources. | Ja | 
Lezer van Log Analytics | Log Analytics Reader kan alle bewakings gegevens weer geven en doorzoeken en controle-instellingen weer geven, inclusief het weer geven van de configuratie van Azure Diagnostics op alle Azure-resources. | Nee | 
Inzender voor logische apps | Hiermee kunt u logische apps beheren, maar niet wijzigen. | Ja | 
Logische app-operator | Hiermee kunt u logische apps lezen, inschakelen en uitschakelen, maar niet bewerken of bijwerken. | Ja | 
Rol beheerde toepassings operator | Hiermee kunt u acties voor beheerde toepassings bronnen lezen en uitvoeren | Ja | 
Lezer voor beheerde toepassingen | Hiermee kunt u bronnen in een beheerde app lezen en JIT-toegang aanvragen. | Nee | 
Inzender beheerde identiteit | Aan de gebruiker toegewezen identiteit maken, lezen, bijwerken en verwijderen | Ja | 
Beheerde identiteits operator | Door gebruiker toegewezen identiteit lezen en toewijzen | Ja | 
Inzender beheer groep | Rol Inzender beheer groep | Ja | 
Lezer beheer groep | Rol van lezer van beheer groep | Nee | 
Inzender bewaken | Kan alle bewakings gegevens lezen en controle-instellingen bewerken. Zie ook aan de slag met rollen, machtigingen en beveiliging met Azure Monitor. | Ja | 
De uitgever van metrische gegevens controleren | Hiermee schakelt u de metrische gegevens voor publicatie in op Azure-resources | Ja | 
Bewakings lezer | Kan alle bewakings gegevens (metrieken, logboeken, enzovoort) lezen. Zie ook aan de slag met rollen, machtigingen en beveiliging met Azure Monitor. | Nee | 
Inzender voor netwerken | Hiermee kunt u netwerken beheren, maar niet de toegang tot de netwerk bestanden. | Ja | 
Nieuwe Inzender voor Relic APM-account | Hiermee kunt u New Relic Application Performance Management accounts en-toepassingen beheren, maar niet de toegang tot ze. | Ja | 
Lezer en gegevens toegang | Hiermee kunt u alles weer geven, maar kunt u geen opslag account of opgenomen resource verwijderen of maken. Ook wordt lees-/schrijftoegang tot alle gegevens in een opslag account toegestaan via toegang tot de sleutel van het opslag account. | Ja | 
Inzender Redis Cache | Hiermee kunt u redis-caches beheren, maar niet de toegang tot deze bestanden. | Ja | 
Inzender voor resource beleid (preview-versie) | Evaluatie Alsnog gebruikers van EA, met rechten voor het maken/wijzigen van het resource beleid, het maken van een ondersteunings ticket en het lezen van resources/hiërarchie. | Ja | 
Inzender voor scheduler-taak verzamelingen | Hiermee kunt u scheduler-taak verzamelingen beheren, maar niet de toegang tot deze taken. | Ja | 
Inzender Search Service | Hiermee kunt u zoek services beheren, maar niet de toegang tot ze. | Ja | 
Beveiligingsbeheerder | In Security Center: kan beveiligings beleid weer geven, beveiligings status weer geven, beveiligings beleid bewerken, waarschuwingen en aanbevelingen weer geven, waarschuwingen en aanbevelingen negeren | Ja | 
Beveiligings beheer (verouderd) | Dit is een verouderde rol. Gebruik in plaats daarvan beveiligings beheerder | Ja | 
Beveiligingslezer | In Security Center: kunt u aanbevelingen en waarschuwingen weer geven, beveiligings beleid weer geven, beveiligings status weer geven, maar geen wijzigingen aanbrengen | Nee | 
Site Recovery-inzender | Hiermee kunt u Site Recovery-service beheren, behalve het maken van een kluis en roltoewijzing | Ja | 
Site Recovery-operator | Een failover en failback, maar geen andere Site Recovery beheer bewerkingen uitvoeren | Ja | 
Site Recovery-lezer | Hiermee kunt u de Site Recovery status weer geven, maar geen andere beheer bewerkingen uitvoeren | Nee | 
Inzender voor ruimtelijke ankers | Hiermee kunt u ruimtelijke ankers in uw account beheren, maar niet verwijderen | Ja | 
Eigenaar van ruimtelijk ankers | Hiermee kunt u ruimtelijke ankers in uw account beheren, met inbegrip van het verwijderen ervan | Ja | 
Lezer van ruimtelijk ankers-account | Hiermee kunt u eigenschappen van ruimtelijke ankers in uw account zoeken en lezen | Nee | 
Inzender voor SQL-data base | Hiermee kunt u SQL-data bases beheren, maar niet de toegang tot ze. U kunt ook hun beveiligings beleid of de bovenliggende SQL-servers niet beheren. | Ja | 
Inzender voor SQL Managed instance | Hiermee beheert u beheerde SQL-instanties en de vereiste netwerk configuratie, maar kunt u geen toegang verlenen aan anderen. | Ja | 
SQL-beveiligingsbeheerder | Hiermee kunt u het beveiligings beleid van SQL-servers en-data bases beheren, maar niet de toegang tot de services. | Ja | 
Inzender SQL Server | Hiermee kunt u SQL-servers en-data bases beheren, maar niet de toegang tot ze en niet het beveiligings beleid. | Ja | 
Inzender voor opslagaccounts | Hiermee staat u het beheer van opslag accounts toe. Biedt toegang tot de account sleutel, die kan worden gebruikt om toegang te krijgen tot gegevens via een gedeelde sleutel autorisatie. | Ja | 
Functie Service-sleutel operator van opslag account | Kan de toegangs sleutels voor het opslag account weer geven en opnieuw genereren. | Ja | 
Inzender voor Storage Blob-gegevens | Azure Storage containers en blobs lezen, schrijven en verwijderen. Zie machtigingen voor het aanroepen van BLOB-en wachtrij gegevens voor meer informatie over welke acties vereist zijn voor een bepaalde gegevens bewerking. | Ja | 
Eigenaar van opslagblobgegevens | Biedt volledige toegang tot Azure Storage BLOB-containers en-gegevens, met inbegrip van het toewijzen van POSIX-toegangs beheer. Zie machtigingen voor het aanroepen van BLOB-en wachtrij gegevens voor meer informatie over welke acties vereist zijn voor een bepaalde gegevens bewerking. | Ja | 
Lezer voor opslagblobgegevens | Azure Storage containers en blobs lezen en weer geven. Zie machtigingen voor het aanroepen van BLOB-en wachtrij gegevens voor meer informatie over welke acties vereist zijn voor een bepaalde gegevens bewerking. | Nee | 
Delegering van opslag-BLOB | Een sleutel voor gebruikers overdracht ophalen, die vervolgens kan worden gebruikt om een gedeelde toegangs handtekening te maken voor een container of BLOB die is ondertekend met Azure AD-referenties. Zie een gebruiker delegering SA'S maken voor meer informatie. | Ja | 
Inzender voor opslagbestandsgegevens via SMB-share | Hiermee wordt lees-, schrijf-en verwijder toegang in Azure Storage bestands shares via SMB toegestaan | Ja | 
Inzender met verhoogde bevoegdheden voor opslagbestandsgegevens via SMB-share | Hiermee wordt toegang tot NTFS-machtigingen voor lezen, schrijven, verwijderen en wijzigen in Azure Storage bestands shares via SMB toegestaan | Ja | 
Lezer voor opslagbestandgegevens via SMB-share | Hiermee wordt lees toegang tot Azure file share via SMB toegestaan | Nee | 
Inzender voor opslag wachtrij gegevens | Lees-, schrijf-en verwijder Azure Storage-wacht rijen en-wachtrij berichten. Zie machtigingen voor het aanroepen van BLOB-en wachtrij gegevens voor meer informatie over welke acties vereist zijn voor een bepaalde gegevens bewerking. | Ja | 
Processor voor gegevens berichten van de opslag wachtrij | Een bericht uit een Azure Storage wachtrij bekijken, ophalen en verwijderen. Zie machtigingen voor het aanroepen van BLOB-en wachtrij gegevens voor meer informatie over welke acties vereist zijn voor een bepaalde gegevens bewerking. | Ja | 
Afzender gegevens bericht van opslag wachtrij | Berichten toevoegen aan een Azure Storage wachtrij. Zie machtigingen voor het aanroepen van BLOB-en wachtrij gegevens voor meer informatie over welke acties vereist zijn voor een bepaalde gegevens bewerking. | Ja | 
Gegevens lezer van de opslag wachtrij | Azure Storage-wacht rijen en-wachtrij berichten lezen en weer geven. Zie machtigingen voor het aanroepen van BLOB-en wachtrij gegevens voor meer informatie over welke acties vereist zijn voor een bepaalde gegevens bewerking. | Nee | 
Inzender voor ondersteunings aanvragen | Hiermee kunt u ondersteunings aanvragen maken en beheren | Ja | 
Inzender Traffic Manager | Hiermee beheert u Traffic Manager profielen, maar kunt u niet bepalen wie er toegang tot heeft. | Ja | 
Beheerder van gebruikerstoegang | Hiermee beheert u de gebruikers toegang tot Azure-resources. | Ja | 
Aanmelding voor de beheerder van de virtuele machine | Virtual Machines in de portal weer geven en u aanmelden als beheerder | Ja | 
Inzender voor virtuele machines | Met kunt u virtuele machines beheren, maar niet de toegang tot ze en niet het virtuele netwerk of opslag account waarmee ze zijn verbonden. | Ja | 
Gebruikers aanmelding voor de virtuele machine | Bekijk Virtual Machines in de portal en meld u aan als een gewone gebruiker. | Ja | 
Inzender voor webabonnementen | Hiermee kunt u de Webabonnementen voor websites beheren, maar niet de toegang tot de abonnementen. | Ja | 
Website bijdrager | Hiermee beheert u websites (geen Webabonnementen), maar hebt u geen toegang tot ze | Ja |

## <a name="next-steps"></a>Volgende stappen

- [Tegoed van de partner: een overzicht van hoe het werkt in de nieuwe Commerce-ervaring in CSP](partner-earned-credit.md)

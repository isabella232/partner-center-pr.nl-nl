---
title: Gedeelde Azure-partner services toevoegen
description: Gebruik gedeelde services van Azure-partners voor het kopen van Azure-abonnementen voor eigen gebruik en voor een uniforme methode om Azure te kopen, bij te houden en te beheren.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 756fbfda3438933b50fc51936b396291986472a7
ms.sourcegitcommit: ec33c2352a9dd3e5a941f0f42ff1e8d256bb2399
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/24/2021
ms.locfileid: "105028278"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Voeg Shared Services van Azure-partners toe zodat partners Azure-abonnementen kunnen kopen voor hun eigen gebruik

**Juiste rollen**

- Globale beheerder
- Beheer agent
- Verkoop agent

Azure partner Shared Services is een nieuw aanbiedings type voor partners in het CSP-programma, waardoor partners Azure-abonnementen kunnen kopen voor eigen gebruik.Hiermee maakt u de kans dat partners een uniforme methode gebruiken voor het kopen, bijhouden en beheren van Azure, naast de mogelijkheid om hun Azure-licenties samen te voegen en overeenkomsten te verkopen met micro soft. Met gedeelde Azure-partners hebben partners nu dezelfde flexibiliteit voor het gebruik van Azure-abonnementen in CSP als in de Program ma's van micro soft Enterprise Overeenkomst en Web direct, scenario's voor het openen van ontwikkel-en test omgevingen, het implementeren van interne workloads en het hosten van gedeelde services of multi tenant-toepassingen.  

## <a name="create-the-shared-services-tenant"></a>De Shared Services-Tenant maken

1. Ga naar **instellingen**  >  **account instellingen**  >  **gedeelde services**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Account instellingen > gedeelde services":::

2. Als u nog geen Shared Services-Tenant hebt, klikt u op **gedeelde services maken**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Gedeelde services maken":::

3. Hiermee maakt u een Tenant voor gedeelde services en wordt het Azure CSP Shared Services-abonnement gekocht om te worden gebruikt voor gedeelde resources en interne werk belasting.

   :::image type="content" source="images/sharedservices5.png" alt-text="De Tenant maken en het abonnement aanschaffen":::

## <a name="about-the-azure--internalshared-services-offer"></a>Over de Azure-Interne/gedeelde services aanbieding

- Het Azure-Interne/gedeelde services-abonnement is een nieuw Azure-aanbiedings type in CSP die toegankelijk is via het partner centrum waarmee partners hun eigen gebruik van Azure kunnen verkrijgen.

- Azure partner Shared Services-abonnementen komen in aanmerking en kunnen worden gebruikt om RIs aan te schaffen.

- De aanbieding Azure-Interne/gedeelde services kan alleen worden toegepast op de Shared Services-Tenant.

- Het primaire gebruik voor het Azure-Interne/gedeelde services-abonnement is dat u Azure kunt gebruiken voor uw eigen ontwikkelings doeleinden. De gedeelde Tenant die u gebruikt voor het inrichten van deze aanbieding kan niet worden gebruikt voor andere services, zoals Office 365-of Dynamics-licenties.

- U kunt het abonnement annuleren zoals elk ander abonnement. Ga naar de **instellingen**  >  **alle instellingen**  >  **gedeelde services** weer geven. Selecteer het Azure-Interne/gedeelde services-abonnement en Annuleer het.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Details van het gebruik van gedeelde Azure-partner services

U vindt het Azure-verbruik op uw CSP-factuur en het afstemmings bestand. Het wordt opgenomen als onderdeel van Microsoft Azure regel item in de factuur. De gedetailleerde informatie over verbruik is beschikbaar in het afstemmings bestand dat is geregistreerd bij de Tenant die voor deze aanbieding is gemaakt.

## <a name="azure-partner-shared-services-pricing"></a>Prijzen van Azure partner Shared Services

Als u het nieuwe prijs bestand voor gedeelde Azure partner-services wilt bekijken, gaat u naar **verkoop**  >  **prijzen en aanbiedingen** en selecteert u de prijs lijst van de huidige maand. In de komende weken wordt er ook een specifieke tarieven-API uitgebracht.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Marketplace-aanbiedingen en gedeelde Azure partner-services

Vanaf 1 maart 2019 biedt Azure partner Shared Services (APSS) geen ondersteuning meer voor Marketplace-aanbiedingen.

|**Marketplace-ondersteuning**   |**APSS ondersteund vóór 1 maart 2019**|**Na 1 maart 2019**|
|---------------------------|:----------------------------|:-------------------|
|Bring Your Own License (BYOL) en gratis services   | Ja   | Nee|
|Andere Marketplace-aanbiedingen van derden   | Nee   |Nee|

Partners met BYOL of gratis services die zijn geïmplementeerd met APSS, worden niet beïnvloed. na 1 maart 2019 kunnen ze echter geen nieuwe BYOL of gratis services kopen.

Als u gebruik wilt maken van de volledige catalogus met Marketplace-aanbiedingen die beschikbaar zijn (niet alleen BYOL en gratis services), raden wij u aan CSP-partners gedeelde services te implementeren met behulp van web direct Azure-abonnementen.  CSP-partners die eerder BYOL en gratis service bronnen van derden van de Marketplace hebben geïmplementeerd en willen blijven gebruiken en meer aanbiedingen van derden kunnen implementeren, worden aanbevolen om het APSS-abonnement te migreren naar web direct om [bestaande Azure-abonnementen te migreren](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Partners, die van plan zijn APSS-abonnement te blijven gebruiken na 1 maart 2019 en nieuwe [BYOL-Services](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) van derden of gratis services willen implementeren, kunnen de instructies van isv's volgen om deze te implementeren in hun APSS-abonnementen.

## <a name="next-steps"></a>Volgende stappen

- [Software-abonnementen verkopen via CSP](csp-software-subscriptions.md)
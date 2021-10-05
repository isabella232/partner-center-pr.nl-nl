---
title: Nieuwe commerce telco betalen per u
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over nieuwe commerce-ervaringen voor het kopen van aanbiedingen die uitval van betalen per uur mogelijk maken.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8265cb3ce77183c4919e9b8e4e028bb66e8cd2f7
ms.sourcegitcommit: 462d6026287b85c9feea602af5bcdf924f3e6976
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/05/2021
ms.locfileid: "129452493"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Inleiding: Nieuwe commerce-uitval voor telco betalen per uur

**Juiste rollen**

- Beheeragent
- Verkoopagent
- Globale beheerder

> [!NOTE]
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technische preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Sommige op licenties gebaseerde producten omvatten services met toegewezen aanroepplannen die doorgaans een toewijzing per licentie voor minuten per maand bevatten, meestal 120 per licentie. 

In traditionele partnerscenario's op basis van licenties was er geen manier om servicegebruik buiten de maandelijkse limieten in te stellen. Klanten die meer dan 120 minuten nodig hebben om communicatietegoeden te kopen, of *comm-tegoed* zelf rechtstreeks van Microsoft.  Deze communicatietegoeden zijn niet aangeboden in Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Met behulp van nieuwe commerce telco betalen per gebruik

Deze beperking is verholpen in nieuwe handel waardoor de partner uitvalmogelijkheden kan inschakelen voor services die dit toestaan. Partners kunnen aanbiedingen kopen die uitvalmogelijkheden bevatten. Deze aanbiedingen worden geïdentificeerd in de kolom met tags voor prijslijst die *IncludeOverage bevat.* De catalogus-SKU bevat ook een eigenschap om te bepalen of de SKU de mogelijkheid tot uitval ondersteunt. Partners kopen gewoon de aanbiedingen aan en het systeem configureert een uitvalabonnement dat geen kosten bevat en alleen factureert wanneer de gebruikers van de klant de toegewezen maandelijkse belminuten die bij de aangeschafte aanbieding worden ontvangen, over het bestek heen zien. 

Partners kunnen bepalen welke product-SKU's uitvalmogelijkheden bevatten door 

- Product-SKU's voor partnercentrumcatalogus weergeven
- De nieuwe lijst met commerceprijzen filteren op **includesOverage** in de kolom tags

Partners die producten met uitval aanschaffen, maken dit mogelijk door de pagina Uitval beheren **op** de pagina Abonnementen beheren te openen. De interface voor het beheren van uitval stelt de partner in staat om te activeren en toe te wijzen aan welk Azure-abonnement de uitvalkosten zullen stromen. De partner kan uitval op elk moment uitschakelen door het verbruiksabonnement toe te wijzen aan *Geen.* 

Partners wijzen uitval toe of schakelen deze uit met de *functie Uitval* beheren in de lijst met abonnementen. Dit is alleen toegankelijk als de partner abonnementen heeft die uitval inschakelen. Maandelijkse uitvalkosten worden opgeteld bij het toegewezen abonnement en worden geïdentificeerd in het afstemmingsbestand van partners. Partners kunnen het uitvalgebruik bijhouden door de mogelijkheden van Azure Cost Management in de Azure Portal. 

Partners kunnen het uitvalgebruik traceren door naar de Azure Portal en de mogelijkheden en functies voor kostenbeheer te gebruiken. 

## <a name="important-details-about-overage"></a>Belangrijke informatie over uitval

- Als u een product-SKU op basis van licenties aanschaft met uitvalmogelijkheden, wordt alleen het product op basis van licenties gekocht. Partners moeten na aankoop nog een stap nemen om uitval in te zetten door naar de pagina abonnementsbeheer te gaan en op Uitval **beheren te klikken**
- Alleen beheerdersagenten voor de transacting partner kunnen uitval inschakelen na de aankoop op basis van licenties. 
- Als u uitval inschakelen, maakt u een gratis Azure-abonnement en een bijbehorend standaard Azure-abonnement **abonnement 1** specifiek voor uitvalverbruik. Als het Azure-plan al bestaat, maakt het inschakelen van uitval het nieuwe abonnement onder het bestaande Azure-plan. Partners kunnen uitval altijd weergeven of opnieuw toewijzen aan andere abonnementen in **De uitval beheren.** Klanten die nog geen Azure-abonnement (oudere Azure) hebben, moeten overstappen naar een Azure-plan voordat ze uitval kunnen inschakelen.

De toewijzing van uitval wordt bepaald door *de eerste in de* regel. Als een partner E5 koopt met aanroepabonnementen voor een nieuwe klant, wordt er uitval toegewezen aan het verbruiksabonnement van deze partner. Als een tweede partner een ander exemplaar van E5 koopt met aanroepplannen, respecteert het systeem de aankoop en toewijzing van de eerste partner. Partners kunnen *uitval altijd beheren vanaf* de pagina abonnementen om deze uit te schakelen of uit te schakelen door uitval toe te wijzen aan *Geen.*

Uitvalinstellingen zijn per service per klant. Er kan slechts één uitvalabonnement tegelijk worden toegewezen. Als uitval moet worden gewijzigd van de ene partner in de andere, moeten de drie betrokken partijen eerst akkoord gaan. Zodra de klant akkoord gaat, kan de bestaande partner gewoon uitval instellen op *Geen,* zodat de andere partner uitval kan instellen op zijn of haar abonnement.

## <a name="telco-pay-as-you-go-apis"></a>Telco-API's voor betalen per uur

- [SKU-eigenschappen](/partner-center/develop/product-resources#sku) bevatten een *eigenschap consumptionType* om de partner te helpen bepalen of een SKU uitval mogelijk maakt
- [Krijg uitval](/partner-center/develop/get-subscription-overage) om te begrijpen of er momenteel uitval is ingesteld voor uw klant
- [Uitval bijwerken om](/partner-center/develop/update-subscription-overage) de uitval van de klant bij te werken naar een Azure-abonnement of om deze in te stellen op *Geen*

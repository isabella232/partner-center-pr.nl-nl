---
title: New commerce telco pay as you go
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over nieuwe commerce-ervaringen voor het kopen van aanbiedingen waarmee u kunt betalen wanneer u over de uitval gaat.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b7f3fa6ce3b92e7b182192290f5ebb4ee167ff7a
ms.sourcegitcommit: 847ad384d44a5a673791cb2950af02225d8174c9
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/16/2021
ms.locfileid: "127876744"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Inleiding: Nieuwe commerce-uitval voor betalen per telco

**Juiste rollen**

- Beheeragent
- Verkoopagent
- Globale beheerder

> [!NOTE]
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van de technische preview van Microsoft 365/Dynamics 365 New Commerce Experience.

Sommige op licenties gebaseerde producten omvatten services met toegewezen aanroepplannen. Deze aanroepende abonnementen worden doorgaans met een toewijzing per licentie voor minuten per maand, meestal 120 per licentie.

In traditionele partnerscenario's op basis van licenties was er geen manier om servicegebruik buiten de maandelijkse limieten in te stellen. Klanten die meer dan 120 minuten nodig hebben om communicatietegoeden te kopen, of *comm-tegoed* zelf rechtstreeks van Microsoft.  Deze communicatietegoeden zijn niet aangeboden in Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Gebruik van nieuwe commerce telco betalen per gebruik ##

Deze beperking is verholpen in nieuwe handel waardoor de partner uitvalmogelijkheden kan inschakelen voor services die dit toestaan. Partners kunnen aanbiedingen kopen die uitvalmogelijkheden bevatten. Deze aanbiedingen worden in de kolom met prijslijsttags aangeduid met *IncludeOverage*. De catalogus-SKU bevat ook een eigenschap om te bepalen of de SKU de mogelijkheid tot uitval ondersteunt. Partners kopen gewoon de aanbiedingen en het systeem configureert en besturingssysteemabonnementen die geen kosten hebben en worden alleen gefactureerd wanneer de gebruikers van de klant de toegewezen maandelijkse belminuten die bij de aangeschafte aanbieding worden ontvangen, over het bestek heen zien.

Partners kunnen het uitvalgebruik traceren door naar de Azure Portal en de mogelijkheden en functies voor kostenbeheer te gebruiken. Partners hebben ook de mogelijkheid om de  uitval op elk moment in te stellen op Geen als ze uitval op elk moment willen uitschakelen of uitschakelen.

Partners kunnen bepalen welke producten uitvalmogelijkheden bevatten door de product-SKU's van de partnercentrumcatalogus te bekijken. 

Partners die producten met uitval aanschaffen, maken de uitval mogelijk door toegang te krijgen tot *de* pagina Uitval beheren op de pagina Abonnementen beheren. Hierdoor kan de partner uitval activeren en het gewenste verbruiksabonnement toewijzen waar de uitvalkosten naar zullen stromen. De partner kan uitval op elk moment uitschakelen door het verbruiksabonnement toe te wijzen aan *Geen.*

Partners wijzen uitval toe of schakelen deze uit met de *functie Uitval* beheren in de lijst met abonnementen. Dit is alleen toegankelijk als de partner abonnementen heeft die uitval inschakelen. Maandelijkse uitvalkosten worden opgeteld bij het toegewezen abonnement en worden geïdentificeerd in het afstemmingsbestand van partners. Partners kunnen het uitvalgebruik bijhouden door de mogelijkheden van Azure Cost Management in de Azure Portal. 

## <a name="important-details-about-overage"></a>Belangrijke informatie over uitval ##

Als u een product-SKU aanschaft die uitval mogelijk maakt, zorgt u er automatisch voor dat de klant van de partner is ingesteld voor uitval. Dit omvat het maken van een gratis Azure-abonnement, een gekoppeld standaard Azure-abonnement en een abonnement dat specifiek is bedoeld voor uitval. Partners kunnen in de uitval beheren elk abonnement zien en toewijzen waar ze uitval mee willen maken.

De toewijzing van uitval wordt bepaald door *de eerste in de* regel. Als een partner E5 koopt met aanroepabonnementen voor een nieuwe klant, wordt er uitval toegewezen aan het verbruiksabonnement van deze partner. Als een tweede partner een ander exemplaar van E5 koopt met aanroepplannen, respecteert het systeem de aankoop en toewijzing van de eerste partner. Partners kunnen *uitval altijd beheren vanaf* de pagina abonnementen om deze uit te schakelen of uit te schakelen door uitval toe te wijzen aan *Geen.*

Uitvalinstellingen zijn per service per klant. Als een klant dezelfde uitvalservices van verschillende partners heeft, kan er slechts één uitvalabonnement tegelijk worden toegewezen. Als uitval moet worden gewijzigd van de ene partner in de andere, moeten de drie betrokken partijen eerst akkoord gaan. Zodra de klant akkoord gaat, kan de bestaande partner gewoon uitval instellen *op* Geen, zodat de andere partner de uitval kan instellen op zijn of haar abonnement.

API-ondersteuning voor telco-functies voor betalen per gebruik zijn onder andere:

- SKU-eigenschappen om de partner te helpen bepalen of een SKU uitval mogelijk maakt
- Een nieuwe API voor het toewijzen van uitval aan een bestaand abonnement of voor het instellen van uitval op *Geen*

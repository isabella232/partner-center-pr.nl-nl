---
title: New commerce telco pay as you go
ms.topic: article
ms.date: 08/30/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over nieuwe commerce-ervaringen voor het kopen van aanbiedingen waarmee u kunt betalen naar uitval.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0f934b8d858c1fc30d0140d19fb0697ba6bd9001
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957770"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Inleiding: Nieuwe commerce-uitval voor betalen via telco

**Juiste rollen**

- Beheeragent
- Verkoopagent
- Globale beheerder

> [!Note] 
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van Microsoft 365/Dynamics 365 New Commerce Experience Technical Preview.

Sommige op licenties gebaseerde producten omvatten services met toegewezen oproepplannen. Deze aanroepen van abonnementen worden doorgaans gebruikt voor een toewijzing per licentie voor minuten per maand, meestal 120 per licentie. 

In traditionele partnerscenario's op basis van licenties was er geen manier om servicegebruik buiten de maandelijkse limieten in te stellen. Klanten die meer dan 120 minuten nodig hebben om communicatietegoeden te kopen, of *comm-tegoed* zelf rechtstreeks van Microsoft.  Deze communicatietegoeden zijn niet aangeboden in Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Met behulp van nieuwe commerce telco betalen per gebruik ##

Deze beperking is verholpen in nieuwe handel waardoor de partner uitvalmogelijkheden kan inschakelen voor services die dit toestaan. Partners kunnen aanbiedingen kopen die uitvalmogelijkheden bevatten. Deze aanbiedingen worden geïdentificeerd in de kolom met prijslijsttags *die IncludeOverage bevat.* De catalogus-SKU bevat ook een eigenschap om te bepalen of de SKU de uitvalmogelijkheid ondersteunt. Partners kopen gewoon de aanbiedingen en het systeem configureert en verrekening van een abonnement dat geen kosten bevat en brengt alleen facturering met zich mee wanneer de gebruikers van de klant de toegewezen maandelijkse belminuten die bij de aangeschafte aanbieding worden ontvangen, over het bestek heen zien. 

Partners kunnen het uitvalgebruik traceren door naar de Azure Portal te gaan en de mogelijkheden en functies voor kostenbeheer te gebruiken. Partners hebben ook de mogelijkheid om de  uitval op elk moment in te stellen op Geen als ze uitval op elk moment willen uitschakelen of uitschakelen.

Partners kunnen bepalen welke producten uitvalmogelijkheden bevatten door de product-SKU's van de partnercentrumcatalogus te bekijken. 

Partners die producten met uitval aanschaffen, maken de uitval mogelijk door toegang te krijgen tot de pagina *Uitval* beheren op de pagina Abonnementen beheren. Hierdoor kan de partner uitval activeren en het gewenste verbruiksabonnement toewijzen waar de uitvalkosten naar gaan. De partner kan uitval op elk moment uitschakelen door het verbruiksabonnement toe te wijzen aan *Geen.* 

Partners wijzen uitval toe of schakelen deze uit met *de functie Uitval* beheren in de lijst met abonnementen. Dit is alleen toegankelijk als de partner abonnementen heeft die uitval mogelijk maken. Maandelijkse uitvalkosten worden bij het toegewezen abonnement opgeteld en worden geïdentificeerd in het afstemmingsbestand van partners. Partners kunnen het uitvalgebruik bijhouden door de mogelijkheden van Azure Cost Management in de Azure Portal. 

## <a name="important-details-about-overage"></a>Belangrijke informatie over uitval ##

Als u een product-SKU aanschaft die uitval mogelijk maakt, zorgt u er automatisch voor dat de klant van de partner is ingesteld voor stroom uitval. Dit omvat het maken van een gratis Azure-plan, een bijbehorend standaard Azure-abonnement en een abonnement dat specifiek is bedoeld voor uitval. Partners kunnen zien en toewijzen aan welk abonnement ze uitval willen laten maken in de uitval beheren.

De toewijzing van uitval wordt bepaald door *de eerste in de* regel. Als een partner E5 koopt met oproepabonnementen voor een nieuwe klant, wordt er uitval toegewezen aan het verbruiksabonnement van deze partner. Als een tweede partner een ander exemplaar van E5 met oproepplannen koopt, respecteert het systeem de aankoop en toewijzing van de eerste partner. Partners kunnen *uitval altijd beheren vanaf* de pagina abonnementen om deze uit te schakelen of uit te schakelen door uitval toe te wijzen aan *Geen.*

Uitvalinstellingen zijn per service per klant. Als een klant dezelfde uitvalservices van verschillende partners heeft, kan er slechts één uitvalabonnement tegelijk worden toegewezen. Als uitval moet worden gewijzigd van de ene partner in de andere, moeten de drie betrokken partijen het eerst met elkaar eens worden. Zodra ze akkoord gaan, kan de bestaande partner gewoon uitval instellen op *Geen,* zodat de andere partner uitval kan instellen op zijn of haar abonnement.

API-ondersteuning voor telco pay as you go-functies zijn onder andere:

- SKU-eigenschappen om de partner te helpen bepalen of een SKU uitval mogelijk maakt
- Een nieuwe API voor het toewijzen van uitval aan een bestaand abonnement of het instellen van uitval op *Geen*

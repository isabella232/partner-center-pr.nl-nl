---
title: New commerce telco pay-as-you-go
ms.topic: article
ms.date: 09/03/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over nieuwe commerce-ervaringen voor het kopen van aanbiedingen die uitval op betalen per uur mogelijk maken.
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a6abf0a837758819fba8c3a584ba68216657a2b9
ms.sourcegitcommit: 76a7dac540d129ae15cd4c251a4ff43d768370da
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/06/2021
ms.locfileid: "129593239"
---
# <a name="introduction-new-commerce-overage-for-telco-pay-as-you-go"></a>Inleiding: Nieuwe commerce-uitval voor telco betalen per uur

**Juiste rollen**

- Beheeragent
- Verkoopagent
- Globale beheerder

> [!NOTE]
> De wijzigingen in de nieuwe commerce-ervaring zijn momenteel alleen beschikbaar voor partners die deel uitmaken van Microsoft 365/Dynamics 365 New Commerce Experience Technical Preview.

Sommige op licenties gebaseerde producten omvatten services met toegewezen aanroepplannen die doorgaans een toewijzing per licentie bevatten voor minuten per maand, meestal 120 per licentie. 

In traditionele partnerscenario's op basis van licenties was er geen manier om servicegebruik buiten de maandelijkse limieten in te stellen. Klanten die meer dan 120 minuten nodig hebben om communicatietegoeden te kopen, of *comm-tegoeden* zelf rechtstreeks van Microsoft.  Deze communicatietegoeden zijn niet aangeboden in Partner Center.

## <a name="using-new-commerce-telco-pay-as-you-go"></a>Met behulp van nieuwe commerce telco betalen per gebruik

Deze beperking is verholpen in nieuwe handel waardoor de partner uitvalmogelijkheden kan inschakelen voor services die dit toestaan. Partners kunnen aanbiedingen kopen die uitvalmogelijkheden bevatten. Deze aanbiedingen worden geïdentificeerd in de kolom met prijslijsttags *die IncludeOverage bevat.* De catalogus-SKU bevat ook een eigenschap om te bepalen of de SKU de uitvalmogelijkheid ondersteunt. Partners kopen gewoon de aanbiedingen aan en het systeem configureert een uitvalabonnement zonder kosten en brengt alleen facturering met zich mee wanneer de gebruikers van de klant de toegewezen maandelijkse belminuten die bij de aangeschafte aanbieding worden ontvangen, over het hele jaar over het hele bedrijf heen laten lopen. 

Partners kunnen bepalen welke product-SKU's uitvalmogelijkheden bevatten door 

- De product-SKU's van de partnercentrumcatalogus weergeven
- De nieuwe lijst met commerceprijzen filteren op **includesOverage** in de kolom tags

Partners die producten met uitval aanschaffen, kunnen dit doen door toegang te krijgen tot de pagina **Uitval** beheren op de pagina Abonnementen beheren. Met de beheer-uitvalinterface kan de partner activeren en toewijzen naar welk Azure-abonnement de uitvalkosten gaan. De partner kan uitval op elk moment uitschakelen door het verbruiksabonnement toe te wijzen aan *Geen.* 

> [!NOTE]
> Voor het beheren van uitval is de mogelijkheid vereist om een Azure-plan te maken. Standaard kunnen partners geen Azure-abonnementen inrichten met behulp van hun sandbox-accounts. Partners die dit willen doen met hun sandbox-account, moeten toegang aanvragen. Meer informatie vindt u in de sandboxdocumentatie [van het Azure-plan.](/partner-center/develop/test-and-debug#azure-plan)

Partners wijzen uitval toe of schakelen deze uit met *de functie Uitval* beheren in de lijst met abonnementen. Dit is alleen toegankelijk als de partner abonnementen heeft die uitval mogelijk maken. Maandelijkse uitvalkosten worden bij het toegewezen abonnement opgeteld en worden geïdentificeerd in het afstemmingsbestand van partners. Partners kunnen het uitvalgebruik bijhouden door de mogelijkheden van Azure Cost Management in de Azure Portal. 

Partners kunnen het uitvalgebruik traceren door naar de Azure Portal en de mogelijkheden en functies voor kostenbeheer te gebruiken. 

## <a name="important-details-about-overage"></a>Belangrijke informatie over uitval

- Als u een product-SKU op basis van licenties aanschaft die uitvalmogelijkheden bevat, wordt alleen het product op basis van licenties gekocht. Partners moeten na aankoop nog een stap nemen om uitval in te zetten door naar de pagina abonnementsbeheer te gaan en op Uitval **beheren te klikken**
- Alleen beheerdersagenten voor de transactingpartner kunnen uitval inschakelen na de aankoop op basis van licenties. 
- Als u uitval inschakelen, maakt u een gratis Azure-plan en een bijbehorend standaard Azure-abonnement **abonnement 1,** specifiek voor uitval. Als het Azure-plan al bestaat, wordt met het inschakelen van uitval het nieuwe abonnement onder het bestaande Azure-plan gemaakt. Partners kunnen uitval altijd weergeven of opnieuw toewijzen aan andere abonnementen in **De uitval beheren.** Klanten die nog geen Azure-abonnement (oudere Azure) hebben, moeten overstappen op een Azure-plan voordat ze uitval kunnen inschakelen.

De toewijzing van uitval wordt bepaald door *de eerste in de* regel. Als een partner E5 koopt met oproepabonnementen voor een nieuwe klant, wordt er uitval toegewezen aan het verbruiksabonnement van deze partner. Als een tweede partner een ander exemplaar van E5 met oproepplannen koopt, respecteert het systeem de aankoop en toewijzing van de eerste partner. Partners kunnen *uitval altijd beheren vanaf* de pagina abonnementen om deze uit te schakelen of uit te schakelen door uitval toe te wijzen aan *Geen.*

Uitvalinstellingen zijn per service per klant. Er kan slechts één uitvalabonnement tegelijk worden toegewezen. Als uitval moet worden gewijzigd van de ene partner in de andere, moeten de drie betrokken partijen het eerst met elkaar eens worden. Zodra ze akkoord gaan, kan de bestaande partner gewoon uitval instellen op *Geen,* zodat de andere partner uitval kan instellen op zijn of haar abonnement.

## <a name="telco-pay-as-you-go-apis"></a>Telco Pay-As-You-Go-API's

- [SKU-eigenschappen](/partner-center/develop/product-resources#sku) bevatten een *eigenschap consumptionType* om de partner te helpen bepalen of een SKU uitval mogelijk maakt
- [Uitval om](/partner-center/develop/get-subscription-overage) te begrijpen of er momenteel uitval is ingesteld voor uw klant
- [Uitval bijwerken om](/partner-center/develop/update-subscription-overage) de uitval van de klant bij te werken naar een Azure-abonnement of om deze in te stellen op *Geen*

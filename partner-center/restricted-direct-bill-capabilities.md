---
title: Beperkte mogelijkheden voor directe facturering
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Meer informatie over Cloud Solution Provider (CSP) vereisten voor directe factuurpartners en wat u moet doen om te voorkomen dat mogelijkheden worden beperkt. Uitzoeken of uw mogelijkheden zijn beperkt.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: edb67f6ae3054bf5214611ab3ac5ef4ed6713aef
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114836656"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Beperkte mogelijkheden voor directe factuur en de vereisten die nodig zijn voor CSP-partners voor directe factuur

**Juiste rollen:** globale beheerder

## <a name="overview"></a>Overzicht

Partners met directe factuur moeten voldoen aan de nieuwe [vereisten om](direct-partner-new-requirements.md) te blijven werken met het Cloud Solution Provider (CSP) direct bill partner-programma. Anders wordt de toegang tot mogelijkheden voor directe factuur uiteindelijk beperkt en kunnen er meer specifieke taken worden uitgevoerd, zoals het doen van nieuwe aankopen voor hun klanten.

> [!Note]
> Partners met directe factuur die niet voldoen aan de nieuwe vereisten voor het CSP-partnerprogramma voor directe factuur, worden door Microsoft op de hoogte gesteld wanneer hun mogelijkheden voor directe factuur worden beperkt. Dit geldt voor alle directe factuurpartners, ongeacht of ze hebben gekozen voor een overgang van partner voor directe factuur [naar indirecte resellers](transition-direct-to-indirect.md) of niet.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Na te gaan of de mogelijkheden van uw directe factuur zijn beperkt

Volg deze stappen om te controleren of de toegang van de tenant van de directe factuurpartner tot de mogelijkheden voor directe factuur is beperkt.

1. Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard).

2. Ga naar **Accountinstellingen**  >  **Juridisch profiel.**

3. Zoek **onder Programmagegevens** naar **Microsoft Cloud Solution Provider status**.

4. Als de programmastatus de waarde **beperkt heeft,** betekent dit dat de toegang van de tenant van uw directe factuurpartner tot de mogelijkheden voor directe factuur is beperkt.

## <a name="affected-direct-bill-capabilities"></a>Betrokken mogelijkheden voor directe factuur

Als de mogelijkheden voor directe factuur zijn beperkt, kunt u geen nieuwe aankopen meer doen voor uw klanten in Partner Center. Deze beperking omvat:

- Azure-abonnementen

- Op licenties gebaseerde abonnementen

- Voeg nieuwe invoegtoepassingen toe aan bestaande abonnementen op basis van licenties.

- Een een keer software- en reserveringsproducten aanschaffen (bijvoorbeeld softwareabonnementen, permanente software en azure-instanties voor gereserveerde virtuele machines).

U kunt ook de aanbieding voor gedeelde [services van azure-partners in](shared-services.md) het CSP-programma niet gebruiken om nieuwe Azure-abonnementen voor uw eigen gebruik aan te schaffen.

Bestaande abonnementen op directe factuur worden niet beïnvloed. Ze blijven geldig en zijn autorenewed. U wordt nog steeds rechtstreeks door Microsoft gefactureerd totdat ze zijn geannuleerd. U kunt bestaande abonnementen nog steeds op de volgende manieren beheren:

- Bestaande abonnementen opschorten

- Het aantal licenties van bestaande op licenties gebaseerde abonnementen aanpassen

- Het aantal licenties van bestaande invoegtoepassingen aanpassen aan een abonnement. 

    >[!Note]
    >U kunt geen nieuwe invoegtoepassingen toevoegen aan bestaande abonnementen, omdat deze worden behandeld als nieuwe aankoop.

- Implementeer nieuwe Azure-resources en beheer bestaande Azure-resources onder bestaande Azure-abonnementen. Dit omvat resources die beschikbaar zijn via Azure Marketplace en Visual Studio-abonnementen.

Naast nieuwe aankopen hebt u geen toegang tot de volgende mogelijkheden voor directe factuur in Partner Center:

- U kunt geen nieuwe tenants voor klanten maken. De **optie Klant** maken op de **pagina** Klanten in Partner Center is niet beschikbaar.

- U kunt geen uitnodiging genereren voor klanten die een rechtstreekse resellerrelatie aanvragen. De **optie Een resellerrelatie aanvragen** op de **pagina** Klanten in Partner Center is niet beschikbaar.

    >[!NOTE]
    >Als onderdeel van de overgang van directe factuurpartner naar indirecte reseller, kunt u, als u de tenant van uw directe factuurpartner al hebt geregistreerd als indirecte reseller, in plaats daarvan een uitnodiging genereren voor klanten die een indirecte resellerrelatie aanvragen.

- U kunt geen nieuwe sandbox-tenant maken. Elke tenant van een directe factuurpartner kan één sandbox-tenant maken voor API-integratie met directe factuur. Als u nog geen partner hebt gemaakt, kunt u dit niet doen nadat de mogelijkheid van uw partner voor directe factuur is beperkt.  

## <a name="next-steps"></a>Volgende stappen

- [Aanvullende informatie over hoe u een indirecte reseller wordt](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nieuwe vereisten voor directe CSP-partner](direct-partner-new-requirements.md)

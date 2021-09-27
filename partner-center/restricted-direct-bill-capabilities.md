---
title: Beperkte mogelijkheden voor directe facturering
ms.topic: article
ms.date: 09/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Meer informatie over Cloud Solution Provider (CSP) vereisten voor directe factuurpartners en wat u kunt doen om te voorkomen dat mogelijkheden worden beperkt. Uitzoeken of uw mogelijkheden zijn beperkt.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: ebd364c1268217579316338e884d96491ddd70fb
ms.sourcegitcommit: d731813da1d31519dc2dc583d17899e5cf4ec1b2
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/27/2021
ms.locfileid: "129070742"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Beperkte mogelijkheden voor directe factuur en de vereisten die nodig zijn voor CSP-partners voor directe factuur

**Juiste rollen:** globale beheerder

## <a name="overview"></a>Overzicht

Partners met directe factuur moeten voldoen aan de nieuwe [vereisten om](direct-partner-new-requirements.md) te blijven Cloud Solution Provider het CSP-programma voor directe factuurpartners. Anders wordt de toegang tot mogelijkheden voor directe factuur uiteindelijk beperkt en kunnen ze meer specifieke taken uitvoeren, zoals het doen van nieuwe aankopen voor hun klanten.

> [!Note]
> Partners met directe factuur die niet voldoen aan de nieuwe vereisten voor het CSP-partnerprogramma voor directe factuur, worden door Microsoft geïnformeerd wanneer hun mogelijkheden voor directe factuur worden beperkt. Dit geldt voor alle directe factuurpartners, ongeacht of ze hebben gekozen voor een overgang van partner voor directe factuur [naar indirecte resellers](transition-direct-to-indirect.md) of niet.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Na gaan of de mogelijkheden van uw directe factuur zijn beperkt

Volg deze stappen om te controleren of de toegang van de tenant van de directe factuurpartner tot de mogelijkheden voor directe factuur is beperkt.

1. Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard).

2. Selecteer het Instellingen tandwielpictogram, vervolgens **Accountinstellingen** en selecteer **vervolgens Juridisch profiel.**

3. Zoek **onder Programmagegevens** naar **Microsoft Cloud Solution Provider status**.

4. Als de programmastatus de waarde **beperkt heeft,** betekent dit dat de toegang van de tenant van uw directe factuurpartner tot de mogelijkheden voor directe factuur is beperkt.

## <a name="affected-direct-bill-capabilities"></a>Betrokken mogelijkheden voor directe factuur

Als de mogelijkheden voor directe factuur zijn beperkt, kunt u geen nieuwe aankopen meer doen voor uw klanten in Partner Center. Deze beperking omvat:

- Azure-abonnementen

- Op licenties gebaseerde abonnementen

- Voeg nieuwe invoegtoepassingen toe aan bestaande abonnementen op basis van licenties.

- Een een time-aankoop doen van software- en reserveringsproducten (bijvoorbeeld softwareabonnementen, permanente software en Gereserveerde VM-instanties van Azure).

U kunt ook de aanbieding voor gedeelde [services van de Azure-partner](shared-services.md) onder het CSP-programma niet gebruiken om nieuwe Azure-abonnementen voor uw eigen gebruik aan te schaffen.

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
    >Als onderdeel van de overgang van directe factuurpartner naar indirecte reseller, kunt u in plaats daarvan een uitnodiging genereren voor klanten die een indirecte resellerrelatie aanvragen als u de tenant van uw directe factuurpartner al hebt geregistreerd als indirecte reseller.

- U kunt geen nieuwe sandbox-tenant maken. Elke tenant van een directe factuurpartner kan één sandbox-tenant maken voor API-integratie met directe factuur. Als u er nog geen hebt gemaakt, kunt u dit niet doen nadat de mogelijkheid van uw directe factuurpartner is beperkt.  

## <a name="next-steps"></a>Volgende stappen

- [Aanvullende informatie over hoe u een indirecte reseller wordt](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Nieuwe vereisten voor directe CSP-partner](direct-partner-new-requirements.md)

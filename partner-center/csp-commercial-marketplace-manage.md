---
title: Marketplace-Producten & aanbiedingen beheren
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Met behulp van partner centrum leert u hoe u met Cloud Solution Providers ISV-aanbiedingen van derden kunt beheren die zijn gekocht voor klanten van de commerciële Marketplace.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1d32f42b2c4bd8e4ec6c659326d1a21385c0642f
ms.sourcegitcommit: 51e3c912eba8cfa72733206c0fee22386fbc34aa
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/22/2020
ms.locfileid: "92528582"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Commerciële Marketplace-Producten en aanbiedingen voor uw klanten beheren

**Van toepassing op**

- Partnercentrum
- Partners in het CSP-programma

**Juiste rollen**

- Globale beheerder
- Beheer agent

Partners in het programma Cloud Solution Provider (CSP) kunnen de Partner Center-Portal gebruiken om veel ISV SaaS-aanbiedingen of-abonnementen voor hun klanten te kopen van de commerciële Marketplace. Zodra u een aanbieding hebt gekocht, hebt u verschillende manieren om deze te beheren.

## <a name="view-or-edit-a-subscription"></a>Een abonnement weer geven of bewerken

Nadat u een abonnement hebt aangeschaft bij een onafhankelijke ISV-Uitgever, kunt u deze als volgt controleren of bewerken:

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum en selecteer vervolgens **klanten** in het navigatie menu links.

2. Selecteer een geschikte klant en selecteer vervolgens **abonnementen** . Hier vindt u een overzicht van de op licenties gebaseerde abonnementen die u hebt aangeschaft voor de klant.

3. Selecteer in de kolom **abonnement** het abonnement dat u wilt weer geven of bewerken. Dit geeft u meer informatie over het instellen of inrichten van de aanbieding. (Als er meer acties nodig zijn voor de aanbieding, wordt mogelijk ook de status ' actie vereist ' weer gegeven in de kolom Status. Dit kan ook vergezeld gaan van een koppeling naar de site van de ISV-Uitgever.)

4. Zodra u het abonnement hebt geselecteerd dat u wilt weer geven of bewerken, kunt u op de detail pagina van het abonnement het abonnement bewerken en op de volgende manieren te werk gaan:

    - De bijnaam van het abonnement wijzigen

    - Het aantal licenties in het abonnement toevoegen/verlagen

    - Het abonnement opzeggen

    - Automatisch vernieuwen uitschakelen

    - Een indirecte wederverkoper MPN-ID toevoegen, indien van toepassing

> [!NOTE]
> Mogelijk moet u bepaalde stappen uitvoeren die zijn gedefinieerd door de ISV-uitgever voordat u een aantal wijzigingen kunt aanbrengen in een abonnement, zoals het annuleren van een abonnement.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Licenties toewijzen en een abonnement activeren namens een klant

Wanneer u een SaaS-aanbieding (Software as a Service) aanschaft die door een onafhankelijke software leverancier (ISV) wordt aangeboden in de commerciële Marketplace, helpt de ISV-uitgever het proces van het toewijzen van licenties en het activeren van het abonnement namens uw klant te beheren.

De uitgever moet u een gepersonaliseerde koppeling geven en een autorisatie code die uw specifieke aankoop identificeert.

1. U kunt deze aangepaste koppeling op een paar manieren vinden in de ISV-Uitgever:

   - U kunt de koppeling zien op de bevestigings pagina die wordt weer gegeven nadat u een ISV SaaS-aanbieding hebt aangeschaft. Als u deze koppeling wilt vinden op de pagina, zoekt en selecteert u **Ga naar de site van de Publisher** .

   - U kunt de koppeling zien op de pagina Abonnementen van de specifieke klant. Deze Publisher-koppeling wordt weer gegeven in de rij die is gekoppeld aan de ISV-aanbieding of het aangeschafte abonnement voor de klant.

   - U kunt [de koppeling ophalen met behulp van partner Center-api's](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Als u dit namens uw klant wilt doen, moet u de gepersonaliseerde koppeling wellicht kopiëren, in een persoonlijke browser plakken en de referenties van de klant invoeren.

2. Zodra u zich op de site of het systeem van de ISV-Uitgever bevindt, kunt u met de uitgever weten welke extra stappen u moet uitvoeren om het installatie proces van de klant te volt ooien en licenties in te richten of toe te wijzen.

3. Als partner in het CSP-programma die namens uw klant werkt, bent u verantwoordelijk voor het uitvoeren van de volgende taken:

    - Verzend de vereiste informatie naar de uitgever.

    - Stuur een vereiste URL rechtstreeks naar uw klant (of Communiceer rechtstreeks informatie over dit abonnement naar uw klant)

4. Zodra u de vereiste informatie voor de uitgever hebt opgegeven, worden de juiste licenties door de uitgever ingericht en toegewezen. De facturering van abonnementen wordt alleen gestart nadat de volgende gebeurtenissen optreden:

    - De ISV-uitgever heeft de juiste licenties toegewezen

    - De ISV-Uitgever is met micro soft bevestigd (via een afzonderlijke, SaaS-fulfillment API) dat de account installatie is voltooid

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Een op licentie gebaseerd SaaS-abonnement op een ISV-Uitgever annuleren

Wanneer u zich abonneert op een op licenties gebaseerd SaaS-product dat wordt aangeboden door een ISV-Uitgever binnen de commerciële Marketplace, hebt u de mogelijkheid om het abonnement binnen de aangewezen annulerings periode te annuleren. Deze annulerings periode verandert, afhankelijk van of u een maandelijks of jaarlijks abonnement hebt. U kunt ook kiezen of u het abonnement automatisch wilt vernieuwen.

Zie voor meer informatie over de annulerings perioden die van toepassing zijn, het annuleren of het automatisch vernieuwen van een abonnement.

- [Een abonnement annuleren](create-a-new-subscription.md#cancel-a-subscription)

- [Een abonnement op commerciële Marketplace automatisch vernieuwen](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Licenties toevoegen aan of verwijderen voor een SaaS-abonnement

Voor SaaS-Commercial Marketplace-aanbiedingen kunt u gebruikers licenties toevoegen aan of verwijderen uit een klant abonnement.

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van het partner centrum en selecteer vervolgens **klanten** in het navigatie menu links.

2. Selecteer een geschikte klant en selecteer vervolgens **abonnementen** . Hier vindt u een overzicht van de op licenties gebaseerde abonnementen die u hebt aangeschaft voor de klant.

3. Selecteer in de kolom **abonnement** het abonnement dat u wilt wijzigen.

4. Zoek op de pagina abonnements Details het veld **hoeveelheid** . Hier kunt u het aantal licenties verhogen of verlagen.

5. Wijzig de hoeveelheid en selecteer vervolgens **verzenden** .

## <a name="manage-subscriptions-using-partner-center-apis"></a>Abonnementen beheren met partner Center-Api's

U kunt ook partner Center-Api's gebruiken voor het uitvoeren van levenscyclus beheer en het beheren van facturen voor uw abonnementen. Zie [een abonnement voor commerciële Marketplace-producten maken](/partner-center/develop/create-subscription-azure-marketplace-products)voor meer informatie.

## <a name="next-steps"></a>Volgende stappen

- [Commerciële Marketplace-aanbiedingen kopen](csp-commercial-marketplace-purchase.md)
- [Meer informatie over facturering in de commerciële Marketplace](csp-commercial-marketplace-billing.md)
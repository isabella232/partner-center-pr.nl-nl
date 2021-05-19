---
title: Marketplace-producten en & beheren
ms.topic: how-to
ms.date: 07/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Leer Partner Center hoe cloudoplossingsproviders ISV-aanbiedingen van derden kunnen beheren die zijn gekocht voor klanten van de commerciële marketplace.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e1bb2752dad5325478496c83fc368943780d8afb
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147901"
---
# <a name="manage-commercial-marketplace-products-and-offers-for-your-customers"></a>Commerciële marketplace-producten en -aanbiedingen voor uw klanten beheren


**Juiste rollen:** Globale | Beheeragent

Partners in het Cloud Solution Provider-programma (CSP) kunnen de Partner Center-portal gebruiken om veel ISV SaaS-aanbiedingen of -abonnementen voor hun klanten te kopen via de commerciële marketplace. Nadat u een aanbieding hebt aangeschaft, kunt u deze op verschillende manieren beheren.

## <a name="view-or-edit-a-subscription"></a>Een abonnement weergeven of bewerken

Nadat u een abonnement van een externe ISV-uitgever hebt aangeschaft, kunt u dit als volgt controleren of bewerken:

1. Meld u aan Partner Center [dashboard en](https://partner.microsoft.com/dashboard)selecteer vervolgens **Klanten** in het navigatiemenu aan de linkerkant.

2. Selecteer een geschikte klant en selecteer **vervolgens Abonnementen.** Hiermee worden alle op licenties gebaseerde abonnementen vermeld die u voor de klant hebt aangeschaft.

3. Selecteer in **de** kolom Abonnement het abonnement dat u wilt weergeven of bewerken. Dit biedt u meer informatie over het instellen of inrichten van de aanbieding. (Als er meer actie nodig is voor de aanbieding, wordt mogelijk ook de status Actie nodig weergegeven in de kolom Status. Dit kan ook vergezeld gaan van een koppeling naar de site van de ISV-uitgever.)

4. Zodra u het abonnement hebt geselecteerd dat u wilt bekijken of bewerken, kunt u op de detailpagina van het abonnement het abonnement bewerken en bijvoorbeeld het volgende doen:

    - De bijnaam van het abonnement wijzigen

    - Het aantal licenties in het abonnement toevoegen/verlagen

    - Het abonnement opzeggen

    - Automatisch vernieuwen uitschakelen

    - Een MPN-id voor indirecte resellers toevoegen, indien van toepassing

> [!NOTE]
> Mogelijk moet u bepaalde stappen uitvoeren die zijn gedefinieerd door de ISV-uitgever voordat u enkele wijzigingen in een abonnement kunt uitvoeren, zoals het annuleren van een abonnement.

## <a name="assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer"></a>Licenties toewijzen en een abonnement activeren namens een klant

Wanneer u een SaaS-aanbieding (Software as a Service) aanschaft die wordt geleverd door een ISV-uitgever (Independent Software Vendor) in de commerciële marketplace, helpt de ISV-uitgever bij het beheren van het proces van het toewijzen van licenties en het activeren van het abonnement namens uw klant.

De uitgever moet u een gepersonaliseerde koppeling en een autorisatiecode verstrekken die uw specifieke aankoop identificeert.

1. U vindt deze gepersonaliseerde koppeling van de ISV-uitgever op een aantal manieren:

   - U kunt de koppeling zien op de bevestigingspagina die wordt weergegeven nadat u een ISV SaaS-aanbieding hebt aangeschaft. Als u deze koppeling op de pagina wilt vinden, gaat u naar de **site van de uitgever en selecteert u deze.**

   - U kunt de koppeling bekijken op de pagina Abonnementen van de specifieke klant. Deze uitgeverskoppeling wordt weergegeven in de rij die is gekoppeld aan de ISV-aanbieding of het abonnement dat voor de klant is gekocht.

   - U kunt [de koppeling ophalen met behulp Partner Center API's](/partner-center/develop/get-activation-link-by-order-line-item).

   > [!NOTE]
   > Als u dit namens uw klant wilt doen, moet u mogelijk de gepersonaliseerde koppeling kopiëren, deze in een privébrowser plakken en de referenties van de klant invoeren.

2. Zodra u zich in de site of het systeem van de ISV-uitgever hebt geplaatst, laat de uitgever u weten welke extra stappen u moet nemen om het installatieproces van de klant te voltooien en licenties in terichten of toe te wijzen.

3. Als partner in het CSP-programma dat namens uw klant werkt, bent u verantwoordelijk voor het uitvoeren van de volgende taken:

    - Dien de vereiste gegevens in bij de uitgever.

    - Elke vereiste URL rechtstreeks naar uw klant verzenden (of anderszins rechtstreeks details over dit abonnement naar uw klant communiceren)

4. Zodra u de vereiste gegevens aan de uitgever hebt verstrekt, zal de uitgever de juiste licenties inrichten en toewijzen. Abonnementsfacturering begint pas nadat de volgende gebeurtenissen optreden:

    - De ISV-uitgever heeft de juiste licenties toegewezen

    - De ISV-uitgever heeft aan Microsoft (via een afzonderlijke SaaS-uitvoerings-API) bevestigd dat het instellen van het account is voltooid

## <a name="cancel-a-license-based-saas-subscription-from-an-isv-publisher"></a>Een SaaS-abonnement op basis van een licentie annuleren van een ISV-uitgever

Wanneer u zich abonneert op een SaaS-product op basis van licenties dat wordt aangeboden door een ISV-uitgever binnen de commerciële marketplace, hebt u de mogelijkheid om het abonnement te annuleren binnen de aangewezen annuleringsperiode. Deze annuleringsperiode verandert, afhankelijk van of u een maandelijks of jaarlijks abonnement hebt. U kunt ook kiezen of u het abonnement automatisch wilt verlengen.

Zie voor meer informatie over annuleringsperioden die van toepassing zijn, het annuleren of automatisch verlengen van een abonnement:

- [Een abonnement annuleren](create-a-new-subscription.md#cancel-a-subscription)

- [Een abonnement op de commerciële marketplace automatisch verlengen](create-a-new-subscription.md#choose-whether-to-automatically-renew-a-commercial-marketplace-subscription)

## <a name="add-or-remove-licenses-for-a-saas-subscription"></a>Licenties voor een SaaS-abonnement toevoegen of verwijderen

Voor aanbiedingen op de commerciële SaaS-marketplace kunt u gebruikerslicenties voor een klantabonnement toevoegen of verwijderen.

1. Meld u aan Partner Center [dashboard en](https://partner.microsoft.com/dashboard)selecteer klanten in het navigatiemenu aan de linkerkant. 

2. Selecteer een geschikte klant en selecteer **vervolgens Abonnementen.** Hier worden alle op licenties gebaseerde abonnementen vermeld die u voor de klant hebt aangeschaft.

3. Selecteer in **de** kolom Abonnement het abonnement dat u wilt wijzigen.

4. Zoek op de pagina met abonnementsdetails het **veld Hoeveelheid.** Hier kunt u het aantal licenties verhogen of verlagen.

5. Wijzig de hoeveelheid en selecteer vervolgens **Verzenden.**

## <a name="manage-subscriptions-using-partner-center-apis"></a>Abonnementen beheren met behulp van Partner Center API's

U kunt ook Partner Center's gebruiken om levenscyclusbeheer uit te voeren en facturen voor uw abonnementen te beheren. Zie Een abonnement maken voor [commerciële marketplace-producten voor meer informatie.](/partner-center/develop/create-subscription-azure-marketplace-products)

## <a name="next-steps"></a>Volgende stappen

- [Aanbiedingen voor de commerciële marketplace kopen](csp-commercial-marketplace-purchase.md)
- [Meer informatie over facturering in de commerciële marketplace](csp-commercial-marketplace-billing.md)
---
title: Facturering voor commerciële marketplace-producten
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-billing
description: Ontdek hoe facturering werkt voor ISV SaaS-producten of -abonnementen die zijn gekocht voor klanten van de commerciële marketplace binnen Partner Center.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 102f13530ece08cd813412a44897ece0186e7cbb
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123956932"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Facturering voor commerciële marketplace-producten en -abonnementen in Partner Center


**Juiste rollen:** Globale | Factureringsbeheerder

Als partner in het CSP-programma kunt u Partner Center SaaS-producten op basis van licenties kopen bij ISV-uitgevers in de commerciële marketplace. Nadat u dit hebt gedaan, hebt u toegang tot een factuur voor deze typen aankopen. De factureringsperiode begint op de eerste dag van de kalendermaand en eindigt op de laatste dag van de kalendermaand. Facturen worden beschikbaar gesteld op de 8e dag van de volgende maand.

U hebt toegang tot facturen vanuit het Partner Center [dashboard](https://partner.microsoft.com/dashboard/) of met behulp [van Partner Center API's.](/partner-center/develop/)

Partners in het CSP-programma worden gefactureerd voor isV-oplossingen op de commerciële marketplace die zijn gekocht voor een klant wanneer ze deze producten kopen bij Partner Center of bij de Azure Portal (met behulp van de eerder door CSP gekochte Azure-tenant van de klant).

>[!NOTE]
>Als klanten hun eigen Azure AD-tenant gebruiken (niet een die is aangeschaft bij een partner in het CSP-programma), kunnen klanten er ook voor kiezen om hun eigen ISV SaaS-oplossing rechtstreeks te kopen vanuit ([Microsoft AppSource](https://appsource.microsoft.com/) of [Azure Marketplace).](https://azuremarketplace.microsoft.com/) Als ze dit doen, ontvangen ze hun eigen factuur rechtstreeks van Microsoft. En als een partner in het CSP-programma een [Azure-abonnement](/azure/role-based-access-control/built-in-roles) of het nieuwe Azure-plan aan de klant verkoopt en de klant (of indirecte reseller) op rollen gebaseerde toegang verleent tot die tenant (een rol toewijzen aan de klant naast **Lezer),** kan die klant (of indirecte reseller) ook aanbiedingen van de commerciële marketplace kopen zonder voorafgaande goedkeuring of melding aan de CSP-partner. In dergelijke gevallen zal Microsoft partners in het CSP-programma niet rechtstreeks op de hoogte stellen van aankopen van hun klanten. Microsoft biedt echter een optionele Azure Monitor [waarmee](/azure/azure-monitor/platform/alerts-activity-log) u waarschuwingen of meldingen over activiteiten in een Azure-abonnement kunt instellen.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Toegang tot factureringsgegevens voor commerciële marketplace-producten

De globale beheerder of factureringsbeheerder voor uw bedrijf ontvangt een e-mail wanneer een factuur gereed is om te worden bekeken. Voor toegang tot het meest recente factuur- en afstemmingsbestand voor productaankopen op de commerciële marketplace:

1. Meld u aan bij het [dashboard](https://partner.microsoft.com/dashboard/) van het Partnercentrum.

2. Selecteer in Partner Center menu **Facturering.** 

    Boven aan de pagina Facturering ziet u twee tabbladen: **Terugkerende** en Terugkerende en **eenmalige aankopen.** Op elk tabblad hebt u toegang tot factuur- en afstemmingsbestanden voor verschillende Marketplace-producten:

    - **Tabblad** Terugkerend: hier worden factuur- en afstemmingsbestanden weergegeven voor abonnementen met betrekking tot Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro en Microsoft Azure.

    - **Tabblad Terugkerende en eenmalige aankopen:** Toont factuur- en afstemmingsbestanden voor Azure-plan, Azure-reserveringen, software en commerciële marketplace-producten.
  
3. Selecteer het **tabblad Terugkerende en eenmalige** aankopen. Als u abonnementen voor een klant in een andere valuta hebt aangeschaft, ziet u een tabblad voor elke valuta. U kunt op deze pagina enkele dingen doen:

    - Als u het meest recente factuur- en afstemmingsbestand wilt zien, **selecteert u Factuur-** **of Afstemmingsbestand.** (Als u wilt, kunt u ook toegang krijgen tot de meest recente factuur- en recon-bestandsgegevens met behulp [Partner Center API's.](/partner-center/develop/)

    - Als u eerdere facturen en recon-bestanden wilt bekijken, vouwt u de **onderstaande** rij Factureringsgeschiedenis uit.

    - Als u het geschatte saldo of de factuur op elk moment wilt controleren op basis van de meest recente accountactiviteit, selecteert u een koppeling onder **de kop Schattingen.**  

    >[!NOTE]
    > Wanneer uw factuur op de 8e dag van de maand wordt posten, worden de belastingen en eventuele andere toepasselijke kosten en tegoeden in rekening gebracht. Dit betekent dat het uiteindelijke verschuldigde bedrag kan verschillen van wat u ziet tijdens de factureringsperiode.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Meer informatie over facturen en recon-bestanden voor commerciële marketplace-producten

Deze sectie biedt meer informatie over factuur- en afstemmingsbestanden voor SaaS-abonnementen op de commerciële marketplace die zijn gekocht voor klanten van externe ISV-uitgevers.

Wanneer u Terugkerende en eenmalige aankopen  selecteert bij de optie Facturering in het menu Partner Center, krijgt u toegang tot facturen en **afstemmingsbestanden** voor kosten die betrekking hebben op aankopen van Zowel Microsoft (eigen partij) als ISV-aankopen (van derden). Deze aankopen kunnen worden gekoppeld aan:

- SaaS-abonnementen (van Microsoft- of ISV-uitgevers)

- Azure-abonnement

- Azure-reserveringen

- Andere op abonnementen gebaseerde software (van Microsoft- of ISV-uitgevers)

Voorbeelden van deze aankopen zijn bijvoorbeeld SUSE Linux-software (een softwareabonnement) of een Azure ISV SaaS-productabonnement.

>[!NOTE]
> Zie ook Factureringsoverzicht voor meer informatie over het lezen van factuur- en [reconsefactureringsbestanden.](billing.md)

### <a name="tips-on-reading-your-invoice"></a>Tips uw factuur lezen

Wanneer u een SaaS-product op basis van een licentie aanschaft bij een externe ISV-uitgever, ziet u alleen de kosten voor de licentiekosten op uw factuur. Dit geldt ook wanneer het SaaS-product van de ISV onderliggende Azure-infrastructuurbronnen gebruikt (of verbruikt). Dat komt doordat de gebruikskosten van de Azure-infrastructuur van uw klant voor het SaaS-product van een ISV rechtstreeks worden gefactureerd bij de ISV. (ISV's zien de bijbehorende Azure-verbruikskosten in hun eigen dagelijks beoordeelde factuurafstemmingsbestand voor Azure-gebruik.)

Uw factuur bevat verschillende pagina's:

- **Pagina 1 van de factuur:** Bevat een overzicht van de factureringsgegevens van de CSP-programmapartner. Dit omvat een overzicht van de kosten voor de factureringsperiode, een factuurnummer, betalingsvoorwaarden (net 60 dagen) en betalingswijzen voor facturering die per overboeking of cheque moeten worden betaald.

- **Pagina 2 (en alle volgende pagina's) van de factuur:** Details van de kosten voor zowel eigen Microsoft-aankopen als ISV-aankopen van derden (op basis van licenties) van de commerciële marketplace. U kunt aankopen op basis van ISV-licenties identificeren aan de **hand Publisher** regel onder elke productnaam. Het bijbehorende afstemmingsbestand biedt meer factureringsgegevens voor specifieke factuurkosten.

- **Laatste pagina van de factuur:** Als er kosten in rekening zijn gebracht voor Marketplace-producten op basis van licenties van een ISV, worden op deze laatste pagina meer details weergegeven over de naam en het adres van de ISV-uitgever.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tips over het lezen van uw afstemmingsbestand

Het **afstemmingsbestand Terugkerende** en eenmalige aankopen bevat verschillende kolommen met aanvullende details die zijn toe te schrijven aan de kosten in uw factuur. In **de kolom PublisherName** ziet u of de aankoop afkomstig is van Microsoft of van een externe ISV-uitgever.

Sommige kosten in uw afstemmingsbestand kunnen worden weergegeven met een kosten van $ 0. Dit kan het gevolg zijn van een ISV-aanbieding voor een gratis proefversie (meestal 30 of 60 dagen) of een Bring Your Own License-aanbieding.

In het geval van gratis proefversie biedt ISV het volgende:

- De gratis proefperiode dekt de kosten van het SaaS-product op basis van licenties van de ISV gedurende die periode. Er worden ook geen kosten in rekening gebracht voor het bijbehorende gebruik van de Azure-infrastructuur van dat SaaS-product.  Als u echter een ISV-aanbieding op basis van gebruik gebruikt, omvat de gratis proefversie niet de kosten van het onderliggende gebruik van de Azure-infrastructuur. In dit geval worden de gebruikskosten voor de Azure-infrastructuur weergegeven in een afzonderlijk Azure-afstemmingsbestand.

- Wanneer u voor uw klant een product koopt en implementeert dat in aanmerking komt voor een gratis proefversie, wordt de klant automatisch door de ISV-uitgever ingeschreven voor de gratis proefversie. De gratis proefperiode eindigt automatisch na de periode die is gedefinieerd door de ISV-uitgever. Nadat de periode is afgelopen, worden er kosten in rekening gebracht voor de klant. Dit betekent dat het afstemmingsbestand twee rijen kan weergeven voor een product dat in aanmerking komt voor een proefversie: een waarmee de proefperiode wordt bijhoudt en een waarin de betaalde aanbieding wordt bijhoudt (waarbij de kosten van $ 0 tot na het einde van de proefperiode worden weergegeven). Zodra de proefversie is beëindigd, worden er kosten weergegeven in de rij met de betaalde aanbieding. 

Zie Uw afstemmingsbestanden gebruiken voor meer informatie over wat [elke kolom vertegenwoordigt.](use-the-reconciliation-files.md) Zie ook [Typen facturering in Partner Center](./billing-basics.md)

## <a name="next-steps"></a>Volgende stappen

- [Commerciële marketplace-producten voor klanten beheren](csp-commercial-marketplace-manage.md)
- [Meer informatie over ondersteuning voor commerciële marketplace-producten](csp-commercial-marketplace-support.md)
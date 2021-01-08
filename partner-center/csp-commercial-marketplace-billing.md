---
title: Facturering voor commerciële Marketplace-Producten
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe facturering werkt voor ISV SaaS-producten of-abonnementen die zijn aangeschaft voor klanten van de commerciële Marketplace binnen het partner centrum.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 10592c7f8a3b1f075bc726161603859552b29961
ms.sourcegitcommit: a78dd3c532860d01867d116bfb4e2c88b84bcd25
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 01/08/2021
ms.locfileid: "97979529"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Facturering voor commerciële Marketplace-Producten en-abonnementen in partner centrum


**Juiste rollen**

- Globale beheerder
- Factureringsbeheerder

Als partner in het CSP-programma kunt u het partner centrum gebruiken om SaaS-producten op basis van licenties te kopen van ISV-uitgevers in de commerciële Marketplace. Nadat u dit hebt gedaan, kunt u toegang krijgen tot een factuur voor dit soort aankopen. De facturerings periode begint op de eerste dag van de kalender maand en eindigt op de laatste dag van de kalender maand. Facturen worden beschikbaar gesteld op de achtste dag van de volgende maand.

U kunt facturen openen via het [dash board](https://partner.microsoft.com/dashboard/) van de partner centrum of via [Partner Center-api's](/partner-center/develop/).

Partners in het CSP-programma worden gefactureerd voor ISV-commerciële Marketplace-oplossingen die zijn aangeschaft voor een klant, wanneer ze deze producten aanschaffen bij een partner centrum of vanuit de Azure Portal (met de vooraf aangeschafte Azure-Tenant voor CSP van de klant).

>[!NOTE]
>Als klanten hun eigen Azure AD-Tenant gebruiken (niet één gekocht bij een partner in het CSP-programma), kunnen klanten er ook voor kiezen om rechtstreeks vanuit ([Microsoft AppSource](https://appsource.microsoft.com/) of [Azure Marketplace](https://azuremarketplace.microsoft.com/)) hun eigen ISV-oplossing te kopen. Als dit het geval is, ontvangen ze hun eigen factuur rechtstreeks van micro soft. En als een partner in het CSP-programma een Azure-abonnement of het nieuwe Azure-plan aan de klant verkoopt en de [op rollen gebaseerde toegang van](/azure/role-based-access-control/built-in-roles) de klant (of indirecte wederverkoper) verleent aan die Tenant (waarbij elke rol aan de klant wordt toegewezen, behalve **lezer**), kan die klant (of indirecte wederverkoper) ook commerciële Marketplace-aanbiedingen kopen zonder voorafgaande goed keuring of melding aan de CSP In dergelijke gevallen waarschuwt micro soft partners in het CSP-programma over aankopen door hun klanten. Micro soft biedt echter een optioneel [Azure monitor](/azure/azure-monitor/platform/alerts-activity-log) -mechanisme dat u kunt gebruiken voor het instellen van waarschuwingen of meldingen over activiteiten in een Azure-abonnement.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Toegang tot facturerings gegevens voor producten voor commerciële Marketplace

De globale beheerder of facturerings beheerder van uw bedrijf ontvangt een e-mail wanneer een factuur gereed is om te worden weer gegeven. Voor toegang tot het meest recente factuur-en afstemmings bestand voor product aankopen voor commerciële Marketplace:

1. Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard/)van de partner centrum.

2. Selecteer **facturering** in het menu van het partner centrum. 

    Boven aan de facturerings pagina ziet u twee tabbladen: **terugkerende** en **terugkerende en eenmalige aankopen**. Op elk tabblad kunt u toegang krijgen tot factuur-en afstemmings bestanden voor verschillende Marketplace-Producten:

    - **Terugkerend** tabblad: toont factuur-en afstemmings bestanden voor abonnementen die betrekking hebben op Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, Power BI Pro en Microsoft Azure.

    - Het tabblad **terugkerende en eenmalige aankopen** : toont de factuur-en reconciliatie bestanden voor Azure-abonnement, Azure-reserve ringen, software-en commerciële Marketplace-producten.
  
3. Selecteer het tabblad **terugkerend en eenmalige aankopen** . Als u abonnementen hebt gekocht voor een klant in een andere valuta, ziet u een tabblad voor elke valuta. U kunt een paar dingen doen: om deze pagina:

    - Selecteer **factuur** of **afstemmings bestand** om het laatste factuur-en reconciliatie bestand te bekijken. (Indien gewenst, hebt u ook toegang tot de laatste factuur en kunt u bestands gegevens afstemmen met behulp van [Partner Center-api's](/partner-center/develop/).

    - Als u eerdere facturen wilt bekijken en bestanden wilt afstemmen, vouwt u de rij **facturerings geschiedenis** hieronder uit.

    - Selecteer een koppeling onder de kop **schattingen** om het geschatte account saldo of de factuur op elk gewenst moment te controleren op basis van de meest recente account activiteit.  

    >[!NOTE]
    > Wanneer we uw factuur op de achtste dag van de maand plaatsen, worden belastingen en eventuele andere toepasselijke kosten en tegoeden vermeld. Dit betekent dat het uiteindelijke verschuldigde bedrag mogelijk afwijkt van wat u tijdens de facturerings periode ziet.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Meer informatie over facturen en afstemmings bestanden voor commerciële Marketplace-Producten

In deze sectie vindt u meer informatie over de factuur-en afstemmings bestanden voor door de klant aangeschafte SaaS-abonnementen voor commerciële Marketplace.

Wanneer u **terugkerende en eenmalige aankopen** selecteert via de optie **facturering** in het menu van het partner centrum, hebt u toegang tot facturen en afstemmings bestanden voor kosten met betrekking tot de aanschaf van zowel micro soft (eerste partij) als ISV (derden). Deze aankopen kunnen worden gekoppeld aan:

- SaaS-abonnementen (van micro soft of ISV-uitgevers)

- Azure-abonnement

- Azure-reserveringen

- Andere software op basis van een abonnement (van micro soft of ISV-uitgevers)

Voor beelden van deze aankopen zijn onder andere SUSE Linux-software (een software abonnement) of een Azure ISV SaaS-product abonnement.

>[!NOTE]
> Zie ook factuur [overzicht](billing.md)voor meer informatie over het lezen van factuur-en afstemmings bestanden.

### <a name="tips-on-reading-your-invoice"></a>Tips voor het lezen van uw factuur

Wanneer u een SaaS-product op basis van een licentie aanschaft vanuit een ISV-Uitgever van een derde partij, worden er alleen kosten in rekening gebracht voor de licentie kosten op uw factuur. Dit geldt zelfs wanneer het SaaS-product van de ISV de onderliggende Azure-infrastructuur resources gebruikt (of gebruikt). Dat komt doordat de gebruiks kosten van de Azure-infra structuur van de klant voor een SaaS-product van een ISV rechtstreeks worden gefactureerd aan de ISV. (Isv's zien de gekoppelde verbruiks kosten van Azure in hun eigen Azure-gebruik van een factuur afstemmings bestand.)

Uw factuur bevat verschillende pagina's:

- **Pagina 1 van de factuur:** Bevat een overzicht van de facturerings gegevens van het CSP-programma partner. Dit omvat een samen vatting van de kosten voor de facturerings periode, een factuur nummer, betalings voorwaarden (netto 60 dagen) en facturerings methoden om per telegram of per cheque te betalen.

- **Pagina 2 (en eventuele volgende pagina's) van de factuur:** Details van de kosten voor micro soft-aankopen en onafhankelijke software leveranciers van derden (op basis van licenties) van de commerciële Marketplace. U kunt op ISV-licenties gebaseerde aankopen identificeren op de **Uitgever** regel onder elke product naam. Het bijbehorende afstemmings bestand bevat meer facturerings gegevens voor specifieke factuur kosten.

- **Laatste pagina van de factuur:** Als u in rekening wordt gebracht voor Marketplace-producten op basis van licenties van een ISV, wordt op deze laatste pagina meer informatie over de naam en het adres van de ISV-Uitgever weer gegeven.

### <a name="tips-on-reading-your-reconciliation-file"></a>Tips voor het lezen van het afstemmings bestand

Het **periodieke en eenmalige aankoop** afstemmings bestand bevat verschillende kolommen met aanvullende details die zijn gekoppeld aan de kosten in uw factuur. De kolom **Uitgever** naam toont of de aanschaf van micro soft of van een ISV-Uitgever van een derde partij is.

Sommige kosten in het afstemmings bestand kunnen worden weer gegeven met een prijs van $0. Dit kan worden veroorzaakt door een ISV-aanbieding (een gratis proef versie van 30 of 60 dagen) of een aanbieding van uw eigen licentie.

In het geval van ISV-aanbiedingen voor een gratis proef versie:

- De gratis proef periode heeft betrekking op de kosten van het SaaS-product op basis van licenties van de ISV tijdens die tijd. Er worden ook geen kosten in rekening gebracht voor het gebruik van de betreffende Azure-infra structuur van dat SaaS-product.  Als u een ISV-aanbieding op basis van gebruik gebruikt, bevat de gratis proef versie echter niet de kosten voor het gebruik van de onderliggende Azure-infra structuur. In dit geval worden de gebruiks kosten voor Azure-infra structuur weer gegeven in een afzonderlijk Azure-afstemmings bestand.

- Wanneer u een gratis proef versie van een ISV-product aanschaft en implementeert voor uw klant, wordt de klant automatisch Inge schreven bij de gratis proef versie door de ISV-Uitgever. De gratis proef periode eindigt automatisch na de periode die is gedefinieerd door de ISV-Uitgever. Na afloop van de periode wordt de klant in rekening gebracht. Dit betekent dat het afstemmings bestand twee rijen kan weer geven voor een product waarvoor een proef versie in aanmerking komt: een voor de proef periode en een die de betaalde aanbieding bijhoudt (waarbij de kosten van $0 worden weer gegeven nadat de proef periode is afgelopen). Zodra de proef versie is afgelopen, wordt in de rij met de betaalde aanbieding de kosten weer gegeven. 

Zie [uw reconciliatie bestanden gebruiken](use-the-reconciliation-files.md)voor meer informatie over wat elke kolom vertegenwoordigt. Zie ook [typen facturering in partner centrum](billing-different-types.md)

## <a name="next-steps"></a>Volgende stappen

- [Commerciële Marketplace-Producten voor klanten beheren](csp-commercial-marketplace-manage.md)
- [Meer informatie over ondersteuning voor commerciële Marketplace-Producten](csp-commercial-marketplace-support.md)
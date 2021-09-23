---
title: On-premises software verkopen via CSP
ms.topic: how-to
ms.date: 03/08/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Ontdek hoe partners in het CSP-programma on-premises softwareabonnementen kunnen kopen, beheren, verkopen en annuleren namens klanten in Partner Center.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: f58f120d376b98f9fa054f0bec87f324874ce0bb
ms.sourcegitcommit: fceaca54b0ec695cf214209c09b4516e1b40866a
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/23/2021
ms.locfileid: "128322081"
---
# <a name="sell-on-premises-software-through-the-cloud-solution-provider-csp-program"></a>On-premises software verkopen via het Cloud Solution Provider (CSP)-programma

**Juiste rollen:** beheeragent | Globale beheerder

On-premises software in CSP ondersteunt een soepele overgang naar de cloud door de introductie van on-premises software in een cloudgericht programma. Deze nieuwe aanbieding helpt de toegevoegde waarde van de partner bij elk aankoopscenario te brengen, omdat deze één platform biedt voor het transacten van alle Microsoft-producten. Als CSP kunt u nu on-premises software verkopen via Partner Center naast Open, EA en andere programma's die momenteel in gebruik zijn.  
 
Hoewel we de beste algemene klantwaarde met on-premises softwarelicentieopties garanderen, hebben we het bedrijfsmodel ook zo gebruiksvriendelijk mogelijk gemaakt. Eenvoudige licentieverlening van on-premises software in CSP betekent kostenvoorspeller en een gestroomlijnd verkoopproces voor u. Met dit nieuwe bedrijfsmodel kunt u eenvoudig on-premises software aanschaffen, beheren en prijzen voor uw klanten, zodat u zich kunt richten op het winnen van uw bedrijf met een uitgebreide portfolio met oplossingen met toegevoegde waarde voor IT-beheer.

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a>Softwareabonnementen kopen namens klanten

Als u softwareabonnementen namens een klant wilt kopen, gaat u naar de detailpagina van de klant, selecteert u Producten toevoegen en volgt u vervolgens de instructies op het scherm om uw bestelling te maken en te betalen.

> [!NOTE]
> Zie voor meer informatie deze handleiding [voor bestellen en afhandeling via Partner Center.](https://partner.microsoft.com/resources/detail/guide-to-ordering-and-fulfillment-through-partner-center-pdf)

## <a name="activate-and-manage-software-subscriptions"></a>Software-abonnementen activeren en beheren

Nadat u uw software hebt aangeschaft, moeten u of uw klanten deze downloaden (partners die Partner Center; klanten die het Microsoft 365-beheer Center gebruiken). Gebruik de volgende procedure om dit te doen. Het is belangrijk om inzicht te krijgen in de risico's die gepaard gaan met het kopiëren van koppelingen en het downloaden van software. Zie Using Partner Center to obtain customer **software downloads and license keys** in de Partner Center New Commerce Operations Guide voor meer [informatie.](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf)

> [!NOTE]
> U moet een beheerderagent in Partner Center om de koppeling naar sleutels en downloads te verkrijgen.

1. Ga naar de detailpagina van uw klant en selecteer **Software**. U ziet een lijst met alle software die u namens de klant hebt aangeschaft.

2. Kies **productversie,** **taal**, **bit** en selecteer **Sleutels en downloads ophalen.** 

3. Kies **Sleutel op** halen waarmee het 32-cijferige product wordt weergegeven in een pop-updialoogdialoog dat u kunt kopiëren en verzenden naar de klant. 

4. Kies **Downloaden om** de bits te downloaden. 

5. Kies **Koppeling kopiëren** als u de klant de koppeling naar de bits download wilt sturen. 

6. U kunt ook **de** softwareorder annuleren en een tegoed van 100% ontvangen (indien uitgevoerd binnen de annuleringsbeleidsperiode van 60 dagen).

> [!NOTE]
> Alleen klanten hebben toegang tot de productcodes en het downloaden van informatie in Microsoft 365-beheer Center (globale beheerdersrol vereist). Partners moeten deze Partner Center gebruiken om deze informatie te bekijken.

> [!NOTE]
> CSP-aankopen worden geactiveerd via een MULTIPLE Activation Key (MAK). Key Management Service sleutels (KMS) zijn niet toegestaan, zelfs niet op aanvraag. 

## <a name="move-a-customers-on-premises-license-from-vl-to-csp-with-no-downtime"></a>De on-premises licentie van een klant zonder downtime verplaatsen van VL naar CSP

Hoewel KMS sleutels niet beschikbaar zijn in CSP, kunt u nog steeds de on-premises licenties van uw klant van VL naar CSP verplaatsen en downtime voorkomen als gevolg van de schakelaar voor het aankoopkanaal. KMS licenties distribueert naar de clients en ze blijven meestal 180 dagen actief voordat het apparaat die activering probeert te vernieuwen. Dit betekent dat het apparaat al is geactiveerd en enige tijd actief is voordat er problemen optreden. 

Als de klant gedurende deze tijd de nieuwe MAK implementeert, handmatig of via een script (met ), treedt `slmgr.vbs` er geen downtime op. Als de klant de nieuwe MAK gedurende deze tijd niet implementeert en later probeert de licentie te verlengen, kan het apparaat in sommige functies worden beperkt of geblokkeerd totdat het opnieuw wordt geactiveerd. 

Ga voor meer informatie naar [Clients activeren met Windows 10 (Windows 10) - Windows Deployment](/windows/deployment/volume-activation/activate-windows-10-clients-vamt#key-management-service-activation-renewal). Voor hulp bij dit type implementatie kunt u een aanvraag voor technische [presales-](/partner-center/technical-benefits#submit-a-technical-presales-and-deployment-services-request) en implementatieservices indienen.

## <a name="cancel-a-purchase"></a>Een aankoop annuleren

Gebruik de volgende procedure om een aankoop te annuleren. Zodra de annulering is voltooid, wordt de softwaresleutel ingetrokken.

> [!NOTE]
> U moet een beheerderagent zijn om een aankoop te annuleren. 

1.  Voordat u met het proces begint, moet u ervoor zorgen dat u het volgende hebt: 
    - De GUID of domeinnaam van de tenant van de klant
    - Order-id of abonnements-id
    - Reden van restitutie
    - Gevraagd bedrag

2.  Selecteer software op de pagina met details van **de klant.** U ziet een lijst met alle software die u hebt aangeschaft. 

3.  Zoek de software die u wilt annuleren en selecteer **Annuleren.** De **pagina Een probleem met Partner Center** melden wordt geopend. 

4.  Selecteer **onder Details** in de lijst Type **probleem** de optie **CSP-aankoop/-restitutie namens klanten**.

5.  Vul de velden **Impact** en **Titel** in. 

6.  Geef in **het** veld Beschrijving het volgende op: 
    -   De GUID of domeinnaam van de tenant van de klant
    -   Order-id of abonnements-id
    -   Reden van restitutie
    -   Gevraagd bedrag

7.  Voer in **het** veld Contactpersoon uw naam, e-mailadres en telefoonnummer in. 

8.  Als u om wat voor reden dan ook een bestand wilt bijvoegen, **selecteert u Bestanden toevoegen.** Deze stap is optioneel. 

9.  Wanneer u klaar bent, selecteert u **Verzenden.**

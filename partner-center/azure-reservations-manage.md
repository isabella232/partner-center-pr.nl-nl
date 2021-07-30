---
title: Azure-reserveringen voor klanten beheren
description: Meer informatie over het beheren van Azure-reserveringen voor een klant, waaronder het annuleren van een reservering, het inruilen van een reservering of het aanvragen van een restitutie.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: 627c6f8d09a904e7d988c4229ec10eeac38dc2e9
ms.sourcegitcommit: ad1af627f5ee6b6e3a70655f90927e932cf4c985
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 07/29/2021
ms.locfileid: "114841467"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Reserveringen voor klanten beheren, annuleren, inruilen Microsoft Azure restitutie

**Juiste rollen:** beheeragent | Globale beheerders | Helpdeskagent | Verkoopagent | Beheerder van gebruikersbeheer

In dit artikel wordt uitgelegd hoe u Azure-reserveringen voor een klant beheert, waaronder hoe u een reservering annuleert, een reservering inwisselt of een restitutie aanvraagt.

> [!NOTE]
> Dit artikel is alleen van toepassing op partners in het Cloud Solution Provider (CSP)-programma. Klanten die gebruikmaken van andere typen abonnementen (zoals betalen per gebruik, individueel, Microsoft-klantovereenkomst- of Enterprise Agreement-abonnementen), moeten in plaats daarvan deze documentatie voor [Azure-reserveringen lezen.](/azure/cost-management-billing/reservations)

Als u de Azure-reserveringen van uw klanten na aankoop wilt beheren, selecteert u de klant en reservering die u wilt beheren in Partner Center en wijzigt u vervolgens de reservering in de Azure Portal.

1. Om aan de slag **te** gaan, selecteert u Klanten in Partner Center menu en selecteert u vervolgens de klant waarvan u de reserveringen wilt beheren. 

2. Selecteer azure-reserveringen in het menu van de detailpagina **van** de klant en selecteer vervolgens de specifieke reservering die u wilt beheren.  

3. Selecteer **beheren** onder Acties **om** naar de reserveringsrecord van de klant in de Azure Portal. Volg op de pagina met reserveringsdetails de onderstaande stappen om taken uit te voeren.  

    | **Selecteren**   | **Aan**    |
    |:-----------------------------|:-----------------|
    | **Overzicht**   | Bekijk details van de reservering van een klant, inclusief verloopdatum, bereik en gebruiksgegevens. **OPMERKING** Selecteer **Restitutie** om een ondersteuningsaanvraag voor een restitutie naar eigen goed tarief te maken. Selecteer **Exchange** om een ondersteuningsaanvraag te maken om het ongebruikte gedeelte van uw reserveringstermijn in te wisselen.  
    | **Access Control (IAM)**   | Toegang tot de reserveringsgegevens van de klant beheren.|
    | **Configuratie**   | Wijzig het bereik van de reservering en/of het Azure-abonnement waar de reservering aan is gekoppeld.    |
    | **Eigenschappen**   | Bekijk de eigenschappen van de reservering en kopieer de reserverings-id en reserveringsorder-id naar het klembord. **OPMERKING** Ondersteuning kan u om de reserverings-id en reserveringsorder-id vragen wanneer u ondersteuning namens een klant aanvraagt.    |
    | **Nieuwe ondersteuningsaanvraag**    | Vraag hulp aan Microsoft-ondersteuning.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Een reservering annuleren of inruilen

Als het bedrijf van een klant op enig moment moet worden gewijzigd, kan het zijn dat hij een reservering wil annuleren en een restitutie wil krijgen of het restitutiebedrag van een reservering wil inruilen om te worden gebruikt voor de prijs van een nieuwe reservering.

In beide scenario's wordt het bedrag door Microsoft aan u terugbetaald, zodat u vervolgens de resulterende financiële transacties met uw klanten kunt beheren. Microsoft neemt niet rechtstreeks contact op met klanten over facturering, annuleringen of restituties.

### <a name="how-cancellations-work"></a>Hoe annuleringen werken

Klanten kunnen op elk moment een aanvraag indienen om een reservering te annuleren (restitutiebedrag van $ 50.000 per jaar). Door een reservering te annuleren, kan de klant het bedrag van de resterende maanden van een Azure-reservering retourneren tegen kosten voor vroegtijdige beëindiging. Het resterende prorated balance, minus de kosten voor vroegtijdige beëindiging, wordt gerestitueerd naar uw account, zodat u de restitutie voor het account van de klant kunt krijgen. 

Zie hieronder voor annuleringsdetails en kosten.


|**Annuleringsdatum**<br> (dagen)   |**Gebruik**    |**Tegoed**  |**Vroegtijdige beëindiging**<br> Vergoeding    |**Restitutielimiet** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 of minder                         | Nee          | 100%       | Nee                              | $ 50.000 USD   |
|5 of minder                         | Ja         | Pro beoordeeld  | Nee                              | $ 50.000 USD   |
|Meer dan 5                        | Nee          | Pro beoordeeld  | 12%                             | $ 50.000 USD   |
|Meer dan 5                        | Ja         | Pro beoordeeld  | 12%                             | $ 50.000 USD   |

### <a name="how-exchanges-work"></a>Hoe exchanges werken 

Als een klant een andere reservering wil kopen dan de reservering die hij oorspronkelijk van u heeft gekocht, kan deze een inwisseling aanvragen. Het uitwisselen van een reservering kan een aantrekkelijk alternatief zijn voor het annuleren van een reservering, omdat de klant hiermee het restitutiebedrag naar meer dan de prijs van de nieuwe reservering kan gebruiken. 

Het restitutiebedrag naar pro 1 wordt bijgeschreven op uw account, zodat u de klant een inwisseling kunt aanbieden.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Een restitutie of uitwisseling aanvragen namens een klant

Als u een ondersteuningsaanvraag voor een restitutie of uitwisseling namens uw klanten wilt indienen, selecteert u de klant en de reservering in Partner Center en maakt u vervolgens de ondersteuningsaanvraag in de Azure Portal. 

>[!NOTE]
>Microsoft-ondersteuning kunnen u vragen om de reserverings-id en reserveringsorder-id op te geven. U vindt deze informatie op de pagina Eigenschappen **van de** reservering in de Azure Portal.

1. Om aan de slag te **gaan,** selecteert u Klanten in Partner Center menu en selecteert u vervolgens de klant die een restitutie wil. 

2. Selecteer azure-reserveringen op de detailpagina van de klant **en** selecteer vervolgens de specifieke reservering die de klant wil laten restitutie.  

3. Selecteer **onder Acties** de optie **Restitutie** om naar de reserveringsrecord van de klant in de Azure Portal te gaan en een ondersteuningsaanvraag te initiëren.  

4. Volg op **de pagina Nieuwe ondersteuningsaanvraag** de onderstaande stappen om een restitutie aan te vragen. Selecteer **Volgende** na elke stap. 

   |**Stap**                    |**Selecties**    |
   |:---------------------------|:-----------------|
   |**1 Basisbeginselen**                |Type probleem: Facturering.  |
   |**2 Probleem**               |Probleemtype: Reserveringsbeheer. Categorie: Omruilen en restituties. |
   |**3 Contactgegevens**   |Selecteer uw voorkeuren en voer de vereiste gegevens in. 

5. Selecteer **Maken** wanneer u klaar bent.

## <a name="azure-reservations-resources"></a>Resources voor Azure-reserveringen

|**Voor informatie over**   |**Leest u**    |
|:-----------------------------|:-----------------|
|Overzicht van Azure-reserveringen in CSP  | [Verkopen Microsoft Azure gereserveerde instanties](azure-reservations.md) |
|Azure-reserveringen kopen voor uw klanten in Partner Center   | [Azure-reserveringen kopen](azure-reservations-buying.md) |
|De juiste VM-grootte bepalen en het gebruik van de klant-VM controleren   | [VM-formaat voor maximaal azure-reserveringsgebruik](azure-usage.md)   |
|Azure-reserveringen kopen met behulp van Partner Center API | [Aankoop van Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in de documentatie Partner Center ontwikkelaars   |
|Klanten toestemming geven om hun eigen Azure-reserveringen te kopen bij een abonnement dat u voor hen hebt aangeschaft. | [Klanten toestemming geven om hun eigen Azure-reserveringen te kopen](give-customers-permission.md)   |
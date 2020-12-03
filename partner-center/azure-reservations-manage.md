---
title: Azure-reserve ringen voor klanten beheren
description: Meer informatie over het beheren van Azure-reserve ringen voor een klant, inclusief het annuleren van een reserve ring, het afvragen van een reserve ring of het aanvragen van een restitutie.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 08/06/2020
ms.openlocfilehash: c377fca3e38161258c836d14202ac4db21484526
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534757"
---
# <a name="manage-cancel-exchange-or-refund-microsoft-azure-reservations-for-customers"></a>Microsoft Azure reserve ringen voor klanten beheren, annuleren, uitwisselen of terugbetalen

**Juiste rollen**

- Beheer agent
- Globale beheerder
- Helpdesk medewerker
- Verkoop agent
- Beheerder van gebruikers beheer

In dit artikel wordt uitgelegd hoe u Azure-reserve ringen voor een klant beheert, met inbegrip van het annuleren van een reserve ring, het omruilen van een reserve ring of het aanvragen van een restitutie.

> [!NOTE]
> Dit artikel is alleen van toepassing op partners in het Cloud Solution Provider-programma (CSP). Klanten die andere soorten abonnementen gebruiken (zoals betalen per gebruik, individuele, micro soft-klant overeenkomst of Enterprise Agreement-abonnementen), moeten in plaats daarvan [deze Azure rehanden documentatie](/azure/cost-management-billing/reservations)lezen.

Als u de Azure-reserve ringen van uw klanten wilt beheren, selecteert u de klant en de reserve ring die u wilt beheren in partner centrum en brengt u wijzigingen aan in de reserve ring in de Azure Portal.

1. Als u aan de slag wilt gaan, selecteert u **klanten** in het menu van het partner centrum en selecteert u vervolgens de klant van wie u de reserve ringen wilt beheren. 

2. Selecteer in het menu detail pagina van de klant **Azure-reserve ringen** en selecteer vervolgens de specifieke reserve ring die u wilt beheren.  

3. Selecteer **beheren** onder **acties** om naar de reserverings record van de klant te gaan in de Azure Portal. Volg de onderstaande stappen op de pagina reserverings details om de taken uit te voeren.  

    | **Selecteren**   | **Aan**    |
    |:-----------------------------|:-----------------|
    | **Overzicht**   | Details weer geven van de reserve ring van een klant, inclusief verval datum, bereik en gebruiks gegevens. **Opmerking** Selecteer **terugbetaling** om een ondersteunings aanvraag te maken voor een pro-rating restitutie. Selecteer **Exchange** om een ondersteunings aanvraag te maken om het ongebruikte deel van uw reserverings termijn uit te wisselen.  
    | **Access Control (IAM)**   | De toegang tot de reserverings gegevens van de klant beheren.|
    | **Configuratie**   | Wijzig het bereik van de reserve ring en/of het Azure-abonnement waaraan de reserve ring is gekoppeld.    |
    | **Eigenschappen**   | Bekijk de eigenschappen van de reserve ring en kopieer de reserverings-id en de reserverings Order-ID naar het klem bord. **Opmerking** Ondersteuning kan u vragen om de reserverings-ID en de reserverings Order-ID wanneer u ondersteuning voor namens een klant aanvraagt.    |
    | **Nieuwe ondersteuningsaanvraag**    | Hulp vragen bij Microsoft Ondersteuning.   |
 
## <a name="cancel-or-exchange-a-reservation"></a>Een reserve ring annuleren of uitwisselen

Als de bedrijfs behoeften van een klant op elk moment veranderen, willen ze mogelijk een reserve ring annuleren en een restitutie ontvangen, of de verschuldigde restitutie van een reserve ring uitwisselen zodat deze kan worden gebruikt voor de prijs van een nieuwe reserve ring.

In beide scenario's heeft micro soft het bedrag terugbetaald zodat u vervolgens de resulterende financiële trans acties kunt beheren met uw klanten. Micro soft neemt niet rechtstreeks contact op met klanten met betrekking tot facturering, annuleringen of restituties.

### <a name="how-cancellations-work"></a>Hoe annuleringen werken

Klanten kunnen aanvragen om op elk gewenst moment een reserve ring te annuleren (restitutie bedrag beperkt tot $50.000 per jaar). Als u een reserve ring annuleert, kan de klant het bedrag van de resterende maanden van een Azure-reserve ring retour neren voor een vroegtijdige beëindigings vergoeding. Het resterende tarief saldo, min de kosten voor vroegtijdige beëindiging, wordt terugbetaald aan uw account, zodat u het account van de klant kunt terugbetalen. 

Hieronder vindt u meer informatie over de annulering en de kosten.


|**Annulerings datum**<br> resterende   |**Gebruik**    |**Tegoed**  |**Vroege beëindiging**<br> taksen    |**Restitutie limiet** | 
|:----------------------------------|:------------|:-----------|:--------------------------------|:--------------|
|5 of minder                         | Nee          | 100%       | Nee                              | $50.000 USD   |
|5 of minder                         | Ja         | Pro-beoordeeld  | Nee                              | $50.000 USD   |
|Meer dan 5                        | Nee          | Pro-beoordeeld  | 12%                             | $50.000 USD   |
|Meer dan 5                        | Ja         | Pro-beoordeeld  | 12%                             | $50.000 USD   |

### <a name="how-exchanges-work"></a>Hoe uitwisselingen werken 

Als een klant een andere reserve ring wil kopen dan het account dat oorspronkelijk door u is gekocht, kunnen ze een uitwisseling aanvragen. Het uitwisselen van een reserve ring kan een aantrekkelijk alternatief zijn voor het annuleren van een reserve ring omdat de klant het bedrag van de gefactureerde restitutie kan gebruiken voor de prijs van de nieuwe reserve ring. 

Het bedrag van de evenredige restitutie wordt gecrediteerd aan uw account, zodat u de klant een uitwisseling kunt aanbieden.

## <a name="request-a-refund-or-exchange-on-behalf-of-a-customer"></a>Een terugbetaling of uitwisseling aanvragen namens een klant

Als u een ondersteunings aanvraag wilt indienen voor een terugbetaling of uitwisseling namens uw klanten, selecteert u de klant en de reserve ring in partner centrum en maakt u de ondersteunings aanvraag in de Azure Portal. 

>[!NOTE]
>Microsoft Ondersteuning agents kunnen u vragen de reserverings-ID en de reserverings Order-ID op te geven. U kunt deze informatie vinden op de **Eigenschappen** pagina van de reserve ring in de Azure Portal.

1. Als u aan de slag wilt gaan, selecteert u **klanten** in het menu van het partner centrum en selecteert u vervolgens de klant die een terugbetaling wil. 

2. Selecteer **Azure-reserve ringen** op de detail pagina van de klant en selecteer vervolgens de specifieke reserve ring die de klant wil terugbetalen.  

3. Selecteer onder **acties** de optie **terugbetaling** om naar de reserverings record van de klant in de Azure portal te gaan en een ondersteunings aanvraag te initiëren.  

4. Voer op de pagina **nieuwe ondersteunings aanvraag** de volgende stappen uit om een restitutie aan te vragen. Selecteer **volgende** na elke stap. 

   |**Stap**                    |**Selecties**    |
   |:---------------------------|:-----------------|
   |**1 basis beginselen**                |Probleem type: facturering.  |
   |**2 probleem**               |Probleem type: reserverings beheer. Categorie: uitwisselingen en terugbetalingen. |
   |**3 contact gegevens**   |Selecteer uw voor keuren en voer de vereiste gegevens in. 

5. Selecteer **maken** wanneer u klaar bent.

## <a name="azure-reservations-resources"></a>Resources voor Azure-reserve ringen

|**Voor informatie over**   |**Leest u**    |
|:-----------------------------|:-----------------|
|Overzicht van Azure-reserve ringen in CSP  | [Gereserveerde instanties van Microsoft Azure verkopen](azure-reservations.md) |
|Azure-reserve ringen voor uw klanten kopen in het partner centrum   | [Azure-reserve ringen kopen](azure-reservations-buying.md) |
|Bepaal de juiste VM-grootte en controleer het gebruik van de virtuele machine van de klant   | [VM-grootte voor maximum gebruik van Azure-reserve ring](azure-usage.md)   |
|Azure-reserve ringen aanschaffen met de Partner Center-API | [Azure reserved VM instances kopen](/partner-center/develop/purchase-azure-reservations) in de ontwikkelaars documentatie van partner Center   |
|Klanten toestemming geven om hun eigen Azure-reserve ringen te kopen vanuit een abonnement dat u hebt aangeschaft. | [Geef klanten toestemming om hun eigen Azure-reserve ringen te kopen](give-customers-permission.md)   |
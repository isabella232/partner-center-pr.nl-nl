---
title: Reserveringsreserveringen Microsoft Azure klanten kopen
description: Meer informatie over het kopen of kopen van Azure-reserveringen namens uw klanten in Partner Center. Toont ook markten waar Azure-reserveringen niet beschikbaar zijn.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.date: 08/06/2020
ms.openlocfilehash: 61ddb91e296436817e45ae0a2c3d9fe12b326f18
ms.sourcegitcommit: b78e85a0bc62e3536b067417cb3db7899cda4f97
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/06/2021
ms.locfileid: "129565288"
---
# <a name="buy-microsoft-azure-reservations-on-behalf-of-your-customers-in-partner-center"></a>Koop Microsoft Azure namens uw klanten in Partner Center

**Juiste rollen:** beheeragent | Globale beheerder | Helpdeskagent | Verkoopagent | Beheerder van gebruikersbeheer

In dit artikel wordt uitgelegd hoe u Azure-reserveringen namens uw klanten kunt kopen of kopen in Partner Center. Het identificeert ook markten waar Azure-reserveringen niet beschikbaar zijn.
 
> [!NOTE]
> Dit artikel is alleen van toepassing op partners in Cloud Solution Provider (CSP)-programma. Klanten die andere typen abonnementen gebruiken (zoals betalen per gebruik, afzonderlijke, Microsoft-klantovereenkomst- of Enterprise Agreement-abonnementen), moeten in plaats daarvan deze documentatie voor [Azure-reserveringen lezen.](/azure/cost-management-billing/reservations)

## <a name="before-you-begin"></a>Voordat u begint

Lees de belangrijke informatie hieronder voordat u Azure-reserveringen namens uw klanten koopt. (Wilt u dat klanten hun eigen Azure-reserveringen kunnen kopen bij een eerder Azure-abonnement dat u voor hen hebt gekocht? Zie [Klanten toestemming geven om hun eigen Azure-reserveringen te kopen.)](give-customers-permission.md#give-customers-permission-to-buy-their-own-azure-reservations)

- Als en wanneer uw klant de nieuwe Microsoft-klantovereenkomst (zie Acceptatie van de [Microsoft-klantovereenkomst](confirm-customer-agreement.md)door de klant bevestigen), moet u Azure-reserveringen aanschaffen onder het Azure-plan. Lees [Azure-abonnement aanschaffen voor meer informatie.](purchase-azure-plan.md)

- Klanten moeten al een actief Azure-abonnement hebben voordat u namens hen reserveringen kunt kopen
  
- Kosten voor softwareabonnementen, zoals SQL Database of SUSE Linux-software, zijn niet inbegrepen in azure-reserveringsprijzen

- De commerciële prijzen van Microsoft omvatten geen belastingen, tenzij uw locatie Brazilië is. Als uw locatie Brazilië is, bevat de commerciële prijs aan u de juiste belastingen

- Verkoop- en helpdeskmedewerkers hebben expliciete toegang nodig tot het Azure-abonnement, zodat ze het kunnen kopen of beheren in de Azure Portal- en bestandsondersteuningsaanvragen, inclusief voor omruiling en restitutie namens de klant  

- Als u een indirecte provider bent en u Azure-reserveringen koopt via de Azure Portal, wordt de Partner of Record (indirecte reseller) overgenomen van het Azure CSP-abonnement dat u selecteert.

- De Partner of Record voor Azure-reserveringen kan na aankoop niet worden gewijzigd. U kunt de bestaande reservering annuleren en een nieuwe aanschaffen met de nieuwe Partner of Record.

- Als een klant een Azure-abonnement wil overdragen van Direct of EA naar CSP, worden reserveringen niet overgedragen.

## <a name="azure-reservations-unavailable-markets"></a>Niet-beschikbare markten voor Azure-reserveringen

> [!IMPORTANT]
> **Azure-reserveringen zijn niet** beschikbaar in de volgende markten:  
>  
> **Niet-beschikbare markten (in alfabetische volgorde)**
>
> |A naar Gi   | Gr naar Pal  | Pap naar Z |
> |--------------------------------|-----------------------------------|------------------------------------------|
> | Ålandeilanden     | Groenland     | Papoea-Nieuw-Guinea     |
> | Amerikaans-Samoa     | Grenada     | Pitcairneilanden     |
> | Andorra     | Guadeloupe     | Réunion     |
> | Anguilla     | Guam     | Saba   |
> | Antarctica     | Guernsey     | Saint Barthélemy   |
> | Antigua en Barbuda       | Guinee     | Saint Lucia   |
> | Aruba       | Guinee-Bissau     | Saint-Martin   |
> | Azerbeidzjan       | Guyana     | Saint-Pierre en Miquelon   |
> | Benin     | Haïti       | Saint Vincent en de Grenadines     |
> | Bhutan     | Heard- en McDonald-eilanden       | Samoa     |
> | Bonaire     | Isle of Man     | San Marino     |
> | Bouveteiland     | Jan Mayen     | Sño Toñ en Prñncipe   |
> | Brits Territorium in de Indische Oceaan       | Jersey     | Seychellen   |
> | Britse Maagdeneilanden     | Kiribati       | Sierra Leone   |
> | Burkina Faso     | Kosovo     | Sint Eustatius     |
> | Burundi     | Laos     | Sint Maarten     |
> | Cambodja     | Lesotho     | Salomonseilanden     |
> | Centraal-Afrikaanse Republiek     | Liberia     | Somalië     |
> | Tsjaad     | Madagaskar     | Zuid-Georgië en de Zuidelijke Sandwicheilanden     |
> | China     | Malawi     | Zuid-Soedan     |
> | Christmaseiland     | Maldiven     | St Helena, Ascension, Tristan da Cunha     |
> | Cocoseilanden     | Mali     | Suriname     |
> | Comoren     | Marshalleilanden     | Svalbard     |
> | Congo     | Martinique     | Swaziland     |
> | Congo (DRC)     | Mauritanië     | Timor-Leste   |
> | Cookeilanden     | Mayotte     | Togo   |
> | Djibouti     | Micronesia     | Tokelau   |
> | Dominica     | Montserrat     | Tonga   |
> | Equatoriaal-Guinea     | Mozambique     | Turks- en Caicos-eilanden   |
> | Eritrea     | Myanmar     | Tuvalu   |
> | Falklandeilanden     | Nauru     | Amerikaanse outlyingeilanden   |
> | Frans-Guyana     | Nieuw-Caledonië     | Vanuatu   |
> | Frans-Polynesië     | Niger     | Vaticaanstad   |
> | Franse Gebieden in de zuidelijke Indische Oceaan     | Niue     | Wallis en Walluna   |
> | Gabon     | Norfolk     | Jemen   |
> | Gambia     | Noordelijke Marianen     |    |
> | Gibraltar     | Palau       |    |

## <a name="purchase-azure-reservations"></a>Azure-reserveringen kopen

Volg de onderstaande stappen om Microsoft Azure namens uw klanten te kopen in Partner Center. (Wilt u dat klanten hun eigen Azure-reserveringen kunnen kopen bij een eerder Azure-abonnement dat u voor hen hebt gekocht? Zie [Klanten toestemming geven om hun eigen Azure-reserveringen te kopen.)](give-customers-permission.md)

1. Selecteer **Klanten** in het Partner Center menu.  

2. Zoek op **de** pagina Klanten de klant die Azure-reserveringen wil aanschaffen en selecteer vervolgens de pijl-omlaag om de rij van de klant uit te vouwen.  

3. Selecteer **Producten toevoegen** en selecteer vervolgens **Azure**. 

    a. Kies het marktsegment van de klant in de **lijst Segment.**

    b. Kies **Reserveringen in** de lijst **producttype.**

    c. Kies in de lijst **Reserveringstype** het type reservering dat de klant wil.

4. Azure-reserveringen moeten zijn gekoppeld aan een actief Azure-abonnement. Kies in de lijst Klantabonnement het abonnement van de klant aan wie u **Azure-reserveringen wilt** toevoegen. 

   >[!IMPORTANT]
   >Als de klant nog geen actief Azure-abonnement heeft, selecteert u **Azure om** er nu een toe te voegen. 

5. Gebruik de filters om Azure-reserveringen te vinden op virtuele machines die voldoen aan de vereisten van uw klant.  

6. Nadat u de reservering(en) hebt gevonden die u wilt kopen, voert u het aantal gereserveerde instanties in dat de klant nodig heeft **in** Hoeveelheid en selecteert u vervolgens Toevoegen **aan winkelwagen.**  

7. Herhaal stap 5 en 6 totdat u alle benodigde items aan de order hebt toegevoegd. Selecteer **Controleren** om te controleren of uw bestelling juist is.  

8. Op de **pagina Uw orders** controleren kunt u het volgende doen: 

    - Controleer of wijzig de hoeveelheid gereserveerde instanties.

    - Selecteer het bereik van de reservering. Het bereik van de reservering kan betrekking hebben op één abonnement of meerdere abonnementen (gedeeld bereik). Als u de reservering beperkt tot één abonnement, wordt de reserveringskorting alleen toegepast op dit abonnement. Als u Gedeeld selecteert, wordt de reserveringskorting toegepast op abonnementen binnen de factureringscontext van de klant. 

      > [!NOTE] 
      > Als u ervoor kiest om het bereik van de reservering te beperken tot één Azure-abonnement, moet u mogelijk het vCPU-quotum van het abonnement verhogen. Als u het vCPU-quotum van het abonnement wilt verhogen, moet u een ondersteuningsaanvraag maken in de Azure Portal. Volg de instructies [in dit onderwerp om](/azure/azure-supportability/resource-manager-core-quotas-request) de aanvraag te maken. 

      > [!NOTE]   
      > Als uw klant onder het Azure-plan valt, **wordt Bereik** ingesteld op **Gedeeld** op het moment van aankoop. Deze kan later worden gewijzigd.

    - Als u een providerpartner bent, selecteert u de reseller die u aan het product wilt koppelen.
    
    - Als uw Azure-reservering de optie Factureringsplan ondersteunt, kunt u de factureringsfrequentie als maandelijks selecteren in de vervolgkeuzelijst. 
    - Als uw Azure-reservering de optie Factureringsplan niet ondersteunt, wordt uw factureringsfrequentie standaard ingesteld op één keer facturering. 

9. Selecteer **Kopen om** de order te kopen. De details van uw bestelling, inclusief uw ordernummer, worden weergegeven op de **pagina** Bevestigen. Selecteer **Done om** naar de pagina **Ordergeschiedenis te** gaan. 

10. Als u de reservering van de klant in de Azure Portal  wilt beheren, gaat u naar de klant op de pagina Klanten en selecteert u vervolgens de pijl-omlaag om de rij van de klant uit te vouwen. Selecteer **Microsoft Azure Beheerportal** om de record van de klant in de Azure Portal.

## <a name="next-steps"></a>Volgende stappen

|**Voor informatie over**   |**Leest u**    |
|:-----------------------------|:-----------------|
|Overzicht van Azure-reserveringen in CSP  | [Verkopen Microsoft Azure gereserveerde instanties](azure-reservations.md) |
|Azure-reserveringen beheren in Partner Center | [Azure-reserveringen beheren in Partner Center](azure-reservations-manage.md)
|De juiste VM-grootte bepalen en het gebruik van de klant-VM controleren   |[VM-formaat voor maximaal gebruik van Azure-reserveringen](azure-usage.md)   |
|Azure-reserveringen kopen met behulp van Partner Center API | [Aankoop Azure Reserved VM Instances](/partner-center/develop/purchase-azure-reservations) in de documentatie Partner Center ontwikkelaars   |
|Klanten toestemming geven om hun eigen Azure-reserveringen te kopen  | [Klanten toestemming geven om hun eigen Azure-reserveringen te kopen](give-customers-permission.md)  |

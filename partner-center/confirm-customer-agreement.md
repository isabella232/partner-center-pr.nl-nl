---
title: Controleren of uw klant de micro soft-klant overeenkomst heeft geaccepteerd voor het CSP-programma
description: Cloud Solution Provider (CSP)-partners moeten acceptatie van de klant bevestigen van de klant overeenkomst van micro soft voordat ze micro soft-Services voor klanten best Ellen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633775"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Controleren of uw klant de micro soft-klant overeenkomst heeft geaccepteerd voor het CSP-programma

**Juiste rollen**

- Beheer agent
- Verkoop agent


Klanten hebben twee opties voor het accepteren van de klant overeenkomst van micro soft.

**Optie 1**: partner attest van klant acceptatie: de partner kan acceptatie van de klant bevestigen met de Partner Center API/SDK of via het dash board van de partner centrum.

**Optie 2**: klant direct accepteren-partner kan de klant via een URL uitnodigen om de overeenkomst in het Microsoft 365-beheer centrum te bekijken en te accepteren.

## <a name="access-microsoft-customer-agreement-template"></a>Toegang tot micro soft-sjabloon voor klant overeenkomst

U kunt de nieuwste [versie van de](https://aka.ms/customeragreement)micro soft-sjabloon voor klant overeenkomsten hand matig downloaden. De klant overeenkomst van micro soft is specifiek voor het land. Zorg ervoor dat u het juiste land selecteert op basis van de locatie van de klant wanneer u de micro soft-sjabloon voor klant overeenkomsten aanvraagt.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Optie 1: acceptatie van klant bevestigen in partner centrum

Directe factuur partners kunnen acceptatie van klant bevestigen van de klant overeenkomst van micro soft in het partner centrum voor nieuwe en bestaande klanten. Indirecte wederverkopers kunnen geen attesten namens hun klanten afgeven en moeten samen werken met hun indirecte provider om de Attestation te kunnen volt ooien.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Acceptatie van klant bevestigen voor nieuwe klanten

Wanneer u een nieuwe eigenaar van de klant in het partner centrum maakt, moet u de volgende stappen gebruiken om de acceptatie van de klant overeenkomst van micro soft te bevestigen. U moet een beheer agent of een verkoop agent zijn om deze stappen uit te voeren.

1. Selecteer **klanten** en vervolgens **nieuwe klant**.

2. Voer onder **account info** informatie in voor het bedrijf en de primaire contact persoon.

3. Schakel onder **micro soft Agreement** het selectie vakje in om te bevestigen dat de klant de micro soft-klant overeenkomst heeft geaccepteerd.

4. Voer bij **acceptatie datum** van de overeenkomst de juiste datum in. U kunt dit niet instellen op een datum in de toekomst.

5. Zorg ervoor dat de contact gegevens van de primaire gebruiker correct worden weer gegeven. Als het niet juist is, selecteert u **bijwerken** en voert u de juiste informatie in voor de persoon die de overeenkomst heeft geaccepteerd.

6. Selecteer **volgende** om door te gaan met het maken van de Tenant van de klant.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nieuwe klant":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Acceptatie van klant bevestigen voor bestaande klanten

U moet een beheer agent of verkoop agent zijn om dit te kunnen doen:

1. Selecteer **Klanten**. Zoek en selecteer de klant.

2. Selecteer **account gegevens**.

3. Selecteer in de **micro soft-klant overeenkomst** **Update**.

4. Voer de **voor naam**, **Achternaam**, het **e-mail adres** en het **telefoon nummer** (optioneel) in van de persoon die de overeenkomst heeft geaccepteerd. Voer bij **acceptatie datum** van de overeenkomst de juiste datum in. U kunt dit niet instellen op een datum in de toekomst.

5. Selecteer **Opslaan** en door gaan.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Bestaande klant":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Bevestiging van acceptatie van klant ophalen

Gebruik de volgende stappen om de bevestiging te verkrijgen dat een bestaande klant de micro soft-klant overeenkomst heeft geaccepteerd. U moet een beheer agent of verkoop agent zijn om dit te kunnen doen.

1. Selecteer **klanten** en zoek en selecteer de klant die u wilt zien.

2. Selecteer **account gegevens**.

3. Onder de **klant overeenkomst van micro soft** wordt weer gegeven of er een bevestiging is ontvangen door deze klant.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Acceptatie van klant bevestigen met partner Center API/SDK

U kunt de API/SDK van partner Center gebruiken om de acceptatie van de klant van micro soft te bevestigen. Raadpleeg voor meer informatie over de API/SDK:

- [Metagegevens van de overeenkomst voor de Microsoft-klantovereenkomst ophalen](/partner-center/develop/get-customer-agreement-metadata)

- [Acceptatie door de klant van Microsoft-klantovereenkomst bevestigen](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Bevestiging van acceptatie door de klant van Microsoft-klantovereenkomst ophalen](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Een download koppeling voor de micro soft-sjabloon voor klant overeenkomsten ophalen](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Optie 2: acceptatie van klant in Microsoft 365-beheer centrum

Partners kunnen nieuwe en bestaande klanten uitnodigen via een URL om de overeenkomst te bekijken en te accepteren binnen het Microsoft 365-beheer centrum. In de volgende secties ziet u hoe u het volgende kunt doen:

- Maak een nieuwe klant en vraag de klant om de overeenkomst te bekijken en te accepteren.

- Een nieuwe klant uitnodigen om de wederverkoper-relatie en-overeenkomst te bekijken en te accepteren.

- Een bestaande klant uitnodigen om de overeenkomst te bekijken en te accepteren.

>[!NOTE]
> U kunt de [API/SDK van partner Center](/partner-center/develop/get-direct-sign-status-of-customer-agreement) gebruiken om de status van de directe acceptatie van de klant van micro soft te verkrijgen.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Een nieuwe klant maken en de klant uitnodigen om de overeenkomst te bekijken en te accepteren

Voer de volgende stappen uit om een nieuwe klant te maken in het partner centrum en vraag ze om de klant overeenkomst van micro soft te bekijken en te accepteren binnen Microsoft 365 beheer centrum.

1. Selecteer **klant toevoegen** op het tabblad **klanten** binnen partner centrum.

2. Voer onder **account gegevens** informatie over de nieuwe klant in alle vereiste velden in, waaronder de bedrijfs naam en de primaire contact persoon van de klant.

3. Onder **klant overeenkomst** selecteert **u de optie klant wordt gevraagd om de micro soft-klant overeenkomst in Microsoft 365 beheer centrum te accepteren**. Alle andere verplichte velden op de pagina volt ooien.

4. Selecteer **volgende: controleren** en ga door met de stappen voor het maken van de Tenant van de klant. 

>[!NOTE] 
>Nieuwe klanten kunnen pas een aankoop doen als ze de micro soft-klant overeenkomst accepteren.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Nieuwe klant maken":::

5. Wanneer u het **bevestigings** scherm in de nieuwe klant werk stroom bereikt, slaat u de referenties van de klant op. U moet deze referenties later aan uw klant verlenen.

6. Maak en verzend buiten het partner centrum een e-mail die de klant nodig heeft om de micro soft-klant overeenkomst te accepteren in Microsoft 365 beheer centrum. Zorg ervoor dat u deze items opneemt in het e-mail bericht:

   - Een koppeling naar deze [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (aanmelden vereist)

   - De referenties van de klant die u hebt opgeslagen in stap 5.

7. De klant ontvangt vervolgens de uitnodiging voor e-mail van de partner en selecteert de [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. De klant meldt zich aan Microsoft 365 beheer centrum met de referenties van de klant die u hebt ingevoerd.

9. De klant controleert het vakje om de klant overeenkomst van micro soft te accepteren.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Een nieuwe klant uitnodigen om de reseller relationship-en micro soft-klant overeenkomst te bekijken en te accepteren 

Gebruik de volgende stappen om een nieuwe klant uit te nodigen om de reseller-relatie en de micro soft-klant overeenkomst te bekijken en te accepteren. 

1. Selecteer **een reseller-relatie koppeling aanvragen** op het tabblad **klanten** binnen partner centrum. 

2. Er wordt een automatische e-mail sjabloon gegenereerd, inclusief tekst en een geparametriseerde URL die de klant doorstuurt naar het Microsoft 365-beheer centrum.

3. U kunt de automatisch gegenereerde e-mail sjabloon aanpassen en vervolgens **kopiëren naar klem bord** selecteren of **in e-mail bericht openen**.

4. Gebruik deze e-mail sjabloon om de klant uit te nodigen om een **wederverkoper-relatie** aanvraag en de **micro soft-klant overeenkomst** te accepteren. (Opmerking: in de uitnodiging voor het e-mail bericht moet u ervoor zorgen dat de partner ook de URL bevat die automatisch is geleverd, evenals de referenties van de klant die onlangs zijn gemaakt.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="een relatie maken":::

5. Klant ontvangt uitnodiging via e-mail en klikt op de para meter-URL. 

6. De klant gebruikt de referenties die u binnen e-mail verstrekt om zich aan te melden bij Microsoft 365-beheer centrum.

7. Klant controleert het vakje om de **reseller Relationship** en de **klant overeenkomst van micro soft** te accepteren. 

8. Binnen dezelfde URL is de klant in staat een geconsolideerde lijst te zien met verschillende partners waarmee ze werken. Ze kunnen een partner selecteren om de details te zien.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Overeenkomst accepteren":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Een bestaande klant uitnodigen om de overeenkomst te bekijken en te accepteren

Gebruik de volgende stappen om een bestaande klant uit te nodigen om de micro soft-klant overeenkomst te controleren en te accepteren. 

1. Maak de e-mail van de klant met de Inge sloten URL die uw klant uitnodigt om de micro soft-klant overeenkomst te accepteren.

2. Uw klant ontvangt de uitnodiging via e-mail en klikt op de [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. De klant voert hun referenties in Microsoft 365-beheer centrum.

4. Uw klant controleert het vakje om de klant overeenkomst van micro soft te accepteren. 

5. Binnen dezelfde URL kan de klant de geconsolideerde lijst zien van verschillende partners waarmee ze werken. Ze kunnen een partner selecteren om de details te zien.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="gebruikers":::

>[!NOTE]
>In bepaalde scenario's kunnen klanten de micro soft-klant overeenkomst mogelijk niet rechtstreeks accepteren. Lees voor meer informatie over deze situaties twee scenario's waarbij u de volgende stappen moet afhandelen namens uw klant.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Twee scenario's waarin u namens uw klant moet worden verklaard

Er zijn twee scenario's waarbij klanten de micro soft-klant overeenkomst mogelijk niet direct kunnen accepteren binnen het Microsoft 365-beheer centrum.

**Scenario 1**: een bestaande klant heeft een van de volgende gekocht via een bestaande partner relationship: aanbiedingen, software-of software-abonnementen, gereserveerde instanties of Azure-abonnement. De klant probeert nu een nieuwe aankoop te maken (met uitzonde ring van automatische verlenging). Wanneer die klant op de URL klikt, ontvangt het bericht ' Neem contact op met uw partner om te bevestigen dat u de micro soft-klant overeenkomst accepteert. '  

**Om dit op te lossen**, moet u namens de klant een verklaring doen.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Scherm opname van Microsoft 365 beheer centrum pagina waarin u wordt gevraagd om uw partner te bereiken om acceptatie van de micro soft-klant overeenkomst te bevestigen.":::

**Scenario 2**: een bestaande klant heeft een van de volgende aanbiedingen gekocht, software-en software-abonnementen, gereserveerde instanties en Azure-abonnement. De klant probeert nu een nieuwe aankoop te doen met een nieuwe partner.

Wanneer de klant op de URL klikt om het beheer centrum te Microsoft 365 om de nieuwe partner relatie en de overeenkomst te accepteren, ontvangen ze het bericht ' Neem contact op met uw partner om te bevestigen dat de micro soft-klant overeenkomst wordt geaccepteerd. '  

**Om dit op te lossen**, moet u namens de klant een verklaring doen.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Bevestigen dat een klant de overeenkomst heeft geaccepteerd

Als u probeert een nieuwe bestelling te maken voor een bestaande klant die u nog niet eerder hebt bevestigd, ontvangt u een prompt om de bevestiging te volt ooien. Gebruik de volgende procedure om dit te doen.

1. Voer de **voor naam**, **Achternaam**, het **e-mail adres** en het **telefoon nummer** (optioneel) in van de gebruiker die de overeenkomst heeft geaccepteerd.

2. Voer bij **acceptatie datum** van de overeenkomst de juiste datum in. U kunt dit niet instellen op een datum in de toekomst.

3. Selecteer **Opslaan en doorgaan**. 

## <a name="next-steps"></a>Volgende stappen

- [De gegevens van uw bedrijfs profiel controleren of bijwerken](update-your-partner-profile.md)
- [Microsoft-klantovereenkomsten (op regio, taal)](Agreements.md)

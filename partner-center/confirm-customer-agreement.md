---
title: Controleren of uw klant de Microsoft-klantovereenkomst heeft geaccepteerd voor het CSP-programma
description: Cloud Solution Provider (CSP)-partners moeten de klantacceptatie van de Microsoft-klantovereenkomst bevestigen voordat ze Microsoft-services klanten bestellen.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: 205de1c852d263e79978358229f1365852872232
ms.sourcegitcommit: 986573bc4382b803bf4d641df6dd1e37c3af1955
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/16/2021
ms.locfileid: "127862405"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Controleren of uw klant de Microsoft-klantovereenkomst heeft geaccepteerd voor het CSP-programma

**Juiste rollen:** beheeragent | Verkoopagent


Klanten hebben twee opties voor de manier waarop ze de Microsoft-klantovereenkomst.

**Optie 1:** Partnerverklaring van klantacceptatie: de partner kan de acceptatie van de klant bevestigen met behulp van Partner Center API/SDK of via het Partner Center dashboard.

**Optie 2:** directe acceptatie door de klant: de partner kan de klant via een URL uitnodigen om de overeenkomst te controleren en te accepteren in Microsoft 365-beheer Center.

## <a name="access-microsoft-customer-agreement-template"></a>Toegang tot Microsoft-klantovereenkomst sjabloon

U kunt handmatig [de nieuwste versie van de Microsoft-klantovereenkomst.](https://aka.ms/customeragreement) De Microsoft-klantovereenkomst is specifiek voor het land. Wanneer u de sjabloon Microsoft-klantovereenkomst, moet u het juiste land selecteren op basis van de locatie van de klant.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Optie 1: Bevestig de acceptatie van de klant in Partner Center

Partners met directe factuur kunnen bevestigen dat de klant de Microsoft-klantovereenkomst in Partner Center voor nieuwe en bestaande klanten. Indirecte resellers kunnen niet namens hun klanten bevestigen en moeten samenwerken met hun indirecte provider om de attestation te kunnen uitvoeren.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Klantacceptatie voor nieuwe klanten bevestigen

Wanneer u een nieuwe klant-tenant maakt in Partner Center, gebruikt u de volgende stappen om te bevestigen dat de klant de Microsoft-klantovereenkomst. U moet een beheerderagent of verkoopagent zijn om deze stappen uit te voeren.

1. Selecteer **Klanten** en vervolgens **Nieuwe klant.**

2. Voer **onder Accountgegevens** informatie in voor het bedrijf en de primaire contactpersoon.

3. Schakel **onder Microsoft-overeenkomst** het selectievakje in om te bevestigen dat de klant de Microsoft-klantovereenkomst.

4. Voer **onder Acceptatiedatum van overeenkomst** de juiste datum in. U kunt dit niet instellen op een toekomstige datum.

5. Zorg ervoor dat de weergegeven contactgegevens van de primaire gebruiker juist zijn. Als dit onjuist is, selecteert u **Bijwerken** en voert u de juiste informatie in voor de persoon die de overeenkomst heeft geaccepteerd.

6. Selecteer **Volgende om** door te gaan met het maken van de tenant van de klant.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Nieuwe klant.":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Klantacceptatie voor bestaande klanten bevestigen

U moet een beheerderagent of verkoopagent zijn om dit te doen:

1. Selecteer **Klanten**. Zoek en selecteer de klant.

2. Selecteer **Accountgegevens.**

3. Selecteer **onder Microsoft-klantovereenkomst** de optie **Bijwerken.**

4. Voer de **voornaam**, **achternaam,** het **e-mailadres** en **het Telefoon** (optioneel) in van de persoon die de overeenkomst heeft geaccepteerd. Voer **onder Acceptatiedatum van overeenkomst** de juiste datum in. U kunt dit niet instellen op een toekomstige datum.

5. Selecteer **Opslaan** en doorgaan.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Bestaande klant.":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Bevestiging van klantacceptatie ophalen

Als u bevestiging wilt ophalen dat een bestaande klant de Microsoft-klantovereenkomst heeft geaccepteerd, gebruikt u de volgende stappen. U moet een beheerderagent of verkoopagent zijn om dit te doen.

1. Selecteer **Klanten** en zoek en selecteer vervolgens de klant die u wilt zien.

2. Selecteer **Accountgegevens.**

3. Bekijk **onder Microsoft-klantovereenkomst** of er al dan niet bevestiging is gegeven door deze klant.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Acceptatie door klant bevestigen met behulp Partner Center API/SDK

U kunt Partner Center API/SDK gebruiken om te bevestigen dat de klant de Microsoft-klantovereenkomst. Raadpleeg voor meer informatie over de API/SDK:

- [Metagegevens van de overeenkomst voor de Microsoft-klantovereenkomst ophalen](/partner-center/develop/get-customer-agreement-metadata)

- [Acceptatie door de klant van Microsoft-klantovereenkomst bevestigen](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Bevestiging van acceptatie door de klant van Microsoft-klantovereenkomst ophalen](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Downloadkoppeling voor de sjabloon Microsoft-klantovereenkomst downloaden](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Optie 2: Acceptatie van de klant in Microsoft 365-beheer Center

Partners kunnen nieuwe en bestaande klanten via een URL uitnodigen om de overeenkomst in het Microsoft 365-beheer accepteren. In de volgende secties ziet u het volgende:

- Maak een nieuwe klant en nodig de klant uit om de overeenkomst te beoordelen en te accepteren.

- Nodig een nieuwe klant uit om de resellerrelatie en overeenkomst te beoordelen en te accepteren.

- Nodig een bestaande klant uit om de overeenkomst te beoordelen en te accepteren.

>[!NOTE]
> U kunt Partner Center [API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) gebruiken om de status op te vragen van de directe acceptatie van de Microsoft-klantovereenkomst.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Een nieuwe klant maken en de klant uitnodigen om de overeenkomst te beoordelen en te accepteren

Gebruik de volgende stappen om een nieuwe klant te maken in Partner Center nodig ze vervolgens uit om de Microsoft-klantovereenkomst in Microsoft 365-beheer Center te beoordelen en te accepteren.

1. Selecteer op **het** tabblad Klanten Partner Center klant **toevoegen.**

2. Voer **onder Accountgegevens** informatie over de nieuwe klant in alle vereiste velden in, met inbegrip van de bedrijfsnaam en de primaire contactpersoon van de klant.

3. Selecteer **onder Klantovereenkomst** de **optie Klant wordt gevraagd om de Microsoft-klantovereenkomst te accepteren in Microsoft 365-beheer Center**. Vul alle andere vereiste velden op de pagina in.

4. Selecteer **Volgende: Controleren en** ga vervolgens verder met de stappen voor het maken van de tenant van de klant. 

>[!NOTE] 
>Nieuwe klanten kunnen pas een aankoop doen als ze de Microsoft-klantovereenkomst.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Maak een nieuwe klant.":::

5. Wanneer u het **bevestigingsscherm** in de nieuwe klantwerkstroom bereikt, moet u de klantreferenties opslaan. U moet deze referenties later aan uw klant geven.

6. Maak buiten Partner Center een e-mail waarin de klant wordt uitgenodigd om de Microsoft-klantovereenkomst te accepteren in Microsoft 365-beheer Center. Zorg ervoor dat u deze items in het e-mailbericht op neem:

   - Een koppeling naar deze [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (aanmelden vereist)

   - De referenties van de klant die u in stap 5 hebt opgeslagen.

7. De klant ontvangt vervolgens de e-mail-uitnodiging van de partner en selecteert de [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. De klant meldt zich aan Microsoft 365-beheer Center met behulp van de klantreferenties die u hebt opgegeven.

9. De klant controleert het selectievakje om de Microsoft-klantovereenkomst te accepteren.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Een nieuwe klant uitnodigen om de resellerrelatie te beoordelen en te accepteren en Microsoft-klantovereenkomst 

Gebruik de volgende stappen om een nieuwe klant uit te nodigen om de resellerrelatie en de Microsoft-klantovereenkomst. 

1. Selecteer op **het** tabblad Klanten Partner Center koppeling **Een resellerrelatie aanvragen.** 

2. Er wordt een automatische e-mailsjabloon gegenereerd, inclusief tekst en een geparameteriseerde URL die de klant doorgeeft aan Microsoft 365-beheer Center.

3. U kunt de automatisch gegenereerde e-mailsjabloon aanpassen en vervolgens **Kopiëren naar klembord of** Openen in **e-mail selecteren.**

4. Gebruik deze e-mailsjabloon om de klant uit te nodigen om de **aanvraag voor een resellerrelatie** en **de** Microsoft-klantovereenkomst. (Opmerking: Zorg ervoor dat de partner in de e-mailnodiging ook de URL bevat die automatisch is opgegeven, evenals de klantreferenties die onlangs zijn gemaakt.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="een relatie maken.":::

5. De klant ontvangt een uitnodiging via e-mail en klikt op de geparameteriseerde URL. 

6. De klant gebruikt de referenties die u in de e-mail hebt verstrekt om zich aan te melden bij Microsoft 365-beheer Center.

7. De klant controleert het selectievakje om de **resellerrelatie te** accepteren **en Microsoft-klantovereenkomst**. 

8. Binnen dezelfde URL kan de klant een geconsolideerde lijst zien met verschillende partners met wie ze werken. Ze kunnen een partner selecteren om details te bekijken.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Overeenkomst accepteren.":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Een bestaande klant uitnodigen om de overeenkomst te beoordelen en te accepteren

Gebruik de volgende stappen om een bestaande klant uit te nodigen om de Microsoft-klantovereenkomst. 

1. Maak het e-mailadres van de klant met de ingesloten URL waarin u uw klant uitnodigt om de Microsoft-klantovereenkomst.

2. Uw klant ontvangt de uitnodiging via e-mail en klikt op de [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. De klant voert zijn of haar referenties in Microsoft 365-beheer Center.

4. Uw klant controleert het selectievakje om de Microsoft-klantovereenkomst. 

5. Binnen dezelfde URL kan de klant de geconsolideerde lijst met verschillende partners zien met wie ze werken. Ze kunnen een partner selecteren om details te bekijken.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="Klant.":::

>[!NOTE]
>In bepaalde scenario's kunnen klanten de Microsoft-klantovereenkomst. Lees voor meer informatie over deze situaties Twee scenario's waarin u namens uw klant moet bevestigen, hieronder.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Twee scenario's waarbij u namens uw klant moet bevestigen

Er zijn twee scenario's waarin klanten de Microsoft-klantovereenkomst mogelijk niet rechtstreeks kunnen Microsoft 365-beheer het Microsoft 365-beheer center.

**Scenario 1:** een bestaande klant heeft een van de volgende aankopen gedaan via een bestaande partnerrelatie: aanbiedingen, software- of softwareabonnementen, gereserveerde instanties of een Azure-abonnement. De klant probeert nu een nieuwe aankoop te doen (met uitzondering van automatische verlenging). Wanneer die klant op de URL klikt, ontvangt deze het bericht 'Neem contact op met uw partner om te bevestigen dat u de url hebt Microsoft-klantovereenkomst.'  

**Om het probleem** op te lossen, moet u namens de klant bevestigen.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Schermopname van Microsoft 365-beheer centerpagina waarin u wordt gevraagd contact op te nemen met uw partner om te bevestigen dat de Microsoft-klantovereenkomst.":::

**Scenario 2:** Een bestaande klant heeft een van de volgende aanbiedingen, software- en softwareabonnementen, gereserveerde instanties en een Azure-abonnement aangeschaft. De klant probeert nu een nieuwe aankoop te doen met een nieuwe partner.

Wanneer de klant op de URL naar Microsoft 365-beheer Center klikt om de nieuwe partnerrelatie en de overeenkomst te accepteren, ontvangt deze het bericht 'Neem contact op met uw partner om te bevestigen dat u de Microsoft-klantovereenkomst.'  

**Om het probleem** op te lossen, moet u namens de klant bevestigen.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Bevestig dat een klant de overeenkomst heeft geaccepteerd

Als u probeert een nieuwe bestelling te maken voor een bestaande klant die u nog niet eerder hebt bevestigd, ontvangt u een prompt om de bevestiging te voltooien. Gebruik de volgende procedure om dit te doen.

1. Voer de **voornaam**, **achternaam,** het **e-mailadres** **en het Telefoon (optioneel)** in van de gebruiker die de overeenkomst heeft geaccepteerd.

2. Voer **onder Acceptatiedatum van overeenkomst** de juiste datum in. U kunt dit niet instellen op een toekomstige datum.

3. Selecteer **Opslaan en doorgaan**. 

## <a name="next-steps"></a>Volgende stappen

- [Uw bedrijfsprofielgegevens controleren of bijwerken](update-your-partner-profile.md)
- [Microsoft-klantovereenkomsten (op regio, taal)](Agreements.md)

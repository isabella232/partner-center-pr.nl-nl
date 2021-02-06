---
title: Migreren van PMC naar partner centrum
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Meer informatie over hoe u uw bedrijf migreert van Partner Membership Center (PMC) naar het partner centrum, met inbegrip van de stappen die u moet volgen.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: dd566a6d9ef60747eb7fd515b4d63d87d991da2a
ms.sourcegitcommit: d37a3f353426e52dfbbac577b7576f9c3f6d2ddf
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 02/06/2021
ms.locfileid: "99624184"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Gids voor migratie van PMC naar Partnercentrum

**Juiste rollen**

- Globale beheerder

De website van micro soft partner op partner.microsoft.com is een uniforme digitale ervaring voor partners. Vanuit de partner website kunt u uw kansen verkennen en zich houden in begeleide ervaringen waarmee uw bedrijf uw apps en services kan bouwen en verkopen met micro soft. Met de dashboard koppeling die beschikbaar is via de partner website, kunnen leden van de Microsoft Partner Network zich aanmelden bij het partner centrum waar u uw relatie met micro soft beheert, in Program ma's inschrijft en zich aanmeldt voor aanbiedingen.

Het Partner Membership Center (PMC) wordt buiten gebruik gesteld. Uw bedrijf is uitgenodigd om uw Microsoft Partner Network lidmaatschaps beheer naar het partner centrum te laten overstappen. In deze hand leiding wordt u voor bereid op wat u kunt verwachten wanneer u van PMC naar het partner centrum gaat.

>[!NOTE]
>Zelfs als uw bedrijf meer dan één account of locatie heeft, begint het verplaatsen naar partner centrum door één (uw eerste) account naar het partner centrum te verplaatsen.

## <a name="get-started"></a>Aan de slag

De verplaatsing begint in PMC. Uw globale beheerder krijgt een uitnodiging om te beginnen met verplaatsen.

### <a name="prepare-in-pmc"></a>Voorbereiden in PMC

- Uw bedrijfs gegevens verifiëren
- De contact persoon van het primaire programma verifiëren
- Bedrijfs locaties controleren
- Uw goedgekeurde gebruikers bijwerken

### <a name="when-youre-ready"></a>Wanneer u klaar bent

Selecteer aan de **slag** met uw uitnodiging. U wordt naar de aanmeldings pagina van het partner centrum geleid.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Aan de slag":::

## <a name="start-with-your-work-email"></a>Begin met uw zakelijke e-mail

Als uw bedrijf geen werk-e-mail en AAD-Tenant heeft, kunnen we u helpen bij het instellen van een bericht tijdens het aanmeldings proces van het partner centrum. Wanneer u zich probeert aan te melden met een e-mail account dat geen zakelijke e-mail is, zoals uw persoonlijke account, wordt u omgeleid om informatie over uw bedrijf op te geven zodat we een AAD-Tenant en e-mail berichten kunnen instellen. Deze bedrijfs gegevens worden gebruikt voor het volt ooien van uw account in partner centrum, dus zorg ervoor dat ze nauw keurig zijn.

>[!NOTE]
>Als u een partner bent in China en u bent Inge schreven in het programma voor de Microsoft Partner Network en de Cloud Solution Provider (CSP), hebt u voor elk account een afzonderlijke Tenant. Uw account met het Cloud Solution Provider-programma wordt beheerd op de nationale Cloud en uw Microsoft Partner Network-account wordt beheerd op de wereld wijde Cloud. De twee accounts kunnen niet worden gekoppeld.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Vertel ons over uw bedrijf":::

Nadat u de gegevens hebt gecontroleerd of bijgewerkt, selecteert u **accepteren en door gaan**.
De voor waarden op deze pagina zijn **precies hetzelfde** als de overeenkomst die uw bedrijf al heeft aangemeld bij PMC.  
Met deze stap wordt het maken van uw Azure AD-Tenant gestart en wordt uw met het werk account geleverd.

Selecteer **accepteren en door gaan** om ook het volgende te doen:

- Migreert uw account samen met alle locaties naar het partner centrum

- Hiermee worden alle competenties of kaarten gemigreerd die u mogelijk hebt gekocht in PMC

- Hiermee worden alle marketing resources, aanbiedingen en Program ma's (kaarten, zilver, goud) gemigreerd die u in PMC had

## <a name="invite-employees-to-join-you"></a>Werk nemers uitnodigen om lid te worden van u

Wanneer uw nieuwe Azure AD-Tenant wordt gemaakt, kunt u uw werk nemers uitnodigen om zich aan te melden bij het partner centrum.

:::image type="content" source="images/migration/invite.png" alt-text="Werk nemers uitnodigen":::

Als u bent aangemeld met een bestaande AAD-Tenant, worden uw werk nemers met u verplaatst. Wijs in dit geval uw werk nemers rollen toe die bepalen wat ze kunnen doen in het partner centrum. 

>[!NOTE] 
>Rollen in het partner centrum zijn anders dan rollen in PMC. Zie [overstappen van PMC naar partner Center](move-pmc-pc-map.md)voor meer informatie.

## <a name="verify-your-domain-and-become-a-global-admin"></a>Uw domein verifiëren en een globale beheerder worden  

Als uw AAD-Tenant nieuw is, wijst niemand de rol van globale beheerder toe. Als u de globale beheerder wilt worden, moet u uw domein eigendom verifiëren. Mogelijk hebt u de domein beheerder nodig om u hierbij te helpen.

Hoewel u de aanbiedingen kunt gebruiken die u al hebt aangeschaft, kunt u pas nieuwe aanbiedingen kopen als u de stap voor het toewijzen van een globale beheerder hebt voltooid.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Beheer overnemen":::

Wanneer u aan de slag selecteert, wordt het volgende scherm weer gegeven:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Domeineigendom controleren":::

Uw domein registratie is al voor u ingevuld. Alleen de eigenaar van het domein kan het DNS-bestand bijwerken. door het tekst bestand te kopiëren en toe te voegen aan uw DNS-record, kunnen we controleren of u de eigenaar bent. Het duurt enkele minuten voordat de update is uitgevoerd. U moet zich afmelden bij het partner centrum en u vervolgens weer aanmelden. Uw rol is gewijzigd in globale beheerder.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Kennismaken met uw dash board en partner centrum

Volg de rond leiding door uw dash board. Hier kunt u uw lidmaatschap beheren, een bedrijfs profiel voor verwijzingen toevoegen, registreren in het Cloud Solution Provider-programma en meldingen en aanbiedingen die relevant zijn voor uw bedrijf op elk gewenst moment weer geven door **dash board** te selecteren. U kunt ook prikkels beheren, kopen op Marketplace, registreren voor Go-to-Market-Services en meer.  

:::image type="content" source="images/migration/fre.png" alt-text="Volg de rond leiding":::

## <a name="sign-the-microsoft-partner-agreement"></a>De micro soft-partner overeenkomst ondertekenen

Als u een indirecte wederverkoper bent en u uw partner Center-account hebt ingesteld, moet u zich nog steeds officieel inschrijven in het Cloud Solution Provider-programma. Als u de status van uw lidmaatschap wilt controleren, gaat u naar uw [juridische profiel](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) en bevestigt u het account type. Schrijf u vervolgens in als een [indirecte wederverkoper](enrolling-in-the-csp-program.md).

 Zodra u bent Inge schreven als een indirecte wederverkoper, accepteert u de [CSP-relatie aanvraag met uw indirecte provider](indirect-reseller-tasks-in-partner-center.md).

Ga vervolgens akkoord met de micro soft-partner overeenkomst in het [dash board](https://partner.microsoft.com/pvc/dashboard) van de Partner Center met behulp van globale beheerders referenties. Bevestig dat u de micro soft-partner overeenkomst hebt ondertekend in het gedeelte met programma gegevens van het Partner profiel. U ziet ook een melding over een bericht met een waarschuwing op de overzichts pagina van CSP. 

## <a name="next-steps"></a>Volgende stappen

- [Uw globale beheerder zoeken](become-global-admin.md)

- [Microsoft Partner-overeenkomst](microsoft-partner-agreement.md)

- [Gebruikersaccounts maken](create-user-accounts-and-set-permissions.md)

- [Gebruikersrollen en -machtigingen toewijzen](permissions-overview.md)

- [Uw lidmaatschaps Programma's beheren](renew-mpn-offers.md)

- [Het bedrijfs profiel van uw bedrijf maken](create-a-marketing-profile.md)

- [Verbinding maken met klanten via verwijzingen](manage-leads.md)

- [Hand leiding voor het migreren van meerdere bedrijven van PMC naar partner Center](move-multiple-companies.md)

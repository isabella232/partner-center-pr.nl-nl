---
title: Migreren van PMC naar Partner Center
ms.topic: article
ms.date: 10/02/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Leer hoe u uw bedrijf migreert van Partner Membership Center (PMC) naar Partner Center, inclusief de stappen die u moet volgen.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 511612042f7da5e43d045d2991fa7d5251612726
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150740"
---
# <a name="guide-to-migrating-from-pmc-to-partner-center"></a>Gids voor migratie van PMC naar Partnercentrum

**Juiste rollen:** globale beheerder

De Microsoft-partnerwebsite op partner.microsoft.com is een uniforme digitale ervaring voor partners. Vanaf de partnerwebsite kunt u uw kansen verkennen en deelnemen aan begeleide ervaringen die uw bedrijf helpen bij het bouwen en verkopen van uw apps en services met Microsoft. Met behulp van de dashboardkoppeling die beschikbaar is op de partnerwebsite, kunnen leden van de Microsoft Partner Network zich aanmelden bij het partnercentrum waar u uw relatie met Microsoft beheert, zich inschrijft in programma's en zich kunt registreren voor aanbiedingen.

Partner Membership Center (PMC) wordt buiten gebruik gesteld. Uw bedrijf is uitgenodigd om uw lidmaatschapsbeheer over te Microsoft Partner Network naar Partner Center. Deze handleiding bereidt u voor op wat u kunt verwachten wanneer u overstapt van PMC naar Partner Center.

>[!NOTE]
>Zelfs als uw bedrijf meer dan één account of locatie heeft, begint de overstap naar Partner Center met het verplaatsen van één (uw eerste) account naar Partner Center.

## <a name="get-started"></a>Aan de slag

De overstap begint in PMC. Uw globale beheerder ontvangt een uitnodiging om de overstap te starten.

### <a name="prepare-in-pmc"></a>Voorbereiden in PMC

- De gegevens van uw bedrijf controleren
- De contactpersoon voor het primaire programma verifiëren
- Bedrijfslocaties controleren
- Uw goedgekeurde gebruikers bijwerken

### <a name="when-youre-ready"></a>Wanneer u klaar bent

Selecteer **Aan de slag** met uw uitnodiging. U gaat naar de Partner Center aanmeldingspagina.

:::image type="content" source="images/migration/getstarted.jpg" alt-text="Aan de slag":::

## <a name="start-with-your-work-email"></a>Beginnen met uw werk-e-mail

Als uw bedrijf geen werk-e-mail en AAD-tenant heeft, kunnen we u helpen er een in te stellen tijdens het Partner Center aanmeldingsproces. Wanneer u zich probeert aan te melden met een e-mailaccount dat geen werk-e-mail is, zoals uw persoonlijke account, wordt u omgeleid om informatie over uw bedrijf op te geven, zodat we een AAD-tenant en werk-e-mail kunnen instellen. Deze bedrijfsgegevens worden gebruikt om uw account in de Partner Center, dus zorg ervoor dat ze juist zijn.

>[!NOTE]
>Als u een partner in China bent en bent ingeschreven bij het Microsoft Partner Network- en Cloud Solution Provider(CSP)-programma, hebt u voor elk account een afzonderlijke tenant. Uw account met het Cloud Solution Provider-programma wordt beheerd in de nationale cloud en uw Microsoft Partner Network-account wordt beheerd in de wereldwijde cloud. De twee accounts kunnen niet worden gekoppeld.

:::image type="content" source="images/migration/newtellusabout.png" alt-text="Vertel ons meer over uw bedrijf":::

Nadat u de gegevens hebt geverifieerd of bijgewerkt, selecteert u **Accepteren en doorgaan.**
De voorwaarden op deze pagina zijn **exact hetzelfde** als de overeenkomst die uw bedrijf al heeft ondertekend in PMC.  
Met deze stap wordt het maken van uw Azure AD-tenant gestart en krijgt u het werkaccount.

Als u **Accepteren en doorgaan selecteert,** doet u het volgende:

- Migreert uw account samen met ALLE locaties naar Partner Center

- Migreert alle competenties of MAPs die u mogelijk hebt aangeschaft in PMC

- Migreert alle marketingbronnen, aanbiedingen en programma's (MAPs, Silver, Gold) die u in PMC had

## <a name="invite-employees-to-join-you"></a>Werknemers uitnodigen om lid te worden

Wanneer uw nieuwe Azure AD-tenant is gemaakt, kunt u uw werknemers uitnodigen om zich aan te melden bij Partner Center.

:::image type="content" source="images/migration/invite.png" alt-text="Werknemers uitnodigen":::

Als u zich hebt aangemeld met een bestaande AAD-tenant, zijn uw werknemers met u verplaatst. In dit geval wijst u de rollen van uw werknemers toe om te beheren wat ze kunnen doen in Partner Center. 

>[!NOTE] 
>Rollen in Partner Center zijn anders dan rollen in PMC. Zie Moving [from PMC to Partner Center (Over van PMC naar Partner Center).](move-pmc-pc-map.md)

## <a name="verify-your-domain-and-become-a-global-admin"></a>Uw domein verifiëren en een globale beheerder worden  

Als uw AAD-tenant nieuw is, krijgt niemand de rol van globale beheerder toegewezen. Als u de globale beheerder wilt worden, moet u het eigendom van uw domein verifiëren. Mogelijk hebt u de domeinbeheerder nodig om u daarbij te helpen.

Hoewel u de aanbiedingen kunt gebruiken die u al hebt aangeschaft, kunt u geen nieuwe aanbiedingen kopen totdat u de stap voor het toewijzen van een globale beheerder hebt voltooid.

:::image type="content" source="images/migration/takecontrol.png" alt-text="Controle nemen":::

Wanneer u Aan de slag selecteert, ziet u het volgende scherm:

:::image type="content" source="images/migration/verifytxt.png" alt-text="Domeineigendom controleren":::

Uw domeinregistrar is al voor u ingevuld. Alleen de domeineigenaar kan het DNS-bestand bijwerken, dus door het tekstbestand te kopiëren en toe te voegen aan uw DNS-record, kunnen we controleren of u de eigenaar bent. Het duurt enkele minuten voordat de update wordt uitgevoerd. Meld u af bij Partner Center en meld u vervolgens weer aan. Uw rol is gewijzigd in globale beheerder.

## <a name="get-acquainted-with-your-dashboard-and-partner-center"></a>Maak kennis met uw dashboard en Partner Center

Bekijk uw dashboard. Hier kunt u uw lidmaatschap beheren, een bedrijfsprofiel voor verwijzingen toevoegen, u inschrijven voor het Cloud Solution Provider-programma en meldingen en aanbiedingen bekijken die relevant zijn voor uw bedrijf door Dashboard te **selecteren.** U kunt ook incentives beheren, kopen op de marketplace, u registreren voor go-to-market-services en meer.  

:::image type="content" source="images/migration/fre.png" alt-text="Rondleiding":::

## <a name="sign-the-microsoft-partner-agreement"></a>De Microsoft Partner-overeenkomst

Als u een indirecte reseller bent en u uw Partner Center-account hebt ingesteld, moet u zich nog wel officieel inschrijven voor het Cloud Solution Provider programma. Als u de status van uw lidmaatschap wilt controleren, gaat u naar [uw juridische profiel](https://partner.microsoft.com/pcv/accountsettings/partnerprofile) en bevestigt u het accounttype. Schrijf u vervolgens in bij CSP als een [indirecte reseller](enrolling-in-the-csp-program.md).

 Nadat u zich hebt geregistreerd als een indirecte reseller, accepteert u de [aanvraag voor de CSP-relatie met uw indirecte provider](indirect-reseller-tasks-in-partner-center.md).

Accepteer vervolgens de Microsoft Partner-overeenkomst in het overzicht Partner Center [dashboard](https://partner.microsoft.com/pvc/dashboard) met de referenties van de globale beheerder. Controleer of u de Microsoft Partner-overeenkomst hebt ondertekend in de sectie Programmagegevens van partnerprofiel. U ziet ook een bevestigingsbannermelding op de CSP-overzichtspagina. 

## <a name="next-steps"></a>Volgende stappen

- [Uw globale beheerder zoeken](become-global-admin.md)

- [Microsoft Partner-overeenkomst](microsoft-partner-agreement.md)

- [Gebruikersaccounts maken](create-user-accounts-and-set-permissions.md)

- [Gebruikersrollen en -machtigingen toewijzen](permissions-overview.md)

- [Uw lidmaatschapsprogramma's beheren](renew-mpn-offers.md)

- [Het bedrijfsprofiel van uw bedrijf maken](create-a-marketing-profile.md)

- [Verbinding maken met klanten via verwijzingen](manage-leads.md)

- [Handleiding voor het migreren van meerdere bedrijven van PMC naar Partner Center](move-multiple-companies.md)

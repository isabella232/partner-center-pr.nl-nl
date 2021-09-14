---
title: Licenties beheren in Marketplace-aanbiedingen
ms.topic: how-to
ms.date: 04/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
description: Meer informatie over het instellen en beheren van licenties voor uw aanbiedingen op de commerciële marketplace van ISV.
author: petand123
ms.author: v-petand
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 73a02a0a6cad28939d21800c726811c8969ce9a2
ms.sourcegitcommit: 37eac16c4339cb97831eb2a86d156c45bdf6a531
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/13/2021
ms.locfileid: "126244925"
---
# <a name="manage-licensing-in-marketplace-offers"></a>Licenties beheren in Marketplace-aanbiedingen

**Juiste rollen:** Globale | Accountbeheerder

In dit artikel wordt beschreven hoe u een aanbieding in Partner Center instelt, deze beschikbaar maakt in Microsoft AppSource en vervolgens licenties voor die aanbieding beheert.  

>[!IMPORTANT]
>De mogelijkheden in dit artikel zijn momenteel beschikbaar als openbare preview.

## <a name="before-you-begin"></a>Voordat u begint

### <a name="commercial-marketplace-basics"></a>Basisbeginselen van de commerciële marketplace

Voordat u met dit proces begint, moet u zich vertrouwd maken met de basisbeginselen van de commerciële marketplace. Aan de slag met de artikelen in de onderstaande tabel. 

| Onderwerp  | Artikel  |
|-------|--------|
|Commerciële marketplace-abonnementen | [Abonnementen en prijzen voor aanbiedingen op de commerciële marketplace](/azure/marketplace/plans-pricing)    |
|Aanbiedingen voor commerciële marketplace  | [Typen vermeldingen](/azure/marketplace/determine-your-listing-type)    |
|Commerciële marketplace-accounts |  [Een account voor een commerciële marketplace maken in het Partnercentrum](/azure/marketplace/create-account) |

### <a name="determine-your-offer-id"></a>Uw aanbiedings-id bepalen

In de onderstaande procedures wordt u gevraagd een aanbiedings-id in te voeren. Neem nu even de tijd om een geschikte aanbiedings-id te vinden, waarbij u rekening houdt met de volgende punten:

- Deze id is zichtbaar voor klanten in het webadres voor de Marketplace-aanbieding en Azure Resource Manager sjablonen, indien van toepassing.
- De aanbiedings-id in combinatie met Publisher id moet minder dan 40 tekens lang zijn.
- Gebruik alleen kleine letters en cijfers. De aanbiedings-id kan afbreekstreepingstekens en onderstrepingstekens bevatten, maar geen spaties. Als uw id bijvoorbeeld Publisher is en u in voert, is `testpublisherid` `test-offer-1` het webadres van de aanbieding `https://appsource.microsoft.com/product/dynamics-365/testpublisherid.test-offer-1` .
- Deze id kan niet worden gewijzigd nadat u Maken **hebt geselecteerd.**

### <a name="determine-your-offer-alias"></a>Uw aanbiedingsalias bepalen

De alias Aanbieding is de naam die wordt gebruikt voor de aanbieding in Partner Center. U hebt ook een geschikte alias voor de aanbieding nodig die de onderstaande richtlijnen volgt:

- Deze naam wordt niet gebruikt in de marketplace en verschilt van de naam van de aanbieding en andere waarden die aan klanten worden weergegeven.
- Deze naam kan niet worden gewijzigd nadat u Maken hebt geselecteerd.

## <a name="create-your-offer"></a>Uw aanbieding maken

De eerste stap in het licentieproces is het maken van uw commerciële marketplace-aanbieding. 

1. Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).
2. Selecteer commerciële marketplace/overzicht in het navigatiemenu **aan de linkerkant.**
3. Selecteer bovenaan de pagina Overzicht de optie Nieuwe **aanbieding** en selecteer vervolgens **Dynamics 365 for Customer Engagement & PowerApps.**
4. Voer de **aanbiedings-id en** **aanbiedingsalias in** die u eerder hebt gemaakt.
5. Selecteer **Maken om** de aanbieding te genereren en door te gaan.
6. Kies uw licentieopties.

    - Als u licentiebeheer voor uw aanbieding wilt inschakelen, selecteert **u App-licentiebeheer via Microsoft inschakelen.** Dit is een een time-instelling en u kunt deze niet meer wijzigen nadat uw aanbieding is gepubliceerd.

    - U kunt klanten ook in staat stellen om de basisfunctionaliteit van uw app uit te voeren zonder licentie en Premium-functies uit te voeren zodra ze een licentie hebben aangeschaft. Als u dit wilt doen, **selecteert u Klanten toestaan mijn app te installeren, zelfs als er geen licenties zijn toegewezen.**

    - Als u niet wilt dat licentiebeheer voor uw aanbieding is ingeschakeld, selecteert u Nu downloaden **(gratis)**, **Gratis proefversie** of **Neem contact met mij op.**

## <a name="create-your-plan"></a>Uw plan maken

In deze stappen definieert u het plan of de plannen die u wilt inschakelen voor uw aanbieding.

1. Selecteer in het navigatiemenu aan de **linkerkant Overzicht plannen** en selecteer **vervolgens Nieuw abonnement maken.**
2. Voer een **plan-id** en **plannaam in** en selecteer **vervolgens Maken.**
3. Voer op **de pagina Abonnementsvermelding** de beschrijving van uw abonnement **in.**
4. Als u de beschrijving wilt opslaan en later wilt voltooien, selecteert **u Concept opslaan.**

5. Wanneer u klaar bent, selecteert u **Controleren en publiceren.** De plangegevens worden nu weergegeven op appsource.microsoft.com aanbiedingsvermelding (sectie abonnementen).

6. Nadat u alle plannen voor deze aanbieding hebt gemaakt, moet u de service-id van elk plan kopiëren. Selecteer **Bovenaan de pagina** Abonnementsvermelding de optie Planoverzicht. Kopieer de service-id voor elk plan naar een veilige locatie.

## <a name="add-service-ids-to-your-solution"></a>Service-ID's toevoegen aan uw oplossing

De volgende stap is het bijwerken van uw oplossing door de service-ID's toe te voegen voor elk plan dat u zojuist hebt gekopieerd. Zie Create an [AppSource Package for your solution (Een AppSource-pakket maken voor uw oplossing) voor hulp.](/powerapps/developer/data-platform/create-package-app-appsource)

## <a name="upload-your-package-and-publish-your-offer"></a>Upload pakket maken en uw aanbieding publiceren

1. Selecteer in het navigatiedeelvenster links **Commerciële marketplace** en selecteer vervolgens **Technische configuratie.**
2. Selecteer **onder Basislicentiemodel** de optie **Gebruiker**.
3. Voer **onder CRM-pakket** de URL van uw pakketlocatie in.
4. Gebruik de andere tabbladen in het linkernavigatievenster om andere vereiste gegevens in te voeren. Wanneer u klaar bent, selecteert u **Controleren en publiceren.**

Nadat u de aanbieding hebt gepubliceerd, controleren en verifiëren we uw gegevens. Als er problemen zijn met dit proces, stellen we u hiervan op de hoogte. Wanneer alle problemen zijn opgelost, ontvangt u een melding dat uw aanbieding beschikbaar is in AppSource. Op dat moment kunt u het live maken.

## <a name="make-your-offer-live-in-partner-center"></a>Uw aanbieding live maken in Partner Center

De onderstaande procedure laat u zien hoe u uw aanbieding live kunt maken in AppSource. Zie Inleiding tot lijstopties voor meer informatie [over dit proces.](/azure/marketplace/determine-your-listing-type)

>[!NOTE]
>Nadat u uw aanbieding hebt gepubliceerd, duurt het 4-6 uur om live te gaan.

1. Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).
2. Selecteer commerciële marketplace/overzicht in het navigatiemenu **aan de linkerkant.**
3. Zoek op **de** pagina Overzicht de aanbieding die u zoekt. Aanbiedingen die gereed zijn om te worden gepubliceerd, hebben de status **Preview**. Selecteer de aanbieding.
4. Selecteer op **de pagina Overzicht** van aanbieding de optie Live **gaan.**
De aanbieding is binnen 4-6 uur live.
5. Als u uw aanbiedingsvermelding op AppSource wilt bekijken, selecteert u de **koppeling AppSource** onder aan de **overzichtspagina van de** aanbieding.

    - **Voor aanbiedingen met licentie:** als voor uw aanbieding een licentiecontrole is vereist, kunnen gebruikers alleen een lead invoeren door op **Contact** opnemen te klikken, zodat u met hen kunt communiceren.

    - **Voor aanbiedingen met licentie met** een gratis installatieoptie: als voor uw aanbieding  geen licentiecontrole is vereist, zien beheerders naast Contact opnemen ook de knop Nu **downloaden.** Gebruikers die de optie voor gratis installatie willen proberen, moeten klikken op Nu downloaden **om** de aanbieding te installeren in Power Platform Beheercentrum. Gebruikers kunnen contact opnemen **nog steeds gebruiken** als ze vragen hebben of als ze willen upgraden naar een betaald abonnement.

## <a name="register-isv-connect-deal-in-deal-registration"></a>ISV-Verbinding maken registreren in dealregistratie

Voordat u licenties aan een klant kunt toewijzen, moet elke verkoop worden geregistreerd in Partner Center. Zie Uw deals registreren [om dit te doen.](register-deals.md)

## <a name="invite-the-customer"></a>De klant uitnodigen

Gebruik de volgende procedure om de klant uit te nodigen om deel te nemen aan deze deal.  

1. Meld u aan bij het [Partnercentrum-dashboard](https://partner.microsoft.com/dashboard/).
2. Selecteer commerciële marketplace/overzicht in het navigatiemenu **aan de linkerkant.**
3. Selecteer in het navigatiemenu links **Verwijzingen** en selecteer vervolgens **Dealregistratie.**
4. Filter op **Ingediende** deals, selecteer het **tabblad Wordt** uitgevoerd en selecteer vervolgens de deal die u wilt.
5. Selecteer licenties beheren op de **overzichtspagina voor deze deal.**
6. Selecteer in **het venster Licenties beheren** de klant in de **vervolgkeuzelijst Klantgegevens.** Als de klantrelatie nog niet bestaat, selecteert u **+Een nieuwe klant uitnodigen om toestemming te geven.**
7. Kopieer de koppeling die wordt weergegeven.
8. Stuur deze koppeling via e-mail naar de factureringsbeheerder of globale beheerder van uw klant en laat deze deze koppeling gebruiken om toegang te krijgen tot admin.microsoft.com en de relatie die u tot stand wilt stellen te accepteren en autoriseerde.

    >[!NOTE]
    >De relatie wordt pas tot stand gebracht als de klant deze stap uitvoert.

## <a name="activate-manage-and-remove-your-licenses"></a>Uw licenties activeren, beheren en verwijderen

Zodra uw klant de relatie met u heeft geautoriseerd, kunt u beginnen met het toevoegen van plannen vanuit uw aanbieding en het toewijzen van licenties aan elk plan.

1. Selecteer in het venster Licenties beheren voor deze deal de optie **+Een abonnement toevoegen.**
2. Vul de **velden Abonnementen voor deze oplossing** en Aantal **licenties** in en selecteer vervolgens **Licenties bijwerken.** De licenties zijn beschikbaar op elk admin.microsoft.com klanten kunnen beheren en toewijzen aan werknemers.

    - Als u het aantal licenties voor een bestaand abonnement  wilt wijzigen, voert u het nieuwe nummer in het veld Aantal licenties in en selecteert u **vervolgens Licenties bijwerken.**

    - Als u licenties voor een deal wilt deactiveren of verwijderen, selecteert u het prullenbakpictogram in het **veld** Acties en selecteert u **vervolgens Licenties bijwerken.**

## <a name="next-steps"></a>Volgende stappen

[Licenties toewijzen aan resources](support-resources-licensing.md)
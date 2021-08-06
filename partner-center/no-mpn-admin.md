---
title: Wat te doen als de enige beheerder voor uw MPN-programma het bedrijf heeft verlaten?
ms.topic: how-to
ms.date: 09/08/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-account
description: Ontdek wat u moet doen om een nieuwe MPN-beheerder te vinden of hulp te krijgen van de globale beheerder van uw bedrijf. Meer informatie over het toevoegen van een nieuwe Partner Center globale beheerder.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 283cc274e150615d8f32da0b3e81ea01e0d86f0a
ms.sourcegitcommit: 90bf27df911b428b1222f483c32ba6367870e7c5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/04/2021
ms.locfileid: "115101630"
---
# <a name="what-to-do-if-the-only-admin-for-your-mpn-program-has-left-the-company"></a>Wat te doen als de enige beheerder voor uw MPN-programma het bedrijf heeft verlaten?

**Juiste rollen:** BEHEER VAN MPN-partner | Accountbeheerder | Globale beheerder

In het volgende artikel worden drie typische scenario's beschreven met betrekking tot wat u moet doen als uw MPN-beheerder het bedrijf heeft verlaten.

## <a name="scenario-1-mpn-partner-adminaccount-admin-has-left-the-company-but-there-are-still-global-admins-in-the-account"></a>Scenario 1: De beheerder/accountbeheerder van de MPN-partner heeft het bedrijf verlaten, maar er zijn nog steeds globale beheerders in het account

In dit geval kan aan een andere persoon in het bedrijf de rol van MPN-partnerbeheerder worden toegewezen. De rol van de specifieke rol van mpn-partnerbeheerder/accountbeheerder worden toegewezen:

1. Meld u aan Partner Center account met uw werkaccount (bijvoorbeeld tom@contoso.com ).
1. Filter op **de pagina Gebruikersbeheer** op Globale beheerder om te zien wie de globale beheerders voor uw bedrijf zijn. 
1. Neem contact op met een van de globale beheerders en vraag deze om u de MPN-specifieke rol toe te wijzen die u nodig hebt. 

## <a name="scenario-2-mpn-partner-adminaccount-admin-has-left-the-company-and-there-are-no-global-admins-in-the-account"></a>Scenario 2: De beheerder/accountbeheerder van de MPN-partner heeft het bedrijf verlaten en er zijn geen globale beheerders in het account 

Als u naar  de pagina Gebruikersbeheer gaat en filtert op Globale beheerder, maar u ziet dat uw bedrijf geen globale beheerder heeft die u kan helpen bij het verkrijgen van de MPN-specifieke rol, volgt u deze stappen:

1. Ga naar [portal.azure.com](https://ms.portal.azure.com/), meld u aan met uw werkaccount (bijvoorbeeld tom@contoso.com ). 
1. Selecteer de **optie Help en ondersteuning** in de navigatiebalk aan de linkerkant.
1. Selecteer op de volgende pagina Nieuw  **Ondersteuningsaanvraag** type technisch probleem in de vervolgkeuzelijst, voeg eventuele aanvullende details in en klik op **Volgende: Oplossingen.**

:::image type="content" source="images/accountsettings/adminfinder.png" alt-text="Zoek de beheerder in Azure Portal.":::

4. Nadat u de aanbevolen oplossingen op de volgende pagina controleert, selecteert u **Volgende: Details en** vult u de benodigde velden in.
1. Controleer en maak de ondersteuningsaanvraag.


## <a name="scenario-3-mpn-partner-adminaccount-adminglobal-admin-has-left-the-company-and-there-are-no-other-users-who-can-access-the-companys-azure-ad-this-is-a-complete-loss-of-access"></a>Scenario 3: DEN-partnerbeheerder/accountbeheerder/globale beheerder heeft het bedrijf verlaten en er zijn geen andere gebruikers die toegang hebben tot Azure AD van het bedrijf. Dit is een volledig verlies van toegang.

Volg de [stappen voor het overnemen](/azure/active-directory/users-groups-roles/domains-admin-takeover#internal-admin-takeover) van beheerders om als beheerder een niet-Azure Active Directory overnemen.

## <a name="not-sure-if-your-company-already-has-a-work-account"></a>Weet u niet zeker of uw bedrijf al een werkaccount heeft?

Als u niet zeker weet of uw bedrijf een werkaccount heeft, volgt u deze stappen om dit te controleren.

1. Meld u aan bij de [Azure-beheerportal.](https://ms.portal.azure.com)
2. Selecteer **Azure Active Directory** in het menu links en selecteer **vervolgens Domeinnamen.**
Als u al een werkaccount hebt, wordt uw domeinnaam weergegeven.

>[!Note]
>Als u een actief abonnement op Microsoft Azure of Office 365 hebt, hebt u al een werkaccount en moeten uw aanmeldingsreferenties hetzelfde zijn als de referenties die worden gebruikt voor toegang tot deze services.
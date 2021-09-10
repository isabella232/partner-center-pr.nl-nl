---
title: Skype voor Bedrijven migreren
description: Leer hoe en wanneer u bepaalde klanten met verlopende Skype voor Bedrijven Online-abonnement 1 migreert naar nieuwe Office 365 versies.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-pricing
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 58908e966eb80d219afa0cbc8c043932f5aef1a1
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "123957806"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrate Skype for Business Online Plan 1 subscriptions to newer Office 365 version (Abonnementen op Skype voor Bedrijven Online Plan 1 migreren naar nieuwere versie van Office 365)

**Juiste rollen:** Verkoopagent

Het Skype voor Bedrijven Online-abonnement 1 wordt met ingang van 1 augustus 2018 ingetrokken. Na die datum kunnen klanten geen nieuwe Skype voor Bedrijven Abonnement 1-abonnementen meer aanschaffen. Bestaande abonnementen worden niet automatisch verlengd wanneer ze verlopen en bieden geen verlengingsoptie. Op de detailpagina van het abonnement is de Skype voor Bedrijven Online-abonnement 1 gewijzigd in 'Verloopt op [datum]' van 'Automatisch verlengen op [datum]'.  

Om de continuïteit voor klanten te waarborgen, moet u klanten met verlopen Skype voor Bedrijven Online Plan 1-abonnementen overstappen naar een ondersteunde SKU-optie, die hieronder wordt vermeld. Het is raadzaam om klanten vóór de jaarlijkse einddatum van het abonnement over te brengen naar nieuwe abonnementen om service-uitval voor klanten te voorkomen. 

>[!NOTE]
>Zowel Skype voor Bedrijven online abonnement 1 commerciële SKU's als overheids-SKU's worden ingetrokken.

Als u de API (Commerce REST (EIGENDOM) of Partner Center) gebruikt, gaat u naar verlopende abonnementen door de einddatum van het abonnement te evalueren, samen met de eigenschap auto renew = False. De Skype voor Bedrijven Online Plan 1-abonnementen worden op 1 september 2018 ingesteld op automatisch verlengen=Onwaar. U kunt klanten op elk moment verplaatsen naar een nieuw abonnement. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Skype voor Bedrijven Vervangingsplannen online abonnement 1

Met de nieuwe abonnementen kunnen uw klanten profiteren van nieuwere functies en functionaliteit in Office 365. Prijsdetails vindt u in de matrix met prijzen en aanbiedingslijst in Partner Center. 

- Optie 1: Office 365 Enterprise F1
- Optie 2: Microsoft 365 Enterprise F1
- Optie 3: Andere Office 365 plannen

|**Functie**    |**Optie 1**   |**Optie 2**   |**Optie 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Alle functies van Skype voor Bedrijven Online-abonnement 1|Ja   |Ja   |Ja   |
|IM en aanwezigheid |Ja   |Ja   |Ja   |
|Peer-to-peer audio en video via IP|Ja   |Ja   |Ja   
|Deelnemen aan vergaderingen als geverifieerde gebruiker| Ja   |Ja   |Ja   |

## <a name="transition-customers-to-new-product-plans"></a>Klanten overstappen op nieuwe productplannen

Microsoft biedt voortdurend nieuwe producten en services aan onze partners. In dergelijke gevallen moet u mogelijk klanten upgraden naar nieuwe services of hun abonnementen migreren van SKU's die uiteindelijk worden afgesloten. Voor het migreren van klanten van buiten gebruik stellende SKU's naar nieuwere SKU's zijn de volgende stappen vereist:

- Het nieuwe abonnement kopen
- Huidige gebruikerslicenties opnieuw toewijzen
- Oud abonnement annuleren

### <a name="migrate-your-customers-to-new-plans"></a>Uw klanten migreren naar nieuwe abonnementen

1. Als u het nieuwe abonnement wilt kopen, selecteert u in Partner Center **menu** **Klanten,** selecteert u de klant die u wilt verplaatsen en selecteert u vervolgens **Abonnementen toevoegen.**

2. Selecteer het abonnement dat u wilt kopen in de catalogus (in dit geval een van de bovenstaande opties), voer het aantal licenties in en selecteer **vervolgens Verzenden.** 

Uw klant moet nu zowel oude als nieuwe abonnementen hebben, het oude Skype voor Bedrijven Online Plan 1-abonnement en het nieuwe doelabonnement, bijvoorbeeld Optie 1 - Office 365 Enterprise F1.

3. Als u de licenties van de gebruikers van de klant opnieuw wilt toewijzen, selecteert u klanten in het **menu Partner Center,** selecteert u de klant die u verplaatst en selecteert u vervolgens Gebruikers **en licenties.** De pagina Gebruikers en licenties van de klant wordt geopend.

4. Als u de gebruikerslicentie opnieuw wilt toewijzen, selecteert u de gebruiker die u opnieuw wilt toewijzen en selecteert u **vervolgens Licenties beheren.**

5. Schakel op **de pagina** Licenties beheren het selectievakje Skype voor Bedrijven Online Abonnement 1-licentie uit en selecteer een nieuw serviceabonnement voor het abonnement waar de klant naar overstapt.

6. Selecteer **Indienen**. Een bevestigingspagina bevat de nieuwe licentietoewijzingen. Ga door met hetzelfde proces voor andere gebruikers die licentietoewijzingen nodig hebben.

Nadat u de gebruikerslicentie hebt verplaatst naar de nieuwe service, kunt u het uit gebruik genomen abonnement veilig op klantniveau annuleren.

7. Selecteer in **Partner Center** menu **Klanten.** Selecteer de klant van wie u het abonnement annuleert.

8. Stel op de detailpagina van het abonnement het abonnement in op **Tijdelijk ingesteld.**

9. Selecteer **Verzenden.**

Het oude abonnement is opgeschort en het nieuwe abonnement is actief. De inrichting van het abonnement wordt na 120 dagen automatisch verwijderd. De klant maakt geen extra kosten voor het oude abonnement.

## <a name="next-steps"></a>Volgende stappen

- [Adviseurs: een uitnodiging voor een proefabonnement maken en verzenden voor clients om de Office 365](advisors-create-a-trial-invitation.md)
- [Adviseurs: stel een klantenbestand samen met behulp van uitnodigingen voor Office 365-proefabonnementen en aankoopaanbiedingen](advisors-build-your-business.md)
- [Adviseurs: Een aankoopaanbieding maken](advisor-create-a-purchase-offer.md)

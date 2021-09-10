---
title: Een nieuwe klantrecord toevoegen
ms.topic: how-to
ms.date: 09/07/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-customers
description: Meer informatie over het toevoegen van een nieuwe klantrecord in Partner Center. Vervolgens kunt u de klantabonnementen verkopen, facturering beheren of klantondersteuning bieden.
author: parthp
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 7995ee8f4da20d80fd260bcb77665e244e448227
ms.sourcegitcommit: 1161d5bcb345e368348c535a7211f0d353c5a471
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 09/09/2021
ms.locfileid: "124343093"
---
# <a name="how-to-add-a-new-customer-record-in-partner-center"></a>Een nieuwe klantrecord toevoegen in Partner Center

**Juiste rollen:** globale | Gebruikersbeheerbeheerders | Beheeragent | Verkoopagent

In dit artikel wordt beschreven hoe u een nieuwe klant toevoegt aan Partner Center. Deze stappen zijn vereist voordat u abonnementen kunt verkopen, facturering kunt beheren of ondersteuning kunt bieden aan een klant.

## <a name="considerations"></a>Overwegingen

**Wanneer u een nieuwe klantrecord toevoegt in Partner Center:**

- **Gebruik de juiste registratie-id:** bij het invoeren van uw bedrijfsregistratie-id moet u uw zakelijke btw-id gebruiken en niet het persoonlijke id van de klant.

- **Voer aanvullende informatie in voor** sommige landen: de registratie-id en het telefoonnummer van het bedrijf zijn vereist voor sommige landen als u een directe factuurpartner of een indirecte provider bent [](#company-registration-id-and-phone-number-required-for-some-countries)
- **Bevestig Microsoft-klantovereenkomst:** voordat u namens een klant een order kunt plaatsen, moet u bevestigen dat de klant de [Microsoft-klantovereenkomst.](confirm-customer-agreement.md)
- **** Verschillende stappen gebruiken voor bestaande klanten: voor bestaande klanten, met inbegrip van [](multichannel.md) klanten die al klantrecords in Partner Center via een [scenario](multipartner.md) met meerdere kanalen of meerdere klanten [hebben,](request-a-relationship-with-a-customer.md)kunt u een relatie met hen aanvragen in plaats van de stappen hier te volgen.
- **Voer gedetailleerde, nauwkeurige klantgegevens in:** om de klantverificatie, moet u ervoor zorgen dat u:
  - Voer de exacte juridische/officiële naam in zoals deze wordt weergegeven in de officiële documenten.
  - Vermijd het gebruik van acroniemen of korte formulieren.
  - Gebruik geen testnamen.
  - Geef volledige, exacte adresgegevens op (bijvoorbeeld locatiegegevens, plaats, staat, land en postcode).

## <a name="new-rules-for-company-name-and-email-address"></a>Nieuwe regels voor bedrijfsnaam en e-mailadres

Vanaf 22 september 2021 zijn de volgende nieuwe validatieregels van toepassing.

Bij het invoeren van een bedrijfsnaam is het volgende niet toegestaan:
- Gebruik slechts één teken.
- Alleen speciale tekens gebruiken, zoals &$^# (zie [de onderstaande](#table-of-special-characters) tabel).
- Alleen spaties en/of tabbladen gebruiken.
- Zelfstandige afkortingen uit de beperkte lijst gebruiken, zoals LLC, Inc, enzovoort (zie [de onderstaande](#table-of-abbreviations) tabel).
- Namen gebruiken met TDL-extensies (Internet Top-Level Domain), zoals '.com', '.org', '.edu', '.club', enzovoort [(zie](#table-of-top-level-domain-extensions) de onderstaande tabel).

- Het gebruik van hetzelfde teken herhaalde drie of meer keren zonder andere tekens, zoals 999.

- Spaties en/of tabbladen gebruiken die zijn gemengd met afzonderlijke tekens, zoals 1 2 3.

Bij het invoeren van een e-mailadres van de klant is het volgende niet toegestaan:

- Het e-mailadres mag geen @microsoft.com bevatten.
- Het e-mailadres van de klant mag niet dezelfde domeinnaam bevatten als de partner. Een partner met de naam ABC kan bijvoorbeeld geen e-mail van een klant maken met @abc.com .

## <a name="to-add-a-new-customer-in-partner-center"></a>Een nieuwe klant toevoegen in het Partner Center

1. Selecteer in Partner Center menu **Klanten** en selecteer vervolgens Klant **toevoegen.**
2. Als uw klant een onderwijsinstelling is, [bekijkt u hoe u een klant voor deductie maakt.](sell-to-education-customers.md)

3. Voer op **de pagina Accountgegevens** de details en primaire contactgegevens van de klant in.
   >[!IMPORTANT]
   >Partners moeten het volgende bevestigen:
   >
   >Ik bevestig dat mijn organisatie als indirecte partner optreedt bij het kiezen van een reseller en als directe partner als er geen reseller wordt geselecteerd
   >
   >Ik bevestig dat ik geen producten die in deze bestelling zijn gekocht, opnieuw verkoop aan andere partners die zijn gelieerd aan mijn bovenliggende organisatie

   >[!NOTE]
   >Volgens de staatswetgeving van de EU/EFTA moeten partners die transacties in deze landen hebben, extra resellers declareeren die zijn gekoppeld aan een transactie. De volgende regels zijn van toepassing:
   >- Er moet een eerste reseller worden gekozen vóór eventuele extra resellers
   >- Aanvullende resellers hebben geen recht op extra incentives, aanbiedingen, enzovoort.
   >- Aanvullende ingevoerde verkopers worden gevalideerd om ervoor te zorgen dat de juiste MPN-id wordt ingevoerd, indien van toepassing, en dat de reseller de MPA heeft ondertekend.
   >- Er kunnen maximaal vijf extra resellers worden ingevoerd als onderdeel van de transactie 

4. Als u een indirecte provider bent, selecteert u de indirecte reseller die u wilt koppelen aan de abonnementen van deze klant in de lijst.

5. Wanneer u klaar bent met het invoeren van de vereiste gegevens, selecteert **u Volgende: Abonnementen.**

6. Selecteer op **de pagina** Abonnementen de aanbieding(en) die uw klant bij u wil kopen, voer het aantal licenties in en selecteer **volgende: Controleren.**

7. Controleer op **de** pagina Controleren uw vermeldingen op nauwkeurigheid en selecteer vervolgens **Verzenden.**

8. Wanneer u klaar bent met het toevoegen van klantgegevens en de vereiste abonnementen hebt aangeschaft, selecteert u **Gereed.**

## <a name="company-registration-id-and-phone-number-required-for-some-countries"></a>Bedrijfsregistratie-id en telefoonnummer vereist voor sommige landen

Partners voor directe factuur en indirecte providers die records toevoegen voor klanten in de volgende landen, moeten ook het telefoonnummer en de registratie-id van het bedrijf invoeren (ook wel de ORGANISATIE-INN genoemd):

10, 2016, 2016, 2018, 2016, 2016, 2016, 2016, 2016, 2016, 2016, 2016, 2016, 2016, 2018 en 2018.

## <a name="company-name-and-email-characters-abbreviations-and-extensions"></a>Bedrijfsnaam en e-mailtekens, afkortingen en extensies

In de volgende tabellen worden de items vermeld die worden vermeld in [de bovenstaande](#new-rules-for-company-name-and-email-address) sectie nieuwe regels.

### <a name="table-of-special-characters"></a>Tabel met speciale tekens

| Tekens. | Tekens. | Tekens. | Tekens. |
| ----- | ----- | -----| ----- |
| '~' | '-' |  '=' |  '_' |
|  '#' | '.' |  '%' |  '-' |
|  '+' |  ':' |  '^' |  '[' |
|  '$' |  '–' |  '&' |  ']' |
|  '@' |  '—' |  '*' |  '(' |
|  ',' |  ')' |  '”' |  '⟩' |
|  '`' |  '<' |  '!' |  '\\' |
|  '(' |  '>' |  '“' |  '/' |
|  ')' |  '{' |  '‘' |  '\|' |
|  '\' |  '}' |  '،' |  ':' |
|  ';' |  '⟨' |  '’' | '?' |
|  '”' |  '⟩' |  '\\' |  |


### <a name="table-of-abbreviations"></a>Tabel met afkortingen

| Afgekort. | Afgekort. | Afgekort. | Afgekort. |
| ----- | ----- | ----- | ----- |
|"c p a" | pty | "l. l. c." | gmbh |
| "c.p.a." | "pty ltd" | "l.l.c." | ". |
| l.l.p. | "pte ltd" | " l l p" | "wll" |
| "c. p. a." | 'beperkte privé' | corp | "lda" |
| "l. l. p." | "pvt" | "corporation" | "sarl" |
| " l l c" | "pvt ltd" | "inc" | "kft" |
| 'corp'. | "zrt" | "opgenomen" | ltd |
| 'llc'. | "ooo" | 'beperkt' | ltd. |
| 'llp'. | "llp" | "llc" | "sdn kunt u"

### <a name="table-of-top-level-domain-extensions"></a>Tabel met domeinextensies op het hoogste niveau

| Ext.  | Ext.  | Ext.  | Ext. |
| ----- | ----- | ----- | ----- |
| .ac | .ba | .ca | .de |
| .ad | .bb | .cc | .dj |
| .ae | .bd | .cd | .dk |
| .af | .be | .cf | .dm |
| .ag | .bf | .cg | .do |
| .ai | .bg | .ch | .dz |
| .al | .kunt u | .ci | .fm |
| .am | .bi | .ck | .fo |
| .an | .kunt u | .cl | .fr |
| .ao | .bl | .cm | .ga |
| .aq | .bm | .cn | .gb |
| .ar | .bn | .co | .gd |
| .as | .bo | .cr | .ge |
| .at | .bq | .cu | .gf |
| .au | .br | .cv | .gg |
| .aw | .bs | .cw | .gh |
| .ax | .bt | .cx | .gi |
| .az | .nl | .cy | .gl |
| .ec | .bw | . gaan | .gm |
| .ee | .by | .eu | .gn |
| .eg | .bz | .fi | .gp |
| .eh | .es | .fj | .gq |
| .er | .et | .fk | .gr |
| .gs | .gw | .hm | .ht |
| .gt | .der | .hn | .hu |
| .gu | .hk | .hr | .id |
| .ie | .kz | .mo | .nz |
| .il | .la | .mp | .om |
| .im | .lb | .mq | .pa |
| .in | .lc | .mr | .pe |
| .io | .li | .ms | .pf |
| .iq | . | .mt | .pg |
| .ir | .lr | .mu | .ph |
| .is | .ls | .mv | .pk |
| .it | .lt | . | .pl |
| .je | .lu | .mx | .pm |
| .jm | .lv | .my | .pn |
| .jo | .ly | .mz | .pr |
| .jp | .ma | .na | .ps |
| .ke | .mc | .nc | .pt |
| .kg | .md | .ne | .pw |
| .kh | .me | .nf | .py |
| .ki | .mf | .ng | .qa |
| .km | .mg | .ni | .re |
| .kn | .mh | .nl | .ro |
| .kp | .mk | .no | .rs |
| .kr | .ml | .np | .ru |
| .kw | .mm | .nr | .rw |
| .ky | .mn | .nu | .sa |
| .sb | .tf | .vc | .中国 |
| .sc | .tg | .ve | .中國 |
| .sd | .th | .vg | .భారత్ |
| .se | .tj | .vi | .ලංකා |
| .sg | .tk | .vn | .ભારત |
| .sh | .tl | .vu | .भारतम् |
| .si | .tm | .wf | .भारत |
| .sj | .tn | .ws | .भारोत |
| .sk | .to | .ಭಾರತ | .укр |
| .sl | .tp | .한국 | .香港 |
| .sm | .tr | .ଭାରତ | .台湾 |
| .sn | .tt | .ভাৰত | .台灣 |
| .so | .tv | .ভারত | .мон |
| .sr | .tw | .சிங்கப்பூர் | .tc |
| .ss | .tz | .sz | .td |
| .st | .ua | .বাংলা | .uz |
| .su | .ug | .қаз | .va |
| .sv | .uk | .срб | .мкд |
| .sx | .um | .бг | .ею |
| .sy | .us | .бел | Uy |
| .tc | .uz | .мкд |  |

## <a name="next-steps"></a>Volgende stappen

- Zie Partneraanbiedingen in het Cloud Solution Provider-programma voor meer informatie over wat u aan klanten kunt verkopen via het [Cloud Solution Provider-programma](csp-offers.md)

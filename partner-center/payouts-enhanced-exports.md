---
title: Gegevenspagina uitbetalingen exporteren
description: Legt uit hoe u de verbeterde pagina met exportgegevens gebruikt om aangepaste transactiegeschiedenisrapporten te genereren
author: Satinder37
ms.author: sabajaj
ms.topic: how-to
ms.date: 10/04/2021
ms.custom: template-how-to
ms.openlocfilehash: 9ac19a8ea42020b4ec2543d9f4ef197eb95e3a61
ms.sourcegitcommit: cf8c78e0c8831371432007d5ab05f934f15a77b5
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 10/05/2021
ms.locfileid: "129528613"
---
# <a name="payouts-export-data-page"></a>Gegevenspagina uitbetalingen exporteren
**Juiste rollen:** Incentives-| Incentives-gebruiker

In dit artikel worden verbeteringen in de ervaring voor het exporteren van gegevens voor **uitbetalingen** in Partner Center. Deze begeleide ervaring biedt nieuwe standaardsjablonen voor het exporteren van uw transactiegeschiedenisrapporten. Het biedt ook de dynamische mogelijkheid om uw eigen aangepaste sjablonen te maken voor uw transactiegeschiedenisrapporten.

## <a name="access-the-export-data-page"></a>De pagina Gegevens exporteren openen
1.  Meld u aan bij het [dashboard van het Partnercentrum](https://partner.microsoft.com/dashboard/home).
2.  Selecteer **Uitbetalingen** en selecteer vervolgens **Incentive-export** of **Transactiegeschiedenis** in het menu.

> [!Note] 
> U hebt toegang tot deze pagina als u een [incentive-beheerder of incentive-gebruiker bent.](/payout-statement#roles-and-permissionsData) Wat u ziet, is afhankelijk van welke MPN-combinaties (program en Microsoft Partner Network) u toegang hebt (vergelijkbaar met transactiegeschiedenis **en** **betalingspagina's).**

## <a name="export-your-data"></a>Uw gegevens exporteren
1.   Selecteer het type gegevens dat u wilt exporteren. 
      - Voor een transactiegeschiedenisrapport selecteert u **Inkomsten, transactie, betalingsstatusdetails.**  Houd er rekening **mee dat details over inkomsten, transacties en betalingsstatussen (groeimogelijkheden)** niet van toepassing zijn op commerciële marketplaces. 
      - Selecteer Betalingsgegevens voor een **betalingsrapport.**
   :::image type="content" source="images/payouts/type-of-data.png" lightbox="images/payouts/type-of-data.png" alt-text="Schermopname van het type gegevensselecties.":::

2.   Selecteer een rapportsjabloontype.

      :::image type="content" source="images/payouts/report-template-type.png" lightbox="images/payouts/report-template-type.png" alt-text="Schermopname van selecties voor rapportsjabloonsjablonen.":::

      Uw keuze voor stap 1 bepaalt de sjabloonopties voor stap 2. Als u bijvoorbeeld **Inkomsten, transactie en** betalingsstatusdetails in stap 1 selecteert, ziet u vier verschillende sjabloonopties:
      - **Standaardtransactiegeschiedenis:** dit rapport bevat alle mogelijke kenmerken die beschikbaar zijn in het rapport voor alle programma's (incentives, commerciële en consumentenmarktinstellingen). Dit was de downloadsjabloon die beschikbaar was vóór oktober 2021.
      - **Standaardmarktplaats:** dit rapport bevat alle kenmerken die vereist zijn voor MPN-leden die zijn ingeschreven in commerciële marketplace-programma's, zoals Azure Marketplace. 
      - **Standaardopslag:** dit rapport bevat alle kenmerken die vereist zijn voor MPN-leden die zijn ingeschreven in de consumentenwinkelprogramma's, zoals Microsoft Store, Minecraft en MS Flight Simulator. 
      - **Aangepaste transactiegeschiedenis:** met dit rapport kunt u uw transactiegeschiedenisrapport aanpassen.

      Als u in stap 1 **inkomsten-,** transactie- en betalingsstatusgegevens  selecteert, kunt u in stap 2 de sjabloon Transactieoverzicht selecteren. Als u **betalingsgegevens** selecteert in stap 1, ziet u één sjabloon 'Betalingen' in stap 2. Als u in stap 1 **AGI-omzetgegevens** selecteert,  kunt u  kiezen tussen de omzet van het programma of de klant voegt sjablonen toe in stap 2.

3. Selecteer een rapportbestandsindeling.
   
      :::image type="content" source="images/payouts/report-file-format.png" lightbox="images/payouts/report-file-format.png" alt-text="Schermopname met selecties voor rapportbestandsindelingen.":::

4.   Kies uw tijdsperiode en pas eventuele andere filters toe. Selecteer **vervolgens Gegevens downloaden.**
   
      :::image type="content" source="images/payouts/time-period-filters.png" lightbox="images/payouts/time-period-filters.png" alt-text="Schermopname van de selectie en filteroptie voor de rapportperiode.":::

> [!Note] 
> U kunt gegevens exporteren en aanvragen beheren vanuit de **tabel Aanvragen** downloaden.

## <a name="create-your-customized-transaction-history-report"></a>Uw aangepaste transactiegeschiedenisrapport maken

Pas uw afstemmingsrapport voor transactiegeschiedenis aan uw behoeften aan. U kunt maximaal vijf rapportsjablonen maken en beheren. 

1.  Selecteer **+ Aangepaste transactiegeschiedenis om** een nieuwe afstemmingssjabloon in te stellen. 
   
      :::image type="content" source="images/payouts/custom-trans-history.png" lightbox="images/payouts/custom-trans-history.png" alt-text="Schermopname van de configuratie van de aangepaste transactiegeschiedenis.":::


2.   Voer een sjabloonnaam en een korte beschrijving in en **selecteer** volgende.
   
      :::image type="content" source="images/payouts/template-name.png" lightbox="images/payouts/template-name.png" alt-text="Schermopname van nieuwe aangepaste afstemmingssjabloonvelden.":::


3.  Selecteer de gegevenskolommen die u wilt opnemen en bekijk de standaardkolommen die al in het rapport worden vermeld. Selecteer **Next**.
   
     :::image type="content" source="images/payouts/data-selection.png" lightbox="images/payouts/data-selection.png" alt-text="Schermopname met nieuwe opties voor gegevensselectie voor aangepaste afstemmingssjabloon.":::

4.  Controleer de sjabloondetails en gegevensselecties, bewerk deze indien nodig en selecteer **vervolgens Aangepaste sjabloon maken.**
   
      :::image type="content" source="images/payouts/new-custom-template.png" lightbox="images/payouts/new-custom-template.png" alt-text="Schermopname van het bevestigingsscherm voor een nieuwe aangepaste afstemmingssjabloon.":::

5.  Selecteer **Downloaden** in het volgende scherm om uw gegevens te exporteren. U kunt ook andere sjablonen in dit scherm toevoegen, bewerken, downloaden of verwijderen.
   
      :::image type="content" source="images/payouts/download-manage-templates.png" lightbox="images/payouts/download-manage-templates.png" alt-text="Schermopname van het beheren van sjablonen en het downloaden van gegevensopties.":::

## <a name="next-steps"></a>Volgende stappen
- [Overzicht van uitbetalingen](non-payment-fraud-misuse.md)
- [Samenvatting van omzet](revenue-summary.md)
- [Uitbetalingsinstructies](payout-statement.md)
- [Veelvoorkomende vragen over uitbetalingen en belastingen](payout-faq.yml)

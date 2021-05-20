---
title: Meerdere gebruikers toevoegen voor een klantaccount
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Als u meerdere gebruikers wilt toevoegen aan het account van een klant, uploadt u een gegevensbestand naar Partner Center met behulp van de bestandsindeling met door komma's gescheiden waarden (.csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150468"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="c1982-103">Een CSV-bestand van gebruikers uploaden naar het account van een klant</span><span class="sxs-lookup"><span data-stu-id="c1982-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="c1982-104">**Juiste rollen:** globale beheerder</span><span class="sxs-lookup"><span data-stu-id="c1982-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="c1982-105">Voeg meerdere gebruikers tegelijk toe aan het account van een klant door een gegevensbestand in de bestandsindeling met door komma's gescheiden waarden (.csv) te uploaden naar de Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c1982-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="c1982-106">Het bestand van klantgebruikers maken en uploaden naar het klantaccount</span><span class="sxs-lookup"><span data-stu-id="c1982-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="c1982-107">Maak een csv-gegevensbestand (door komma's gescheiden waarden) met de hierboven beschreven gegevens.</span><span class="sxs-lookup"><span data-stu-id="c1982-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="c1982-108">Sla het bestand op zodat u er in een latere stap naar kunt bladeren.</span><span class="sxs-lookup"><span data-stu-id="c1982-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="c1982-109">Zie [Velden voor CSV-bestand om meerdere gebruikers voor een klantaccount te importeren.](file-customer-users.md)</span><span class="sxs-lookup"><span data-stu-id="c1982-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="c1982-110">Meld u aan bij Partner Center [dashboard.](https://partner.microsoft.com/dashboard)</span><span class="sxs-lookup"><span data-stu-id="c1982-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="c1982-111">Selecteer in Partner Center menu **Klanten** en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="c1982-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="c1982-112">Selecteer het tabblad Gebruikers en **licenties van de** klant en selecteer vervolgens Gebruikers **uploaden.**</span><span class="sxs-lookup"><span data-stu-id="c1982-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="c1982-113">Selecteer **onder Gebruikersgegevens uploaden** de optie **Bladeren.**</span><span class="sxs-lookup"><span data-stu-id="c1982-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="c1982-114">Selecteer in de bestands selector uw gegevensbestand en selecteer vervolgens **Openen.**</span><span class="sxs-lookup"><span data-stu-id="c1982-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="c1982-115">Selecteer **Valideren**.</span><span class="sxs-lookup"><span data-stu-id="c1982-115">Select **Validate**.</span></span>

    <span data-ttu-id="c1982-116">**Opmerking**  De meeste fouten bij het maken van een account worden veroorzaakt door problemen met gegevensbestanden, waaronder ontbrekende gegevens, onjuist vorm geven of gedupliceerde e-mailadressen of te veel records in het bestand.</span><span class="sxs-lookup"><span data-stu-id="c1982-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="c1982-117">Nadat het Partner Center bestand is gevalideerd, selecteert u de geografische **locatie** voor de nieuwe gebruikers.</span><span class="sxs-lookup"><span data-stu-id="c1982-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="c1982-118">Selecteer **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="c1982-118">Select **Save**.</span></span>
10. <span data-ttu-id="c1982-119">Download de tijdelijke wachtwoordgegevens voor de gebruikers.</span><span class="sxs-lookup"><span data-stu-id="c1982-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="c1982-120">Zorg ervoor dat u het bestand nu downloadt met de tijdelijke wachtwoorden, aangezien u dit later niet meer kunt doen.</span><span class="sxs-lookup"><span data-stu-id="c1982-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="c1982-121">Nieuwe gebruikers moeten zich aanmelden bij hun nieuwe account met het tijdelijke wachtwoord voor hun nieuwe accounts.</span><span class="sxs-lookup"><span data-stu-id="c1982-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="c1982-122">Nieuwe gebruikers krijgen automatisch machtigingen toegewezen van **Kan licenties en services gebruiken.**</span><span class="sxs-lookup"><span data-stu-id="c1982-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="c1982-123">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="c1982-123">Next steps</span></span>

- [<span data-ttu-id="c1982-124">Klanten toestemming geven om Partner Center eigen producten of services te kopen</span><span class="sxs-lookup"><span data-stu-id="c1982-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)

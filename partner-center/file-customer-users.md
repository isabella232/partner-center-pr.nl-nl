---
title: Velden voor CSV-bestand voor het importeren van meerdere gebruikers voor een klantaccount
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Als u meerdere gebruikers wilt toevoegen aan een klantaccount, maakt u een bestand met door komma's gescheiden waarden (CSV) met de juiste velden.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150978"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="c43c9-103">Meerdere gebruikers toevoegen aan een klantaccount door een CSV-bestand te maken</span><span class="sxs-lookup"><span data-stu-id="c43c9-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="c43c9-104">**Juiste rollen:** globale beheerder</span><span class="sxs-lookup"><span data-stu-id="c43c9-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="c43c9-105">Voeg meerdere gebruikers tegelijk toe aan het account van een klant door een gegevensbestand in de bestandsindeling met door komma's gescheiden waarden (.csv) te uploaden naar de Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c43c9-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="c43c9-106">U kunt een voorbeeldgegevensbestand downloaden van de Partner Center en het vervolgens bewerken voor uw gebruik, of u kunt een nieuw gegevensbestand maken met behulp van het gegevensmodel dat hieronder is gedefinieerd.</span><span class="sxs-lookup"><span data-stu-id="c43c9-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="c43c9-107">Vereisten voor gegevensbestand</span><span class="sxs-lookup"><span data-stu-id="c43c9-107">Data file requirements</span></span>

<span data-ttu-id="c43c9-108">Als u meerdere gebruikers wilt toevoegen aan het account van een klant met behulp van het proces voor bulksgewijs uploaden, moet u aan de volgende vereisten voldoen:</span><span class="sxs-lookup"><span data-stu-id="c43c9-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="c43c9-109">U moet globale beheerdersmachtigingen hebben voor het klantaccount;</span><span class="sxs-lookup"><span data-stu-id="c43c9-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="c43c9-110">Elke gebruiker moet een uniek e-mailadres hebben dat is toegevoegd aan de e-maildomeinen van de klant;</span><span class="sxs-lookup"><span data-stu-id="c43c9-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="c43c9-111">U kunt maximaal 100 records tegelijk uploaden.</span><span class="sxs-lookup"><span data-stu-id="c43c9-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="c43c9-112">Als u meer dan 100 gebruikers wilt toevoegen, maakt en uploadt u aanvullende gegevensbestanden.</span><span class="sxs-lookup"><span data-stu-id="c43c9-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="c43c9-113">Alle gebruikers moeten zich in dezelfde geografische **locatie bevinden.**</span><span class="sxs-lookup"><span data-stu-id="c43c9-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="c43c9-114">Voer alleen de gegevens in die hieronder worden beschreven.</span><span class="sxs-lookup"><span data-stu-id="c43c9-114">Enter only the data described below.</span></span> <span data-ttu-id="c43c9-115">Overbodige gegevens zorgen ervoor dat het uploaden mislukt.</span><span class="sxs-lookup"><span data-stu-id="c43c9-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="c43c9-116">Voer de volgende gegevens in het gegevensbestand in:</span><span class="sxs-lookup"><span data-stu-id="c43c9-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="c43c9-117">**Kolomnaam**</span><span class="sxs-lookup"><span data-stu-id="c43c9-117">**Column name**</span></span> | <span data-ttu-id="c43c9-118">**Beschrijving**</span><span class="sxs-lookup"><span data-stu-id="c43c9-118">**Description**</span></span>  | <span data-ttu-id="c43c9-119">**Beperking**</span><span class="sxs-lookup"><span data-stu-id="c43c9-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="c43c9-120">Voornaam</span><span class="sxs-lookup"><span data-stu-id="c43c9-120">First name</span></span>  | <span data-ttu-id="c43c9-121">Voornaam van gebruiker (optioneel veld)</span><span class="sxs-lookup"><span data-stu-id="c43c9-121">User's first name (optional field)</span></span>  | <span data-ttu-id="c43c9-122">Limiet van 50 tekens</span><span class="sxs-lookup"><span data-stu-id="c43c9-122">50-character limit</span></span>  |
| <span data-ttu-id="c43c9-123">Achternaam</span><span class="sxs-lookup"><span data-stu-id="c43c9-123">Last name</span></span>  | <span data-ttu-id="c43c9-124">Achternaam van gebruiker (optioneel veld)</span><span class="sxs-lookup"><span data-stu-id="c43c9-124">User's last name (optional field)</span></span>  | <span data-ttu-id="c43c9-125">Limiet van 50 tekens</span><span class="sxs-lookup"><span data-stu-id="c43c9-125">50-character limit</span></span>  |
| <span data-ttu-id="c43c9-126">Weergavenaam</span><span class="sxs-lookup"><span data-stu-id="c43c9-126">Display name</span></span>    | <span data-ttu-id="c43c9-127">Naam die wordt weergegeven in het Partner Center (vereist veld)</span><span class="sxs-lookup"><span data-stu-id="c43c9-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="c43c9-128">Limiet van 50 tekens</span><span class="sxs-lookup"><span data-stu-id="c43c9-128">50-character limit</span></span>                         |
| <span data-ttu-id="c43c9-129">E-mail</span><span class="sxs-lookup"><span data-stu-id="c43c9-129">Email</span></span>   | <span data-ttu-id="c43c9-130">Het zakelijke e-mailadres van de gebruiker bij het klantbedrijf (vereist veld)</span><span class="sxs-lookup"><span data-stu-id="c43c9-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="c43c9-131">Elke gebruiker moet een uniek e-mailadres hebben</span><span class="sxs-lookup"><span data-stu-id="c43c9-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="c43c9-132">Statusupdate</span><span class="sxs-lookup"><span data-stu-id="c43c9-132">Status update</span></span>   | <span data-ttu-id="c43c9-133">Wordt gebruikt om aan te geven of de nieuwe gebruikersrecord is gemaakt</span><span class="sxs-lookup"><span data-stu-id="c43c9-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="c43c9-134">\*\*Leeg laten\*\*</span><span class="sxs-lookup"><span data-stu-id="c43c9-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="c43c9-135">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="c43c9-135">Next steps</span></span>

- [<span data-ttu-id="c43c9-136">Meerdere gebruikers toevoegen voor een klant</span><span class="sxs-lookup"><span data-stu-id="c43c9-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)
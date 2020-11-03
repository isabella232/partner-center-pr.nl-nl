---
title: Velden voor CSV-bestand voor het importeren van meerdere gebruikers voor een klant account
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Als u meerdere gebruikers aan een klant account wilt toevoegen, maakt u een bestand met door komma's gescheiden waarden (. CSV) met de juiste velden.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 08/03/2020
ms.locfileid: "92528096"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="b7e21-103">Meerdere gebruikers toevoegen aan een klant account door een CSV-bestand te maken</span><span class="sxs-lookup"><span data-stu-id="b7e21-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="b7e21-104">**Van toepassing op**</span><span class="sxs-lookup"><span data-stu-id="b7e21-104">**Applies to**</span></span>

- <span data-ttu-id="b7e21-105">Partnercentrum</span><span class="sxs-lookup"><span data-stu-id="b7e21-105">Partner Center</span></span>

<span data-ttu-id="b7e21-106">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="b7e21-106">**Appropriate roles**</span></span>

- <span data-ttu-id="b7e21-107">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="b7e21-107">Global admin</span></span>

<span data-ttu-id="b7e21-108">Voeg meerdere gebruikers tegelijk aan het account van een klant toe door een gegevens bestand in de bestands indeling met door komma's gescheiden waarden (. CSV) naar het partner centrum te uploaden.</span><span class="sxs-lookup"><span data-stu-id="b7e21-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="b7e21-109">U kunt een voorbeeld gegevensbestand downloaden van het partner centrum en het vervolgens bewerken voor uw gebruik. u kunt ook een nieuw gegevens bestand maken met behulp van het hieronder gedefinieerde gegevens model.</span><span class="sxs-lookup"><span data-stu-id="b7e21-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="b7e21-110">Vereisten voor het gegevens bestand</span><span class="sxs-lookup"><span data-stu-id="b7e21-110">Data file requirements</span></span>

<span data-ttu-id="b7e21-111">Als u meerdere gebruikers wilt toevoegen aan het account van een klant met behulp van het bulk upload proces, moet u aan de volgende vereisten voldoen:</span><span class="sxs-lookup"><span data-stu-id="b7e21-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="b7e21-112">U moet globale beheerders machtigingen hebben voor het klant account;</span><span class="sxs-lookup"><span data-stu-id="b7e21-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="b7e21-113">Elke gebruiker moet een uniek e-mail adres hebben dat is toegevoegd aan de e-mail domein (en) van de klant.</span><span class="sxs-lookup"><span data-stu-id="b7e21-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="b7e21-114">U kunt Maxi maal 100 records tegelijk uploaden.</span><span class="sxs-lookup"><span data-stu-id="b7e21-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="b7e21-115">Als u meer dan 100 gebruikers wilt toevoegen, maakt en uploadt u extra gegevens bestanden.</span><span class="sxs-lookup"><span data-stu-id="b7e21-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="b7e21-116">Alle gebruikers moeten zich op dezelfde geografische **locatie** bestaan.</span><span class="sxs-lookup"><span data-stu-id="b7e21-116">All users must be in the same geographic **Location** .</span></span>
- <span data-ttu-id="b7e21-117">Voer alleen de gegevens in die hieronder worden beschreven.</span><span class="sxs-lookup"><span data-stu-id="b7e21-117">Enter only the data described below.</span></span> <span data-ttu-id="b7e21-118">Externe gegevens zorgen ervoor dat het uploaden mislukt.</span><span class="sxs-lookup"><span data-stu-id="b7e21-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="b7e21-119">Voer de volgende gegevens in het gegevens bestand in:</span><span class="sxs-lookup"><span data-stu-id="b7e21-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="b7e21-120">**Kolomnaam**</span><span class="sxs-lookup"><span data-stu-id="b7e21-120">**Column name**</span></span> | <span data-ttu-id="b7e21-121">**Beschrijving**</span><span class="sxs-lookup"><span data-stu-id="b7e21-121">**Description**</span></span>  | <span data-ttu-id="b7e21-122">**Beperking**</span><span class="sxs-lookup"><span data-stu-id="b7e21-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="b7e21-123">Voornaam</span><span class="sxs-lookup"><span data-stu-id="b7e21-123">First name</span></span>  | <span data-ttu-id="b7e21-124">De voor naam van de gebruiker (optioneel veld)</span><span class="sxs-lookup"><span data-stu-id="b7e21-124">User's first name (optional field)</span></span>  | <span data-ttu-id="b7e21-125">50-teken limiet</span><span class="sxs-lookup"><span data-stu-id="b7e21-125">50-character limit</span></span>  |
| <span data-ttu-id="b7e21-126">Achternaam</span><span class="sxs-lookup"><span data-stu-id="b7e21-126">Last name</span></span>  | <span data-ttu-id="b7e21-127">De achternaam van de gebruiker (optioneel veld)</span><span class="sxs-lookup"><span data-stu-id="b7e21-127">User's last name (optional field)</span></span>  | <span data-ttu-id="b7e21-128">50-teken limiet</span><span class="sxs-lookup"><span data-stu-id="b7e21-128">50-character limit</span></span>  |
| <span data-ttu-id="b7e21-129">Weergavenaam</span><span class="sxs-lookup"><span data-stu-id="b7e21-129">Display name</span></span>    | <span data-ttu-id="b7e21-130">De naam die wordt weer gegeven in het partner centrum (vereist veld)</span><span class="sxs-lookup"><span data-stu-id="b7e21-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="b7e21-131">50-teken limiet</span><span class="sxs-lookup"><span data-stu-id="b7e21-131">50-character limit</span></span>                         |
| <span data-ttu-id="b7e21-132">E-mail</span><span class="sxs-lookup"><span data-stu-id="b7e21-132">Email</span></span>   | <span data-ttu-id="b7e21-133">Zakelijke e-mail adres van gebruiker bij bedrijf van klant (vereist veld)</span><span class="sxs-lookup"><span data-stu-id="b7e21-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="b7e21-134">Elke gebruiker moet een uniek e-mail adres hebben</span><span class="sxs-lookup"><span data-stu-id="b7e21-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="b7e21-135">Status update</span><span class="sxs-lookup"><span data-stu-id="b7e21-135">Status update</span></span>   | <span data-ttu-id="b7e21-136">Hiermee wordt aangegeven of de nieuwe gebruikers record is gemaakt.</span><span class="sxs-lookup"><span data-stu-id="b7e21-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="b7e21-137">\*\*Leeg laten\*\*</span><span class="sxs-lookup"><span data-stu-id="b7e21-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="b7e21-138">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="b7e21-138">Next steps</span></span>

- [<span data-ttu-id="b7e21-139">Meerdere gebruikers toevoegen aan een klant</span><span class="sxs-lookup"><span data-stu-id="b7e21-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)
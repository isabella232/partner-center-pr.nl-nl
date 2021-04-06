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
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441418"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="3f697-103">Meerdere gebruikers toevoegen aan een klant account door een CSV-bestand te maken</span><span class="sxs-lookup"><span data-stu-id="3f697-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="3f697-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="3f697-104">**Appropriate roles**</span></span>

- <span data-ttu-id="3f697-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="3f697-105">Global admin</span></span>

<span data-ttu-id="3f697-106">Voeg meerdere gebruikers tegelijk aan het account van een klant toe door een gegevens bestand in de bestands indeling met door komma's gescheiden waarden (. CSV) naar het partner centrum te uploaden.</span><span class="sxs-lookup"><span data-stu-id="3f697-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="3f697-107">U kunt een voorbeeld gegevensbestand downloaden van het partner centrum en het vervolgens bewerken voor uw gebruik. u kunt ook een nieuw gegevens bestand maken met behulp van het hieronder gedefinieerde gegevens model.</span><span class="sxs-lookup"><span data-stu-id="3f697-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="3f697-108">Vereisten voor het gegevens bestand</span><span class="sxs-lookup"><span data-stu-id="3f697-108">Data file requirements</span></span>

<span data-ttu-id="3f697-109">Als u meerdere gebruikers wilt toevoegen aan het account van een klant met behulp van het bulk upload proces, moet u aan de volgende vereisten voldoen:</span><span class="sxs-lookup"><span data-stu-id="3f697-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="3f697-110">U moet globale beheerders machtigingen hebben voor het klant account;</span><span class="sxs-lookup"><span data-stu-id="3f697-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="3f697-111">Elke gebruiker moet een uniek e-mail adres hebben dat is toegevoegd aan de e-mail domein (en) van de klant.</span><span class="sxs-lookup"><span data-stu-id="3f697-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="3f697-112">U kunt Maxi maal 100 records tegelijk uploaden.</span><span class="sxs-lookup"><span data-stu-id="3f697-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="3f697-113">Als u meer dan 100 gebruikers wilt toevoegen, maakt en uploadt u extra gegevens bestanden.</span><span class="sxs-lookup"><span data-stu-id="3f697-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="3f697-114">Alle gebruikers moeten zich op dezelfde geografische **locatie** bestaan.</span><span class="sxs-lookup"><span data-stu-id="3f697-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="3f697-115">Voer alleen de gegevens in die hieronder worden beschreven.</span><span class="sxs-lookup"><span data-stu-id="3f697-115">Enter only the data described below.</span></span> <span data-ttu-id="3f697-116">Externe gegevens zorgen ervoor dat het uploaden mislukt.</span><span class="sxs-lookup"><span data-stu-id="3f697-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="3f697-117">Voer de volgende gegevens in het gegevens bestand in:</span><span class="sxs-lookup"><span data-stu-id="3f697-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="3f697-118">**Kolomnaam**</span><span class="sxs-lookup"><span data-stu-id="3f697-118">**Column name**</span></span> | <span data-ttu-id="3f697-119">**Beschrijving**</span><span class="sxs-lookup"><span data-stu-id="3f697-119">**Description**</span></span>  | <span data-ttu-id="3f697-120">**Beperking**</span><span class="sxs-lookup"><span data-stu-id="3f697-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="3f697-121">Voornaam</span><span class="sxs-lookup"><span data-stu-id="3f697-121">First name</span></span>  | <span data-ttu-id="3f697-122">De voor naam van de gebruiker (optioneel veld)</span><span class="sxs-lookup"><span data-stu-id="3f697-122">User's first name (optional field)</span></span>  | <span data-ttu-id="3f697-123">50-teken limiet</span><span class="sxs-lookup"><span data-stu-id="3f697-123">50-character limit</span></span>  |
| <span data-ttu-id="3f697-124">Achternaam</span><span class="sxs-lookup"><span data-stu-id="3f697-124">Last name</span></span>  | <span data-ttu-id="3f697-125">De achternaam van de gebruiker (optioneel veld)</span><span class="sxs-lookup"><span data-stu-id="3f697-125">User's last name (optional field)</span></span>  | <span data-ttu-id="3f697-126">50-teken limiet</span><span class="sxs-lookup"><span data-stu-id="3f697-126">50-character limit</span></span>  |
| <span data-ttu-id="3f697-127">Weergavenaam</span><span class="sxs-lookup"><span data-stu-id="3f697-127">Display name</span></span>    | <span data-ttu-id="3f697-128">De naam die wordt weer gegeven in het partner centrum (vereist veld)</span><span class="sxs-lookup"><span data-stu-id="3f697-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="3f697-129">50-teken limiet</span><span class="sxs-lookup"><span data-stu-id="3f697-129">50-character limit</span></span>                         |
| <span data-ttu-id="3f697-130">E-mail</span><span class="sxs-lookup"><span data-stu-id="3f697-130">Email</span></span>   | <span data-ttu-id="3f697-131">Zakelijke e-mail adres van gebruiker bij bedrijf van klant (vereist veld)</span><span class="sxs-lookup"><span data-stu-id="3f697-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="3f697-132">Elke gebruiker moet een uniek e-mail adres hebben</span><span class="sxs-lookup"><span data-stu-id="3f697-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="3f697-133">Status update</span><span class="sxs-lookup"><span data-stu-id="3f697-133">Status update</span></span>   | <span data-ttu-id="3f697-134">Wordt gebruikt om aan te geven of de nieuwe gebruikers record is gemaakt</span><span class="sxs-lookup"><span data-stu-id="3f697-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="3f697-135">\*\*Leeg laten\*\*</span><span class="sxs-lookup"><span data-stu-id="3f697-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="3f697-136">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="3f697-136">Next steps</span></span>

- [<span data-ttu-id="3f697-137">Meerdere gebruikers toevoegen aan een klant</span><span class="sxs-lookup"><span data-stu-id="3f697-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)
---
title: Gebruikers voor klant accounts beheren
ms.topic: how-to
ms.date: 02/25/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: 'Gebruikers beheren voor uw klanten in Partner Center: gebruikers accounts maken, gebruikers licenties toevoegen of verwijderen, wacht woorden opnieuw instellen en gebruikers accounts verwijderen of herstellen.'
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 0e2bb4ceb146174da83e9c08a9ff030380298bd0
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: nl-NL
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756087"
---
# <a name="manage-users-and-user-licenses-for-customer-accounts"></a><span data-ttu-id="68921-103">Gebruikers en gebruikers licenties voor klant accounts beheren</span><span class="sxs-lookup"><span data-stu-id="68921-103">Manage users and user licenses for customer accounts</span></span> 

<span data-ttu-id="68921-104">**Juiste rollen**</span><span class="sxs-lookup"><span data-stu-id="68921-104">**Appropriate roles**</span></span>

- <span data-ttu-id="68921-105">Globale beheerder</span><span class="sxs-lookup"><span data-stu-id="68921-105">Global admin</span></span>
- <span data-ttu-id="68921-106">Beheerder van gebruikers beheer</span><span class="sxs-lookup"><span data-stu-id="68921-106">User management admin</span></span>
- <span data-ttu-id="68921-107">Beheer agent</span><span class="sxs-lookup"><span data-stu-id="68921-107">Admin agent</span></span>


<span data-ttu-id="68921-108">U kunt nieuwe gebruikers maken en verwijderen in het account van een klant.</span><span class="sxs-lookup"><span data-stu-id="68921-108">You can create and delete new users in a customer's account.</span></span> <span data-ttu-id="68921-109">U kunt ook een of meer gebruikers accounts die u eerder hebt verwijderd binnen 30 dagen na de verwijdering herstellen.</span><span class="sxs-lookup"><span data-stu-id="68921-109">You can also restore one or more user accounts that you previously deleted within 30 days of the deletion.</span></span> <span data-ttu-id="68921-110">De vorige abonnements toewijzingen van de gebruiker worden ook teruggezet (ervan uitgaande dat hun vorige toewijzing beschikbaar is).</span><span class="sxs-lookup"><span data-stu-id="68921-110">The user's previous subscription assignments will also be restored (assuming their previous allocations are available).</span></span>

<span data-ttu-id="68921-111">Wanneer u nieuwe abonnementen voor een klant koopt, moet de klant u een lijst geven met alle gebruikers die accounts moeten, hun gebruikers machtigingen en welke services elke gebruiker nodig heeft.</span><span class="sxs-lookup"><span data-stu-id="68921-111">When you buy new subscriptions for a customer, the customer should give you a list of all the users who will need accounts, their user permissions, and which services each user needs.</span></span>  

>[!NOTE]
><span data-ttu-id="68921-112">In het gedeelte **gebruikers en licenties** van het tabblad **klant** worden alle gebruikers weer gegeven die zijn gemaakt in een Tenant van een specifieke klant, met inbegrip van gebruikers die licenties hebben gekocht van een andere CSP-partner of van een ander aankoop kanaal.</span><span class="sxs-lookup"><span data-stu-id="68921-112">The **Users and licenses** section of **Customer** tab shows all users created in a specific customer’s tenant, including users that have licenses purchased from another CSP partner or from another purchasing channel.</span></span>

<span data-ttu-id="68921-113">U kunt [abonnementen toewijzen aan meerdere gebruikers](bulk-license-provisioning-for-multiple-users.md) tegelijk door de namen te importeren met behulp van een [Excel-compatibel CSV-werk blad bestand](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="68921-113">You can [assign subscriptions to multiple users](bulk-license-provisioning-for-multiple-users.md) at one time by importing the names using an [Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span>

<a href="" id="createuseraccounts"></a>

## <a name="create-user-accounts-for-a-customer"></a><span data-ttu-id="68921-114">Gebruikersaccounts maken voor een klant</span><span class="sxs-lookup"><span data-stu-id="68921-114">Create user accounts for a customer</span></span>

1. <span data-ttu-id="68921-115">Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.</span><span class="sxs-lookup"><span data-stu-id="68921-115">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="68921-116">Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="68921-116">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="68921-117">Selecteer **gebruikers en licenties** in het menu klant.</span><span class="sxs-lookup"><span data-stu-id="68921-117">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="68921-118">Voor elke gebruiker die u toevoegt, selecteert u **abonnement toevoegen** en vult u vervolgens de informatie in, met inbegrip van machtigingen en licenties.</span><span class="sxs-lookup"><span data-stu-id="68921-118">For each user you add, select **Add subscription**, then fill out the information, including permissions and licenses.</span></span> <span data-ttu-id="68921-119">U moet vervolgens de wijzigingen **Opslaan**.</span><span class="sxs-lookup"><span data-stu-id="68921-119">**Save** your changes.</span></span>

5. <span data-ttu-id="68921-120">Zorg ervoor dat u de gebruikers naam en het tijdelijke wacht woord noteert om naar de gebruiker te verzenden.</span><span class="sxs-lookup"><span data-stu-id="68921-120">Be sure to record the user name and temporary password to send to the user.</span></span>

6. <span data-ttu-id="68921-121">Als u meerdere gebruikers per keer toevoegt, gebruikt u **een andere gebruiker toevoegen**.</span><span class="sxs-lookup"><span data-stu-id="68921-121">If you are adding multiple users one at a time use **Add another user**.</span></span>

7. <span data-ttu-id="68921-122">U kunt ook meerdere gebruikers tegelijk toevoegen door [een Excel-compatibel CSV-werkblad bestand te importeren](adding-multiple-users-to-a-customer-account.md).</span><span class="sxs-lookup"><span data-stu-id="68921-122">You can also add multiple users at once by [importing an Excel-compatible .csv spreadsheet file](adding-multiple-users-to-a-customer-account.md).</span></span> <span data-ttu-id="68921-123">U kunt wachten tot u klaar bent met de hele set voordat u de namen en wacht woorden in het bevestigings scherm e-mailt of afdrukt.</span><span class="sxs-lookup"><span data-stu-id="68921-123">You can wait until you're done with the whole set before emailing or printing the names and passwords from the confirmation screen.</span></span>

<a href="" id="userlicensing"></a>

## <a name="add-or-remove-user-licenses-for-a-customer"></a><span data-ttu-id="68921-124">Gebruikers licenties toevoegen aan of verwijderen uit een klant</span><span class="sxs-lookup"><span data-stu-id="68921-124">Add or remove user licenses for a customer</span></span>

<span data-ttu-id="68921-125">De volgende stappen zijn van toepassing op het toevoegen of verwijderen van gebruikers licenties voor micro soft-producten.</span><span class="sxs-lookup"><span data-stu-id="68921-125">The following steps apply to adding or removing user licenses for Microsoft products.</span></span> <span data-ttu-id="68921-126">Zie [licenties toevoegen of verwijderen voor een SaaS-abonnement](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription)om gebruikers licenties toe te voegen aan of te verwijderen voor SaaS-abonnementen op basis van licenties in de commerciële Marketplace.</span><span class="sxs-lookup"><span data-stu-id="68921-126">To add or remove user licenses for license-based SaaS subscriptions in the commercial marketplace, see [Add or remove licenses for a SaaS subscription](csp-commercial-marketplace-manage.md#add-or-remove-licenses-for-a-saas-subscription).</span></span>

1. <span data-ttu-id="68921-127">Meld u aan bij het [dash board](https://partner.microsoft.com/dashboard)van de partner centrum.</span><span class="sxs-lookup"><span data-stu-id="68921-127">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="68921-128">Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="68921-128">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="68921-129">Selecteer **gebruikers en licenties** in het menu klant.</span><span class="sxs-lookup"><span data-stu-id="68921-129">In the customer menu, select **Users and licenses**.</span></span>

4. <span data-ttu-id="68921-130">Kies een of meer gebruikers in de lijst.</span><span class="sxs-lookup"><span data-stu-id="68921-130">Choose one or more users from the list.</span></span> <span data-ttu-id="68921-131">Als de klant bijvoorbeeld zojuist nieuwe licenties heeft aangeschaft en u deze wilt toewijzen aan mensen die deze nog niet hebben, kunt u de optie **gebruikers filteren op...** gebruiken om de juiste groep te vinden.</span><span class="sxs-lookup"><span data-stu-id="68921-131">If, for example, the customer just purchased new licenses and you wanted to assign them to people who don't have them yet, you can use the **Filter users by...** option to find the right group.</span></span>

5. <span data-ttu-id="68921-132">Selecteer **licenties beheren**.</span><span class="sxs-lookup"><span data-stu-id="68921-132">Select **Manage licenses**.</span></span> <span data-ttu-id="68921-133">Breng uw wijzigingen aan en **Sla** het bestand op.</span><span class="sxs-lookup"><span data-stu-id="68921-133">Make your changes, then **Save**.</span></span>

> [!NOTE]
> <span data-ttu-id="68921-134">Voor [Azure Marketplace-Producten](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer)wordt licentie toewijzing en-activering beheerd via de onafhankelijke software leverancier (ISV) die het product heeft gepubliceerd.</span><span class="sxs-lookup"><span data-stu-id="68921-134">For [Azure Marketplace products](csp-commercial-marketplace-manage.md#assign-licenses-and-activate-a-subscription-on-behalf-of-a-customer), license assignment and activation is managed through the Independent Software Vendor (ISV) who published the product.</span></span>

<a href="" id="resetpassword"></a>

## <a name="reset-a-users-password-for-a-customer"></a><span data-ttu-id="68921-135">Het wacht woord van een gebruiker voor een klant opnieuw instellen</span><span class="sxs-lookup"><span data-stu-id="68921-135">Reset a user's password for a customer</span></span>

1. <span data-ttu-id="68921-136">Meld u aan bij het [dashboard](https://partner.microsoft.com/dashboard) van het Partnercentrum.</span><span class="sxs-lookup"><span data-stu-id="68921-136">Sign in to the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

2. <span data-ttu-id="68921-137">Selecteer **klanten** in het menu van het partner centrum en kies vervolgens een klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="68921-137">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

3. <span data-ttu-id="68921-138">Selecteer **gebruikers en licenties** in het menu klant.</span><span class="sxs-lookup"><span data-stu-id="68921-138">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="68921-139">Kies de gebruiker in de lijst.</span><span class="sxs-lookup"><span data-stu-id="68921-139">Choose the user from the list.</span></span>

4. <span data-ttu-id="68921-140">Selecteer onder aan het scherm **wacht woord opnieuw instellen**.</span><span class="sxs-lookup"><span data-stu-id="68921-140">At the bottom of the screen, select **Reset password**.</span></span> 

5. <span data-ttu-id="68921-141">Het nieuwe tijdelijke wacht woord naar de gebruiker verzenden.</span><span class="sxs-lookup"><span data-stu-id="68921-141">Send the new temporary password to the user.</span></span>

<a href="" id="deleteuseraccounts"></a>

## <a name="delete-user-accounts-for-a-customer"></a><span data-ttu-id="68921-142">Gebruikers accounts voor een klant verwijderen</span><span class="sxs-lookup"><span data-stu-id="68921-142">Delete user accounts for a customer</span></span>

1. <span data-ttu-id="68921-143">Selecteer in het menu **Partner Center** **klanten**.</span><span class="sxs-lookup"><span data-stu-id="68921-143">From the **Partner Center** menu, select **Customers**.</span></span> <span data-ttu-id="68921-144">Kies de klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="68921-144">Choose the customer from the list.</span></span>

2. <span data-ttu-id="68921-145">Selecteer **gebruikers en licenties** in het menu klant.</span><span class="sxs-lookup"><span data-stu-id="68921-145">In the customer menu, select **Users and licenses**.</span></span> <span data-ttu-id="68921-146">Kies de gebruiker in de lijst.</span><span class="sxs-lookup"><span data-stu-id="68921-146">Choose the user from the list.</span></span>

3. <span data-ttu-id="68921-147">Selecteer onder aan het scherm de optie **gebruikers account verwijderen**.</span><span class="sxs-lookup"><span data-stu-id="68921-147">At the bottom of the screen, select **Delete user account**.</span></span>

<span data-ttu-id="68921-148">Als u dit account wilt herstellen, kunt u het vinden op het tabblad **Verwijderde gebruikers** van de lijst **gebruikers en licenties** van de klant.</span><span class="sxs-lookup"><span data-stu-id="68921-148">If you need to restore this account, you can find it in the **Deleted users** tab of the Customer's **Users and licenses** list.</span></span> <span data-ttu-id="68921-149">U hebt 30 dagen de tijd om een verwijderde gebruiker te herstellen.</span><span class="sxs-lookup"><span data-stu-id="68921-149">You have 30 days to restore a deleted user.</span></span>

<a href="" id="restoreuseraccounts"></a>

## <a name="restore-deleted-user-accounts"></a><span data-ttu-id="68921-150">Verwijderde gebruikers accounts herstellen</span><span class="sxs-lookup"><span data-stu-id="68921-150">Restore deleted user accounts</span></span>

1. <span data-ttu-id="68921-151">Selecteer **klanten** in het menu van het **partner centrum** en kies vervolgens de klant in de lijst.</span><span class="sxs-lookup"><span data-stu-id="68921-151">From the **Partner Center** menu, select **Customers**, then choose the customer from the list.</span></span>

2. <span data-ttu-id="68921-152">Selecteer **gebruikers en licenties**.</span><span class="sxs-lookup"><span data-stu-id="68921-152">Select **Users and licenses**.</span></span>

3. <span data-ttu-id="68921-153">Selecteer het tabblad **Verwijderde gebruikers ()** . Het moet worden gelezen **(1)** of groter wanneer er verwijderde gebruikers zijn die kunnen worden hersteld.</span><span class="sxs-lookup"><span data-stu-id="68921-153">Select the **Deleted users ( )** tab. It should read **(1)** or greater when there are deleted users that can be restored.</span></span>

4. <span data-ttu-id="68921-154">Selecteer een of meer van de selectie vakjes van de verwijderde gebruikers en selecteer vervolgens **herstellen**.</span><span class="sxs-lookup"><span data-stu-id="68921-154">Select one or more of the deleted users' checkboxes and then select **Restore**.</span></span>

    <span data-ttu-id="68921-155">Alle geselecteerde gebruikers accounts worden weer gegeven op de pagina **gebruikers en licenties** .</span><span class="sxs-lookup"><span data-stu-id="68921-155">All selected user accounts will reappear in the **Users and licenses** page.</span></span>

## <a name="next-steps"></a><span data-ttu-id="68921-156">Volgende stappen</span><span class="sxs-lookup"><span data-stu-id="68921-156">Next steps</span></span>

- [<span data-ttu-id="68921-157">Licenties toewijzen of intrekken voor meerdere gebruikers</span><span class="sxs-lookup"><span data-stu-id="68921-157">Assign or revoke licenses to multiple users</span></span>](bulk-license-provisioning-for-multiple-users.md)

- [<span data-ttu-id="68921-158">Meerdere gebruikers voor een klant account maken</span><span class="sxs-lookup"><span data-stu-id="68921-158">Create multiple users for a customer account</span></span>](adding-multiple-users-to-a-customer-account.md)
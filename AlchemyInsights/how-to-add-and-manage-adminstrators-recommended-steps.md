---
title: Postup pridávania a spravovania Adminstrators – Odporúčané kroky
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678872"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="9bd02-102">Postup pridávania a spravovania Adminstrators – Odporúčané kroky</span><span class="sxs-lookup"><span data-stu-id="9bd02-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="9bd02-103">**Úprava správcu predplatného alebo spolusprávcu**</span><span class="sxs-lookup"><span data-stu-id="9bd02-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="9bd02-104">Správca konta môže upraviť obe roly, zatiaľ čo správca predplatného môže zmeniť iba správcov na [portáli Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="9bd02-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="9bd02-105">Pridanie alebo zmena správcov predplatného Azure</span><span class="sxs-lookup"><span data-stu-id="9bd02-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="9bd02-106">**Aktualizácia správcu predplatného alebo Co-Administrator pre interné (VYSIELAné) predplatné**</span><span class="sxs-lookup"><span data-stu-id="9bd02-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="9bd02-107">Správca služieb alebo spolusprávca môže túto akciu samostatne podávať pomocou týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="9bd02-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="9bd02-108">Prihláste sa na [portáli Azure](https://ms.portal.azure.com/#home) a kliknite na položku **Správa nákladov + Fakturácia** v ľavom kotúči.</span><span class="sxs-lookup"><span data-stu-id="9bd02-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="9bd02-109">Kliknite na položku riadok s predplatným.</span><span class="sxs-lookup"><span data-stu-id="9bd02-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="9bd02-110">Otvorí sa vám prehľad predplatného.</span><span class="sxs-lookup"><span data-stu-id="9bd02-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="9bd02-111">Na ostrie **predplatného** kliknite na položku **Vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="9bd02-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="9bd02-112">Kliknite na tlačidlo **Správca služby** .</span><span class="sxs-lookup"><span data-stu-id="9bd02-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="9bd02-113">Zadajte e-mailovú adresu používateľa, ktorého chcete nastaviť ako správcu služby, a kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="9bd02-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="9bd02-114">**Pridanie alebo zmena alebo odstránenie spolusprávcu**</span><span class="sxs-lookup"><span data-stu-id="9bd02-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="9bd02-115">Prihláste sa na [portáli Azure](https://ms.portal.azure.com/#home) ako správca služieb.</span><span class="sxs-lookup"><span data-stu-id="9bd02-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="9bd02-116">Otvorte [predplatné](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) a vyberte predplatné.</span><span class="sxs-lookup"><span data-stu-id="9bd02-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="9bd02-117">(Co-Adminstrators môže byť priradená iba v rozsahu predplatného.)</span><span class="sxs-lookup"><span data-stu-id="9bd02-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="9bd02-118">Prechod na **Ovládací prvok Access Control (IAM)**  >  **Classic správcovia**  >  **Pridať**  >  **Pridať spolusprávcu** na otvorenie tably **Pridať** spolusprávcu (ak je možnosť pridať spolusprávcu vypnutá, znamená to, že nemáte povolenia).</span><span class="sxs-lookup"><span data-stu-id="9bd02-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="9bd02-119">Vyberte používateľa, ktorého chcete pridať, a kliknite na položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="9bd02-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="9bd02-120">**zistiť viac:**</span><span class="sxs-lookup"><span data-stu-id="9bd02-120">**Learn more:**</span></span>
- [<span data-ttu-id="9bd02-121">Pridanie spolusprávcu</span><span class="sxs-lookup"><span data-stu-id="9bd02-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="9bd02-122">Odstránenie spolusprávcu</span><span class="sxs-lookup"><span data-stu-id="9bd02-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="9bd02-123">Zmena správcu služby</span><span class="sxs-lookup"><span data-stu-id="9bd02-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="9bd02-124">Zobrazenie správcu konta</span><span class="sxs-lookup"><span data-stu-id="9bd02-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="9bd02-125">Správa prístupu pomocou RBAC a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="9bd02-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="9bd02-126">**Pridanie alebo odstránenie používateľov pomocou služby Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="9bd02-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="9bd02-127">Môžete pridať nových používateľov alebo odstrániť existujúcich používateľov zo služby Azure Active Directory (Azure AD) organizácie:</span><span class="sxs-lookup"><span data-stu-id="9bd02-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="9bd02-128">Ak chcete pridať nového používateľa, prihláste sa na [portáli Azure](https://ms.portal.azure.com/#home) ako používateľ – správca organizácie.</span><span class="sxs-lookup"><span data-stu-id="9bd02-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="9bd02-129">Vyberte položku **Azure Active Directory**, vyberte položku **Používatelia** a potom kliknite na položku **Nový používateľ**.</span><span class="sxs-lookup"><span data-stu-id="9bd02-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="9bd02-130">Na stránke **používateľ** Vyplňte požadované informácie.</span><span class="sxs-lookup"><span data-stu-id="9bd02-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="9bd02-131">Kliknite na položku **vytvoriť**.</span><span class="sxs-lookup"><span data-stu-id="9bd02-131">Click **Create**.</span></span> <span data-ttu-id="9bd02-132">Používateľ sa vytvorí a pridá do nájomníka služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9bd02-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="9bd02-133">Ďalšie **informácie**:</span><span class="sxs-lookup"><span data-stu-id="9bd02-133">**Learn more**:</span></span>

- [<span data-ttu-id="9bd02-134">Pridanie nového používateľa</span><span class="sxs-lookup"><span data-stu-id="9bd02-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="9bd02-135">Odstránenie používateľa</span><span class="sxs-lookup"><span data-stu-id="9bd02-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="9bd02-136">Pridanie alebo aktualizácia informácií o profile používateľa pomocou služby Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9bd02-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="9bd02-137">**Odporúčané dokumenty**</span><span class="sxs-lookup"><span data-stu-id="9bd02-137">**Recommended documents**</span></span>

- [<span data-ttu-id="9bd02-138">Čo je riadenie prístupu na základe rolí (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="9bd02-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="9bd02-139">Porozumieť rôznym funkciám v službe Azure</span><span class="sxs-lookup"><span data-stu-id="9bd02-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="9bd02-140">Povolenia roly správcu v službe Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9bd02-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="9bd02-141">Kurz: udelenie prístupu používateľovi pomocou RBAC a portálu Azure</span><span class="sxs-lookup"><span data-stu-id="9bd02-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="9bd02-142">Riešenie problémov s RBAC v službe Azure</span><span class="sxs-lookup"><span data-stu-id="9bd02-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="9bd02-143">Usporiadanie zdrojov pomocou skupín spravovania služby Azure</span><span class="sxs-lookup"><span data-stu-id="9bd02-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="9bd02-144">Ako požiadať o kópiu Azure faktúry prostredníctvom e-mailu</span><span class="sxs-lookup"><span data-stu-id="9bd02-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="9bd02-145">Pridanie, aktualizácia alebo odstránenie kreditnej alebo debetnej karty zo služby Azure</span><span class="sxs-lookup"><span data-stu-id="9bd02-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="9bd02-146">Spravovanie (Opätovná aktivácia/zrušenie/zmena) predplatného</span><span class="sxs-lookup"><span data-stu-id="9bd02-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)




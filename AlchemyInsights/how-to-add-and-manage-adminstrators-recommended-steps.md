---
title: Postup pridávania a spravovania správcov – Odporúčané kroky
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
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755850"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="41f5e-102">Postup pridávania a spravovania správcov – Odporúčané kroky</span><span class="sxs-lookup"><span data-stu-id="41f5e-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="41f5e-103">Na základe popisu problému sme našli riešenie.</span><span class="sxs-lookup"><span data-stu-id="41f5e-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="41f5e-104">Väčšina zákazníkov si po vykonaní našej dokumentácie dokázala vyriešiť svoj problém sami.</span><span class="sxs-lookup"><span data-stu-id="41f5e-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="41f5e-105">**Úprava správcu predplatného alebo spolusprávcu**</span><span class="sxs-lookup"><span data-stu-id="41f5e-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="41f5e-106">Správca konta môže upraviť obe roly, zatiaľ čo správca predplatného môže zmeniť iba správcov na [portáli Azure](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="41f5e-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="41f5e-107">Pridanie alebo zmena správcov predplatného Azure</span><span class="sxs-lookup"><span data-stu-id="41f5e-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="41f5e-108">**Aktualizácia správcu predplatného alebo Co-Administrator pre interné (VYSIELAné) predplatné**</span><span class="sxs-lookup"><span data-stu-id="41f5e-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="41f5e-109">Správca služieb alebo spolusprávca môže túto akciu samostatne podávať pomocou týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="41f5e-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="41f5e-110">Prihláste sa na [portáli Azure](https://ms.portal.azure.com/#home) a kliknite na položku **Správa nákladov + Fakturácia** v ľavom kotúči.</span><span class="sxs-lookup"><span data-stu-id="41f5e-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="41f5e-111">Kliknite na položku riadok s predplatným.</span><span class="sxs-lookup"><span data-stu-id="41f5e-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="41f5e-112">Otvorí sa vám prehľad predplatného.</span><span class="sxs-lookup"><span data-stu-id="41f5e-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="41f5e-113">Na ostrie **predplatného** kliknite na položku **Vlastnosti**.</span><span class="sxs-lookup"><span data-stu-id="41f5e-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="41f5e-114">Kliknite na tlačidlo **Správca služby** .</span><span class="sxs-lookup"><span data-stu-id="41f5e-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="41f5e-115">Zadajte e-mailovú adresu používateľa, ktorého chcete nastaviť ako správcu služby, a kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="41f5e-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="41f5e-116">**Pridanie alebo zmena alebo odstránenie spolusprávcu**</span><span class="sxs-lookup"><span data-stu-id="41f5e-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="41f5e-117">Prihláste sa na [portáli Azure](https://ms.portal.azure.com/#home) ako správca služieb.</span><span class="sxs-lookup"><span data-stu-id="41f5e-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="41f5e-118">Otvorte [predplatné](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) a vyberte predplatné.</span><span class="sxs-lookup"><span data-stu-id="41f5e-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="41f5e-119">(Co-Adminstrators môže byť priradená iba v rozsahu predplatného.)</span><span class="sxs-lookup"><span data-stu-id="41f5e-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="41f5e-120">Prechod na **Ovládací prvok Access Control (IAM)**  >  **Classic správcovia**  >  **Pridať**  >  **Pridať spolusprávcu** na otvorenie tably **Pridať** spolusprávcu (ak je možnosť pridať spolusprávcu vypnutá, znamená to, že nemáte povolenia).</span><span class="sxs-lookup"><span data-stu-id="41f5e-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="41f5e-121">Vyberte používateľa, ktorého chcete pridať, a kliknite na položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="41f5e-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="41f5e-122">**zistiť viac:**</span><span class="sxs-lookup"><span data-stu-id="41f5e-122">**Learn more:**</span></span>
- [<span data-ttu-id="41f5e-123">Pridanie spolusprávcu</span><span class="sxs-lookup"><span data-stu-id="41f5e-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="41f5e-124">Odstránenie spolusprávcu</span><span class="sxs-lookup"><span data-stu-id="41f5e-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="41f5e-125">Zmena správcu služby</span><span class="sxs-lookup"><span data-stu-id="41f5e-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="41f5e-126">Zobrazenie správcu konta</span><span class="sxs-lookup"><span data-stu-id="41f5e-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="41f5e-127">Správa prístupu pomocou RBAC a Azure Portal</span><span class="sxs-lookup"><span data-stu-id="41f5e-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="41f5e-128">**Pridanie alebo odstránenie používateľov pomocou služby Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="41f5e-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="41f5e-129">Môžete pridať nových používateľov alebo odstrániť existujúcich používateľov zo služby Azure Active Directory (Azure AD) organizácie:</span><span class="sxs-lookup"><span data-stu-id="41f5e-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="41f5e-130">Ak chcete pridať nového používateľa, prihláste sa na [portáli Azure](https://ms.portal.azure.com/#home) ako používateľ – správca organizácie.</span><span class="sxs-lookup"><span data-stu-id="41f5e-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="41f5e-131">Vyberte položku **Azure Active Directory**, vyberte položku **Používatelia** a potom kliknite na položku **Nový používateľ**.</span><span class="sxs-lookup"><span data-stu-id="41f5e-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="41f5e-132">Na stránke **používateľ** Vyplňte požadované informácie.</span><span class="sxs-lookup"><span data-stu-id="41f5e-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="41f5e-133">Kliknite na položku **vytvoriť**.</span><span class="sxs-lookup"><span data-stu-id="41f5e-133">Click **Create**.</span></span> <span data-ttu-id="41f5e-134">Používateľ sa vytvorí a pridá do nájomníka služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="41f5e-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="41f5e-135">Ďalšie **informácie**:</span><span class="sxs-lookup"><span data-stu-id="41f5e-135">**Learn more**:</span></span>

- [<span data-ttu-id="41f5e-136">Pridanie nového používateľa</span><span class="sxs-lookup"><span data-stu-id="41f5e-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="41f5e-137">Odstránenie používateľa</span><span class="sxs-lookup"><span data-stu-id="41f5e-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="41f5e-138">Pridanie alebo aktualizácia informácií o profile používateľa pomocou služby Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="41f5e-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="41f5e-139">**Odporúčané dokumenty**</span><span class="sxs-lookup"><span data-stu-id="41f5e-139">**Recommended documents**</span></span>

- [<span data-ttu-id="41f5e-140">Čo je riadenie prístupu na základe rolí (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="41f5e-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="41f5e-141">Porozumieť rôznym funkciám v službe Azure</span><span class="sxs-lookup"><span data-stu-id="41f5e-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="41f5e-142">Povolenia roly správcu v službe Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="41f5e-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="41f5e-143">Kurz: udelenie prístupu používateľovi pomocou RBAC a portálu Azure</span><span class="sxs-lookup"><span data-stu-id="41f5e-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="41f5e-144">Riešenie problémov s RBAC v službe Azure</span><span class="sxs-lookup"><span data-stu-id="41f5e-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="41f5e-145">Usporiadanie zdrojov pomocou skupín spravovania služby Azure</span><span class="sxs-lookup"><span data-stu-id="41f5e-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="41f5e-146">Ako požiadať o kópiu Azure faktúry prostredníctvom e-mailu</span><span class="sxs-lookup"><span data-stu-id="41f5e-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="41f5e-147">Pridanie, aktualizácia alebo odstránenie kreditnej alebo debetnej karty zo služby Azure</span><span class="sxs-lookup"><span data-stu-id="41f5e-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="41f5e-148">Spravovanie (Opätovná aktivácia/zrušenie/zmena) predplatného</span><span class="sxs-lookup"><span data-stu-id="41f5e-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)




---
title: Problémy s používaním správcovskej konzoly Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555877"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="d782d-102">Problémy s používaním správcovskej konzoly Intune</span><span class="sxs-lookup"><span data-stu-id="d782d-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="d782d-103">**"Prístup odmietnutý" pri navigácii portálu na správu Intune.**</span><span class="sxs-lookup"><span data-stu-id="d782d-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="d782d-104">Ak ste členom vlastnej roly Intune, uistite sa, že licenciu Intune alebo Enterprise Mobility Suite (EMS) je priradená k vášmu účtu.</span><span class="sxs-lookup"><span data-stu-id="d782d-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="d782d-105">Ak používate Configuration Manager spravovať zariadenia, skontrolujte, či nie ste súčasťou kolekcie používateľov Intune Configuration Manager MDM.</span><span class="sxs-lookup"><span data-stu-id="d782d-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="d782d-106">Overte, či vám boli priradené príslušné povolenia na správu na základe rolí (RBAC) v blade rolí Intune.</span><span class="sxs-lookup"><span data-stu-id="d782d-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="d782d-107">Overte, či použitá skupina nie je distribučný zoznam.</span><span class="sxs-lookup"><span data-stu-id="d782d-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="d782d-108">Intune na portáli Azure podporuje iba používateľské kontá, ktoré patria do skupín zabezpečenia Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="d782d-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="d782d-109">Skontrolujte skupiny na portáli Azure > **Skupiny Intune**  >  **Groups**alebo na portáli Azure > Azure **Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="d782d-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="d782d-110">**Používateľ má príliš veľa povolení pre priradenú rolu Intune**</span><span class="sxs-lookup"><span data-stu-id="d782d-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="d782d-111">Učte používateľa, aby **prejsť na Intune**  >  **Intune**  >  **roly Moje povolenia**  >  **Export** na kontrolu udelených povolení.</span><span class="sxs-lookup"><span data-stu-id="d782d-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="d782d-112">**Skupina rozsahu bola pridaná do roly, ale používatelia v tejto roli stále vidia iných používateľov alebo zariadenia.**</span><span class="sxs-lookup"><span data-stu-id="d782d-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="d782d-113">Skupiny rozsahov nefiltruje používateľov alebo zariadenia.</span><span class="sxs-lookup"><span data-stu-id="d782d-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="d782d-114">Skupiny rozsahu:</span><span class="sxs-lookup"><span data-stu-id="d782d-114">Scope groups:</span></span>

- <span data-ttu-id="d782d-115">Obmedzte používateľov, komu môžu priraďovať politiky alebo aplikácie.</span><span class="sxs-lookup"><span data-stu-id="d782d-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="d782d-116">Povoliť spustenie vzdialených úloh v zariadeniach iba konkrétnym používateľom.</span><span class="sxs-lookup"><span data-stu-id="d782d-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="d782d-117">Ďalšie informácie o skupinách rozsahov nájdete v téme [Riadenie prístupu založené na rolách (RBAC) s programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="d782d-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="d782d-118">**Pridal som užívateľa do úlohy Intune, ale stále majú plný prístup k Admin Console Intune.**</span><span class="sxs-lookup"><span data-stu-id="d782d-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="d782d-119">Prejdite na Intune > **používateľov** na portáli Azure a overte, či používateľ nie je priradený žiadne z nasledujúcich rolí na portáli Azure:</span><span class="sxs-lookup"><span data-stu-id="d782d-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="d782d-120">Globálny správca</span><span class="sxs-lookup"><span data-stu-id="d782d-120">Global administrator</span></span>
- <span data-ttu-id="d782d-121">Správca služby Intune</span><span class="sxs-lookup"><span data-stu-id="d782d-121">Intune service administrator</span></span>
- <span data-ttu-id="d782d-122">Správca služby SharePoint</span><span class="sxs-lookup"><span data-stu-id="d782d-122">SharePoint administrator</span></span>

<span data-ttu-id="d782d-123">Ďalšie informácie nájdete v téme [Riadenie prístupu založené na rolách (RBAC) s microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="d782d-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="d782d-124">**Problémy s prístupom**</span><span class="sxs-lookup"><span data-stu-id="d782d-124">**Access Issues**</span></span>

<span data-ttu-id="d782d-125">Ďalšie informácie nájdete v téme [Nemôžete sa prihlásiť do služieb Office 365, Azure alebo Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="d782d-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>
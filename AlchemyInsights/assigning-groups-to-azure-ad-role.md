---
title: Priradenie skupín k úlohe Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885397"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="f09d2-102">Priradenie skupín k úlohe Azure AD</span><span class="sxs-lookup"><span data-stu-id="f09d2-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="f09d2-103">Ak chcete priradiť skupinu Azure AD so zdrojom autority v službe Azure AD na rolu Azure AD, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="f09d2-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="f09d2-104">Vytvorenie novej skupiny – vytvorenie novej skupiny:</span><span class="sxs-lookup"><span data-stu-id="f09d2-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="f09d2-105">a.</span><span class="sxs-lookup"><span data-stu-id="f09d2-105">a.</span></span> <span data-ttu-id="f09d2-106">Prihláste sa do centra spravovania služby Azure AD s **privilegovaným správcom roly** alebo povoleniami **globálneho správcu** .</span><span class="sxs-lookup"><span data-stu-id="f09d2-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="f09d2-107">b.</span><span class="sxs-lookup"><span data-stu-id="f09d2-107">b.</span></span> <span data-ttu-id="f09d2-108">Vyberte položku **Azure Active Directory > skupiny > všetky skupiny > novú skupinu**.</span><span class="sxs-lookup"><span data-stu-id="f09d2-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="f09d2-109">c.</span><span class="sxs-lookup"><span data-stu-id="f09d2-109">c.</span></span> <span data-ttu-id="f09d2-110">Vytvorte skupinu.</span><span class="sxs-lookup"><span data-stu-id="f09d2-110">Create the group.</span></span>

2. <span data-ttu-id="f09d2-111">Priraďte rolu skupine buď počas vytvárania skupiny alebo po vytvorení skupiny.</span><span class="sxs-lookup"><span data-stu-id="f09d2-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="f09d2-112">a.</span><span class="sxs-lookup"><span data-stu-id="f09d2-112">a.</span></span> <span data-ttu-id="f09d2-113">Ak chcete skupine priradiť rolu v čase vytvárania skupiny, zapnite funkciu prepnutia **funkcií Azure AD môže byť priradená skupine** a vytvorte skupinu.</span><span class="sxs-lookup"><span data-stu-id="f09d2-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="f09d2-114">b.</span><span class="sxs-lookup"><span data-stu-id="f09d2-114">b.</span></span> <span data-ttu-id="f09d2-115">Ak chcete priradiť rolu k skupine po jej vytvorení, prejdite na kartu **priradené roly** pre novo vytvorenú skupinu a priraďte rolu skupine.</span><span class="sxs-lookup"><span data-stu-id="f09d2-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="f09d2-116">**Spravovanie členstva v skupine, ktorá je priradená k úlohe Azure AD**</span><span class="sxs-lookup"><span data-stu-id="f09d2-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="f09d2-117">Ak chcete zabrániť zvýšeniu počtu privilégií, na základe predvoleného nastavenia môžu členovia skupiny, ktorá je priradená k úlohe, upravovať iba privilegovaní správcovia rolí a globálni správcovia.</span><span class="sxs-lookup"><span data-stu-id="f09d2-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="f09d2-118">Môže sa však rozhodnúť priradiť vlastníkovi takejto skupiny a delegovať túto úlohu.</span><span class="sxs-lookup"><span data-stu-id="f09d2-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="f09d2-119">Ďalšie informácie o priraďovaní cloudových skupín k funkciám Azure AD nájdete v téme [Priradenie ROLÍ reklamy skupine cloud](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="f09d2-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="f09d2-120">Ďalšie informácie o riešení problémov s rolami priradenými k cloudovým skupinám nájdete v téme [Riešenie problémov priradených k cloudovým skupinám](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="f09d2-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>






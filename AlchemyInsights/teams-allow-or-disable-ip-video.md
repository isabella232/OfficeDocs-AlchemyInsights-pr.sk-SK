---
title: Povolenie alebo zakázanie IP videa v aplikácii teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670199"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="e9d07-102">Povolenie alebo zakázanie IP videa v aplikácii teams</span><span class="sxs-lookup"><span data-stu-id="e9d07-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="e9d07-103">**Zmena alebo vytvorenie politiky schôdze**</span><span class="sxs-lookup"><span data-stu-id="e9d07-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="e9d07-104">Ak chcete zmeniť alebo vytvoriť politiku schôdze, prejdite na **lokalitu centrum spravovania služieb Microsoft teams > schôdze > politiky schôdzí**.</span><span class="sxs-lookup"><span data-stu-id="e9d07-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="e9d07-105">Vyberte politiku v zozname alebo kliknite na položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="e9d07-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="e9d07-106">Ak vytvárate novú politiku, pridajte názov a popis.</span><span class="sxs-lookup"><span data-stu-id="e9d07-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="e9d07-107">Názov nesmie obsahovať špeciálne znaky a môže mať najviac 64 znakov.</span><span class="sxs-lookup"><span data-stu-id="e9d07-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="e9d07-108">Vyberte požadované nastavenia a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="e9d07-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="e9d07-109">Povedzme napríklad, že máte veľa používateľov a chcete obmedziť veľkosť šírky pásma, ktorú by vyžadovala ich schôdza.</span><span class="sxs-lookup"><span data-stu-id="e9d07-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="e9d07-110">Vytvorili by ste novú vlastnú politiku s názvom Obmedzená šírka pásma a vypnete nasledujúce nastavenia:</span><span class="sxs-lookup"><span data-stu-id="e9d07-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="e9d07-111">V časti **Zvuk a video**:</span><span class="sxs-lookup"><span data-stu-id="e9d07-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="e9d07-112">Vypnite nastavenie Umožniť nahrávanie cez cloud.</span><span class="sxs-lookup"><span data-stu-id="e9d07-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="e9d07-113">Vypnite nastavenie Povoliť IP video.</span><span class="sxs-lookup"><span data-stu-id="e9d07-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="e9d07-114">Potom priraďte politiku používateľom.</span><span class="sxs-lookup"><span data-stu-id="e9d07-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="e9d07-115">**Priradenie politiky pre schôdze používateľom**</span><span class="sxs-lookup"><span data-stu-id="e9d07-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="e9d07-116">V ľavej navigácii centra spravovania pre Microsoft Teams prejdite na položku **Používatelia** a potom kliknite na používateľa.</span><span class="sxs-lookup"><span data-stu-id="e9d07-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="e9d07-117">Vyberte používateľa kliknutím naľavo od mena používateľa a potom kliknite na položku **Upraviť nastavenia**.</span><span class="sxs-lookup"><span data-stu-id="e9d07-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="e9d07-118">V časti **politika schôdze**vyberte politiku, ktorú chcete priradiť, a potom kliknite na položku **použiť**.</span><span class="sxs-lookup"><span data-stu-id="e9d07-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="e9d07-119">Ďalšie informácie nájdete v téme [Správa politík schôdze v aplikácii teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="e9d07-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

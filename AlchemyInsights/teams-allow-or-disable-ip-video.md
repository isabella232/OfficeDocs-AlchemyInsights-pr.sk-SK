---
title: Povolenie alebo zakázanie IP videa v Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826358"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="dc60c-102">Povolenie alebo zakázanie IP videa v Teams</span><span class="sxs-lookup"><span data-stu-id="dc60c-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="dc60c-103">**Zmena alebo vytvorenie politiky schôdze**</span><span class="sxs-lookup"><span data-stu-id="dc60c-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="dc60c-104">Ak chcete zmeniť alebo vytvoriť politiku schôdze, prejdite do Centra spravovania služby **Microsoft Teams a > schôdze > schôdze.**</span><span class="sxs-lookup"><span data-stu-id="dc60c-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="dc60c-105">Vyberte politiku v zozname alebo kliknite na položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="dc60c-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="dc60c-106">Ak vytvárate novú politiku, pridajte názov a popis.</span><span class="sxs-lookup"><span data-stu-id="dc60c-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="dc60c-107">Názov nesmie obsahovať špeciálne znaky a môže mať najviac 64 znakov.</span><span class="sxs-lookup"><span data-stu-id="dc60c-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="dc60c-108">Vyberte požadované nastavenia a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="dc60c-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="dc60c-109">Povedzme, že máte veľa používateľov a chcete obmedziť šírku pásma, ktoré by ich schôdza vyžadovala.</span><span class="sxs-lookup"><span data-stu-id="dc60c-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="dc60c-110">Vytvorili by ste novú vlastnú politiku s názvom Obmedzená šírka pásma a vypnete nasledujúce nastavenia:</span><span class="sxs-lookup"><span data-stu-id="dc60c-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="dc60c-111">V časti **Zvuk a video**:</span><span class="sxs-lookup"><span data-stu-id="dc60c-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="dc60c-112">Vypnite nastavenie Umožniť nahrávanie cez cloud.</span><span class="sxs-lookup"><span data-stu-id="dc60c-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="dc60c-113">Vypnite nastavenie Povoliť IP video.</span><span class="sxs-lookup"><span data-stu-id="dc60c-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="dc60c-114">Potom priraďte politiku používateľom.</span><span class="sxs-lookup"><span data-stu-id="dc60c-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="dc60c-115">**Priradenie politiky pre schôdze používateľom**</span><span class="sxs-lookup"><span data-stu-id="dc60c-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="dc60c-116">V ľavej navigácii centra spravovania pre Microsoft Teams prejdite na položku **Používatelia** a potom kliknite na používateľa.</span><span class="sxs-lookup"><span data-stu-id="dc60c-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="dc60c-117">Vyberte používateľa kliknutím naľavo od mena používateľa a potom kliknite na položku **Upraviť nastavenia**.</span><span class="sxs-lookup"><span data-stu-id="dc60c-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="dc60c-118">V **časti Politika schôdze** vyberte politiku, ktorú chcete priradiť, a potom kliknite na položku **Použiť**.</span><span class="sxs-lookup"><span data-stu-id="dc60c-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="dc60c-119">Ďalšie informácie nájdete v téme [Spravovanie politík schôdzí v Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="dc60c-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

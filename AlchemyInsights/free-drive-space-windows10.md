---
title: Uvoľnenie miesta na disku vo Windowse 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037948"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="65328-102">Uvoľnenie miesta na disku vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="65328-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="65328-103">Tu sú dve možnosti, ako uvoľniť miesto na disku vo Windowse:</span><span class="sxs-lookup"><span data-stu-id="65328-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="65328-104">Uvoľnite miesto na disku vo Windowse 10.</span><span class="sxs-lookup"><span data-stu-id="65328-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="65328-105">Uvoľnite miesto pre aktualizácie pre Windows 10 s externým ukladacím zariadením.</span><span class="sxs-lookup"><span data-stu-id="65328-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="65328-106">Ak máte stále dostatok voľného miesta na disku po použití čistenia disku, je možné, že priečinok Temp sa rýchlo vyplní súbormi Application (. Appx), ktoré používa Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="65328-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="65328-107">Ak chcete tento problém vyriešiť, obnovte ukladanie, vymažte vyrovnávaciu pamäť obchodu a potom spustite Poradcu pri riešení problémov so službou Windows Update.</span><span class="sxs-lookup"><span data-stu-id="65328-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="65328-108">Pred pokračovaním v týchto krokoch Skontrolujte, či je Microsoft Obchod zavretý.</span><span class="sxs-lookup"><span data-stu-id="65328-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="65328-109">**Krok 1: Vynulovanie Microsoft obchodu**</span><span class="sxs-lookup"><span data-stu-id="65328-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="65328-110">**Poznámka:** Týmto sa natrvalo odstránia údaje aplikácie v zariadení vrátane predvolieb a podrobností o prihlasovaní.</span><span class="sxs-lookup"><span data-stu-id="65328-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="65328-111">Vyberte položku **Start**  >  **Settings** Apps Apps  >    >  **& funkcií**.</span><span class="sxs-lookup"><span data-stu-id="65328-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="65328-112">V zozname aplikácií vyhľadajte a vyberte položku Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="65328-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="65328-113">Vyberte položku **Rozšírené možnosti**.</span><span class="sxs-lookup"><span data-stu-id="65328-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="65328-114">Posuňte sa nadol a vyberte položku **obnoviť** a potom **potvrďte vynulovanie**.</span><span class="sxs-lookup"><span data-stu-id="65328-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="65328-115">**Krok 2: Vymazanie vyrovnávacej pamäte Microsoft obchodu**</span><span class="sxs-lookup"><span data-stu-id="65328-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="65328-116">Stlačením klávesu s logom Windows + R otvorte dialógové okno spustiť.</span><span class="sxs-lookup"><span data-stu-id="65328-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="65328-117">Zadajte wsreset.exe a kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="65328-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="65328-118">Otvorí sa prázdne okno príkazového riadka.</span><span class="sxs-lookup"><span data-stu-id="65328-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="65328-119">Po približne 10 sekundách sa okno zavrie a ukladací priestor sa otvorí automaticky.</span><span class="sxs-lookup"><span data-stu-id="65328-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="65328-120">**Krok 3: Vynulovanie aktualizácie Windowsu**</span><span class="sxs-lookup"><span data-stu-id="65328-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="65328-121">Vyberte položku **Spustiť**  >  aktualizáciu **nastavení**  >  & riešenie problémov so **zabezpečením**  >  .</span><span class="sxs-lookup"><span data-stu-id="65328-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="65328-122">Posuňte sa nadol a zo zoznamu vyberte položku **Windows Update** a vyberte položku **spustiť Poradcu pri riešení problémov**.</span><span class="sxs-lookup"><span data-stu-id="65328-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="65328-123">Reštartujte počítač a skontrolujte, či sa problém vyskytuje aj naďalej.</span><span class="sxs-lookup"><span data-stu-id="65328-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>


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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505371"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="d8e8d-102">Uvoľnenie miesta na disku vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="d8e8d-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="d8e8d-103">Existujú dve možnosti, ako vo Windowse uvoľniť miesto na disku:</span><span class="sxs-lookup"><span data-stu-id="d8e8d-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="d8e8d-104">Uvoľnite miesto na disku vo Windowse 10.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="d8e8d-105">Uvoľnite miesto pre aktualizácie Windowsu 10 v externom ukladacom zariadení.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="d8e8d-106">Ak máte po použití nástroja Čistenie disku stále málo miesta na disku, je možné, že sa priečinok Temp rýchlo zapĺňa súbormi aplikácií (.appx), ktoré používa Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="d8e8d-107">Na odstránenie tohto problému resetujte Microsoft Store, vymažte vyrovnávaciu pamäť Microsoft Storeu a spustite nástroj na riešenie problémov pre Windows Update.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="d8e8d-108">Skôr než budete pokračovať podľa týchto krokov, skontrolujte, či je Microsoft Store zatvorený.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="d8e8d-109">**1. krok: Resetovanie Microsoft Storeu**</span><span class="sxs-lookup"><span data-stu-id="d8e8d-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="d8e8d-110">**Poznámka** Týmto sa natrvalo odstránia údaje aplikácie v zariadení vrátane vašich predvolieb a podrobností o prihlásení.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="d8e8d-111">Vyberte možnosti **Štart** > **Nastavenia** > **Aplikácie** > **Aplikácie a funkcie**.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="d8e8d-112">V zozname aplikácií vyhľadajte a vyberte položku Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="d8e8d-113">Vyberte položku **Rozšírené možnosti**.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="d8e8d-114">Posuňte sa nadol a vyberte možnosť **Resetovať** a potom **Potvrdiť resetovanie**.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="d8e8d-115">**2. krok: Vymazanie vyrovnávacej pamäte Microsoft Storeu**</span><span class="sxs-lookup"><span data-stu-id="d8e8d-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="d8e8d-116">Stlačte kláves s logom Windows + R a otvorte dialógové okno Spustenie.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="d8e8d-117">Napíšte wsreset.exe a vyberte **OK**.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="d8e8d-118">Otvorí sa prázdne okno príkazového riadka.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="d8e8d-119">Približne po 10 sekundách sa okno zavrie a Microsoft Store sa automaticky otvorí.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="d8e8d-120">**3. krok: Resetovanie lokality Windows Update**</span><span class="sxs-lookup"><span data-stu-id="d8e8d-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="d8e8d-121">Vyberte možnosti **Štart** > **Nastavenia** > **Aktualizácia a zabezpečenie** > **Riešenie problémov**.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="d8e8d-122">Posuňte sa nadol a vyberte zo zoznamu položku **Windows Update** a potom možnosť **Spustiť riešenie problémov**.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="d8e8d-123">Reštartujte počítač a skontrolujte, či problém stále pretrváva.</span><span class="sxs-lookup"><span data-stu-id="d8e8d-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>


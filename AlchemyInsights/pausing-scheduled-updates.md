---
title: Pozastavenie plánovaných aktualizácií
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 9dc0f387cf63557e2a1f81ca8f3c3ca9998170ca
ms.sourcegitcommit: d1c51266e2890f61662f77dceea2ad0c88210015
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/30/2020
ms.locfileid: "46555989"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="62c62-102">Pozastavenie plánovaných aktualizácií</span><span class="sxs-lookup"><span data-stu-id="62c62-102">Pausing scheduled updates</span></span>

<span data-ttu-id="62c62-103">Po vydaní príkazu na pozastavenie zariadenia spracuje príkaz až po ďalšom odhlásení do intune.</span><span class="sxs-lookup"><span data-stu-id="62c62-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="62c62-104">Z tohto dôvodu môžu mať vaše zariadenia:</span><span class="sxs-lookup"><span data-stu-id="62c62-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="62c62-105">Pred registráciou sa nainštalovali plánované aktualizácie.</span><span class="sxs-lookup"><span data-stu-id="62c62-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="62c62-106">Bol vypnutý, keď ste vydali príkaz pauzy.</span><span class="sxs-lookup"><span data-stu-id="62c62-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="62c62-107">V tomto prípade, keď boli zariadenia zapnuté, mohli pred registráciou prevziať a nainštalovať plánované aktualizácie.</span><span class="sxs-lookup"><span data-stu-id="62c62-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>
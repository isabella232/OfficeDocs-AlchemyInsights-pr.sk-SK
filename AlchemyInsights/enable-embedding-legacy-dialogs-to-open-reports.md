---
title: Povolenie vkladania starších dialógových okna na otváranie zostáv
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814279"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="d853d-102">Povolenie vkladania starších dialógových okna na otváranie zostáv</span><span class="sxs-lookup"><span data-stu-id="d853d-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="d853d-103">**Príznak**</span><span class="sxs-lookup"><span data-stu-id="d853d-103">**Symptom**</span></span>

<span data-ttu-id="d853d-104">Používatelia nemôžu otvárať zostavy.</span><span class="sxs-lookup"><span data-stu-id="d853d-104">Users are unable to open reports.</span></span> <span data-ttu-id="d853d-105">Niečo sa pokazilo.</span><span class="sxs-lookup"><span data-stu-id="d853d-105">"Something has gone wrong.</span></span> <span data-ttu-id="d853d-106">Check technical details for more details".</span><span class="sxs-lookup"><span data-stu-id="d853d-106">Check technical details for more details."</span></span>

<span data-ttu-id="d853d-107">**Príčina**</span><span class="sxs-lookup"><span data-stu-id="d853d-107">**Cause**</span></span>

<span data-ttu-id="d853d-108">Zostavy zlyhávajú pri načítaní v UCI s chybou " Popisovač formulára je null alebo nie je definovaný."</span><span class="sxs-lookup"><span data-stu-id="d853d-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="d853d-109">Zostavy v UCI stále vyžadujú staršie dialógové okná, takže systém zákazníka musí mať povolené povolenie *delegovaniadialogsembe u zákazníkov.*</span><span class="sxs-lookup"><span data-stu-id="d853d-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="d853d-110">**Riešenie**</span><span class="sxs-lookup"><span data-stu-id="d853d-110">**Solution**</span></span>

1. <span data-ttu-id="d853d-111">Prejdite na **položky >Správa > kartu Nastavenie > Všeobecné**.</span><span class="sxs-lookup"><span data-stu-id="d853d-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="d853d-112">Nastavte položku Povoliť vkladanie niektorých starších dialógových oknách v klientovi prehliadača so zjednotením rozhrania na možnosť **Áno.**</span><span class="sxs-lookup"><span data-stu-id="d853d-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>

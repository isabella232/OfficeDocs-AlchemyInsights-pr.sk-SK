---
title: Prevod poštovej schránky používateľa do zdieľanej poštovej schránky?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374338"
---
<span data-ttu-id="1c8c9-102">Poštovú schránku môžete preniesť len k zdieľanej schránke Ak používateľ nemá licenciu Exchange.</span><span class="sxs-lookup"><span data-stu-id="1c8c9-102">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="1c8c9-103">Po skonvertovaní poštovej schránky sa bude naďalej zobrazovať v zozname aktívnych užívateľov, pretože tento zoznam obsahuje zdieľané poštové schránky.</span><span class="sxs-lookup"><span data-stu-id="1c8c9-103">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="1c8c9-104">Však prevedený poštovej schránky sa tiež zobrazí v zozname zdieľanej poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="1c8c9-104">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="1c8c9-105">Ak sa pokúsite previesť poštovej schránky Exchange Admin konzoly a prevod zlyhá, vymažte vyrovnávaciu pamäť prehliadača a súbory cookie a skúste znova.</span><span class="sxs-lookup"><span data-stu-id="1c8c9-105">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="1c8c9-106">Ak to stále nefunguje, skúste prevod poštovej schránky v prostredí Exchange Management Shell spustením nasledujúceho príkazu:</span><span class="sxs-lookup"><span data-stu-id="1c8c9-106">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="1c8c9-107">Viac konverzií informácie poštovej schránky je k dispozícii v [prevod používateľa poštovej schránky zdieľanej poštovej schránke](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span><span class="sxs-lookup"><span data-stu-id="1c8c9-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  

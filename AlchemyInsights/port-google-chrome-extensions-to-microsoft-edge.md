---
title: Prenos rozšírenia Google Chrome do prehliadača Microsoft Edge (chróm)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678982"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="963a0-102">Prenos rozšírenia Google Chrome do prehliadača Microsoft Edge (chróm)</span><span class="sxs-lookup"><span data-stu-id="963a0-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="963a0-103">[Rozšírenie prehliadača Google Chrome na Microsoft Edge (chróm)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)je jednoduché.</span><span class="sxs-lookup"><span data-stu-id="963a0-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="963a0-104">Vo väčšine prípadov je na spustenie týchto rozšírení v prehliadači Microsoft Edge potrebná len minimálna zmena.</span><span class="sxs-lookup"><span data-stu-id="963a0-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="963a0-105">Rozšírenia API a zjavne kľúče podporované prehliadačom Google Chrome sú kompatibilné s kódom Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="963a0-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="963a0-106">Microsoft Edge však nepodporuje rozšírenie rozhrania API Chrome. GCM, Chrome. identity. getAccounts, Chrome. identity. getAuthToken a Chrome. instanceID.</span><span class="sxs-lookup"><span data-stu-id="963a0-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>
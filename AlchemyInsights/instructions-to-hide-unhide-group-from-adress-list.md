---
title: Pokyny na skrytie/odkrytie skupiny zo zoznamu adries
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580024"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="62d59-102">Skryť skupinu Microsoft 365 zo zoznamu adries (GZA)</span><span class="sxs-lookup"><span data-stu-id="62d59-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="62d59-103">Skryť skupinu Microsoft 365 zo zoznamov adries (GZA) klientov exchange (napríklad Outlook alebo OWA), použite nasledujúci príkaz v prostredí EXO:</span><span class="sxs-lookup"><span data-stu-id="62d59-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="62d59-104">Ak chcete skryť skupinu Microsoft 365 viditeľné pre klientov servera Exchange, použite nasledujúci príkaz v prostredí EXO:</span><span class="sxs-lookup"><span data-stu-id="62d59-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


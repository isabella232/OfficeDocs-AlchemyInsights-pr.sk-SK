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
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908359"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skryť Microsoft 365 skupina zo zoznamu adries (GAL)

Ak chcete skryť skupinu Microsoft 365 zo zoznamov adries (GAL) klientov Exchange (napríklad Outlook alebo OWA), použite nasledujúci príkaz v EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Skryť Microsoft 365 skupiny z byť viditeľné na výmenu klientov, použite nasledujúci príkaz v EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


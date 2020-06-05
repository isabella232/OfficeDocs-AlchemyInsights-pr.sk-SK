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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skryť skupinu Microsoft 365 zo zoznamu adries (GZA)

Skryť skupinu Microsoft 365 zo zoznamov adries (GZA) klientov exchange (napríklad Outlook alebo OWA), použite nasledujúci príkaz v prostredí EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Ak chcete skryť skupinu Microsoft 365 viditeľné pre klientov servera Exchange, použite nasledujúci príkaz v prostredí EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


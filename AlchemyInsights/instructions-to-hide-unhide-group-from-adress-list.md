---
title: Pokyny na skrytie alebo odkrytie skupiny v zozname adries
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663024"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skrytie skupiny Microsoft 365 v zozname adries (GAL)

Ak chcete skryť skupinu Microsoft 365 zo zoznamov adries (GAL) klientov Exchange (ako je napríklad Outlook alebo OWA), použite nasledujúci príkaz v prostredí EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Ak chcete skryť skupinu Microsoft 365, ktorá je viditeľná pre klientov Exchange, použite nasledujúci príkaz v prostredí EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


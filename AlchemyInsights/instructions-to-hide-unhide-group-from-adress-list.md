---
title: Pokyny na skrytie alebo odkrytie skupiny v zozname adries
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831893"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skrytie skupiny v Microsoft 365 v zozname adries

Ak chcete skryť skupinu Microsoft 365 v zoznamoch adries (GAL) klientov Exchange (ako je napríklad Outlook alebo OWA), použite nasledujúci príkaz v prostredí EXO shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Ak chcete skryť skupinu v Microsoft 365 pred jej viditeľnením pre klientov Exchangeu, použite v prostredí EXO tento príkaz:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


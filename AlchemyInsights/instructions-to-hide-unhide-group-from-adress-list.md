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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926260"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skrytie Microsoft 365 v zozname adries

Ak chcete skryť Microsoft 365 v zoznamoch adries (GAL) klientov Exchange (napríklad Outlook alebo OWA), použite nasledujúci príkaz v rámci prostredia EXO:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Ak chcete skryť Microsoft 365, aby sa skupina Exchange klientom, použite nasledujúci príkaz v shellu EXO:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`


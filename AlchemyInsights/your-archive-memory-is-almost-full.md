---
title: Archívna poštová schránka je takmer plná
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974663"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Archívna poštová schránka je takmer plná

Ak používateľ dostane upozornenie, **Archívna poštová schránka je takmer plná** alebo potrebujete zväčšiť veľkosť svojej archívnej poštovej schránky, tu je niekoľko tipov:

1. Ak má používateľ priradenú Exchange Online (plán 1), inovujte na licenciu na **Exchange Online Plan 2** a zvýšte veľkosť zo 50 GB na 100 GB.
1. Ak je už používateľ priradený k niektorej z týchto možností: **Exchange Online Plan 2** alebo Exchange Online (plán 1) pomocou doplnku Exchange Online archivácia, pomocou nasledujúcich krokov môžete povoliť automatické rozšírenie archivácie:.
 
    1. [Pripojte sa k službe Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Spustite nasledovné Group pre používateľa:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Ak chcete potvrdiť, že je pre používateľa povolená, spustite nasledujúce Group:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Ďalšie informácie nájdete v témach:

- [ Povolenie neobmedzenej archivácie – Pomocník pre správcov – Microsoft 365 Compliance | Dokumenty Microsoft](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Limity služby Exchange Online – popisy služieb | Dokumenty Microsoft](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Inovácia na iný podnikový plán | Dokumenty Microsoft](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)


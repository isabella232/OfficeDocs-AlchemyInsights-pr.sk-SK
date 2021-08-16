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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046767"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Archívna poštová schránka je takmer plná

Ak používateľ dostane upozornenie, **Archívna poštová schránka je takmer** plná alebo potrebujete zväčšiť veľkosť archívnej poštovej schránky, tu je niekoľko tipov:

1. Ak má používateľ priradenú licenciu na Exchange Online Plan 1, inovujte na **Exchange Online Plán 2,** aby sa veľkosť zväčšla z 50 GB na 100 GB.
1. Ak už má používateľ priradené niektorú z týchto možností: **Exchange Online Plan 2** alebo plán Exchange Online Plan 1 s doplnok pre Exchange Online – archív, pomocou nižšie uvedených krokov zapnite automatickú archiváciu:.
 
    1. [Pripojenie to Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. Spustite nasledujúce okno commandlet pre používateľa:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Spustením nasledujúceho príkazového riadka potvrďte, že je pre používateľa povolená:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Ďalšie informácie nájdete v téme:

- [Povoliť neobmedzenú archiváciu – Pomocník pre správcov – Microsoft 365 súladu s | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online obmedzenia – informácie o popisoch | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Inovácia na iný plán business | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)


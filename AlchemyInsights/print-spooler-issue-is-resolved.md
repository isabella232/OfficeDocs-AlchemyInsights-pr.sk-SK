---
title: Vyriešil sa problém so zaraďovačom tlače
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911353"
---
# <a name="print-spooler-issue-is-resolved"></a>Vyriešil sa problém so zaraďovačom tlače

Ak bolo zariadenie aktualizované so zostavte Windows 10 **OS 19041.329,** mohli ste si pozorovať problém zlyhania niektorých tlačiarní.   Zaraďovač tlače môže neočakávane zobraziť chybu alebo sa neočakávane zavrieť pri pokuse o tlač a z tlačiarne nie je žiaden výstup. Tento problém je vyriešený v zostavu operačného systému **19041.331** [KB4567523.](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)  

**Priebežný prieskum**

Súbor Local Security Authority Subsystem Service (LSASS) (**Isass.exe**) môže zlyhať v niektorých zariadeniach s chybým hlásením Kritický systémový proces, C:\WINDOWS\system32\Isass.exe, zlyhal s kódom stavu c0000008. Počítač je teraz potrebné reštartovať.  **Spoločnosť Microsoft pracuje na riešení a bude poskytovať aktualizáciu v nadchádzajúcom vydaní.**

Ďalšie informácie nájdete v článku Windows 10 [známe problémy verzie 2004.](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)
---
title: Príklad politiky prílohy v Office 365 Trezor Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7294be81a24fa61a92367bae304798a333cb916c8718e28b1a87314c15ef6c8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988310"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a>Príklad politiky prílohy v Office 365 Trezor Microsoft Defender

Tieto nastavenia umožňujú politiku s názvom *Žiadne oneskorenia,* ktoré okamžite doručujú správy a potom znova priložia prílohy po ich naskenovaní:

- **Názov:** Bez oneskorení
- **Popis:** Správy sa ihneď doručí a po skenovaní prílohy znova priloží.
- **Odpoveď:** Vyberte **možnosť Dynamické doručovanie.** Ďalšie informácie nájdete v téme [Dynamické doručovanie v Trezor príloh.](https://go.microsoft.com/fwlink/?linkid=2092328)
- **Časť Presmerovanie** príloh: Vyberte možnosť Povoliť presmerovanie a potom zadajte e-mailovú adresu globálneho správcu spoločnosti Microsoft 365 správcu zabezpečenia alebo analytika zabezpečenia, ktorý preskúma škodlivé prílohy.
- **Applied To** (Použité na): **Vyberte položku The recipient domain is**(Doména príjemcu je ) a potom vyberte svoju doménu. Vyberte **položku pridať** a potom vyberte tlačidlo **OK**. Po dokončení vyberte položku **Uložiť**.

Ďalšie informácie nájdete v téme [Trezor prílohy v programe Microsoft Defender pre Office 365.](https://go.microsoft.com/fwlink/?linkid=2092213)

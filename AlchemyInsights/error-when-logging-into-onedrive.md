---
title: chyba 0x8004de40 pri spúšťaní OneDrivu
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
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823117"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>chyba 0x8004de40 pri spúšťaní OneDrivu

Ak sa pri prihlasovaní do služby OneDrive zobrazí chybové hlásenie **0x8004de40** , reštartujte počítač pri pripojení k pracovnej alebo školskej doméne. Ak sa po reštartovaní zobrazí táto chyba, skúste to pri pripojení k pracovnej alebo školskej doméne:

1. Kliknite na tlačidlo Štart a do vyhľadávacieho poľa zadajte príkaz **cmd** alebo **Príkazový riadok**  , kliknite pravým tlačidlom myši na aplikáciu príkazového riadka a vyberte položku  **Spustiť ako správca** . Ak sa zobrazí výzva na zadanie hesla správcu alebo na potvrdenie, zadajte heslo alebo kliknite na položku **Povoliť** .  

2. V okne príkazového riadka zadajte **dsregcmd/Leave**  a počkajte, kým sa príkaz dokončí. Potom zadajte **dsregcmd/JOIN** a počkajte, kým sa príkaz dokončí.
3. Reštartujte počítač.

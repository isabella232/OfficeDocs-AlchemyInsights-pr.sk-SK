---
title: 0x8004de40 pri spúšťaní OneDrivu
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
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813667"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 pri spúšťaní OneDrivu

Ak sa pri prihlasovaní **do 0x8004de40** OneDrive zobrazí chybové hlásenie, reštartujte počítač po pripojení k pracovnej alebo školskej doméne. Ak sa táto chyba zobrazí po reštartovaní, skúste to po pripojení k pracovnej alebo školskej doméne:

1. Kliknite na tlačidlo Štart a zadajte **výraz cmd** alebo **príkazový** riadok do vyhľadávacieho poľa, kliknite pravým tlačidlom myši na aplikáciu príkazového riadka a vyberte položku **Spustiť ako správca.** Ak sa zobrazí výzva na zadanie hesla správcu alebo potvrdenie, zadajte heslo alebo kliknite na položku **Povoliť**.  

2. V okne príkazového riadka zadajte **príkaz dsregcmd /leave**  a počkajte, kým sa príkaz dokončí. Potom zadajte **dsregcmd /join** a počkajte, kým sa dokončí príkaz.
3. Reštartujte počítač.

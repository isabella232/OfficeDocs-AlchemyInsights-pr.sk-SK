---
title: 0x8004de40 chybe pri spúšťaní OneDrive
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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946594"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 chybe pri spúšťaní OneDrive

Ak sa pri prihlasovaní **0x8004de40** do počítača OneDrive počítač po pripojení k pracovnej alebo školskej doméne, počítač reštartujte. Ak sa táto chyba zobrazí po reštartovaní, skúste to po pripojení k pracovnej alebo školskej doméne:

1. Kliknite na tlačidlo Štart a zadajte **výraz cmd** alebo **príkazový** riadok do vyhľadávacieho poľa, kliknite pravým tlačidlom myši na aplikáciu príkazového riadka a vyberte položku **Spustiť ako správca.** Ak sa zobrazí výzva na zadanie hesla správcu alebo potvrdenie, zadajte heslo alebo kliknite na položku **Povoliť**.  

2. V okne príkazového riadka zadajte **príkaz dsregcmd /leave**  a počkajte, kým sa príkaz dokončí. Potom zadajte **dsregcmd /join** a počkajte, kým sa dokončí príkaz.
3. Reštartujte počítač.

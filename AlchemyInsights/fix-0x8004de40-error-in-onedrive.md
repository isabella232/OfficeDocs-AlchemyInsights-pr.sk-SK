---
title: Fix 0x8004de40 chyba v OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755863"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Fix 0x8004de40 chyba v OneDrive

Ak sa zobrazí chyba 0x8004de40 OneDrive:

- Reštartujte postihnutého počítača pri pripojení k doméne Acitve adresára.
- Ak sa problém nevyrieši reštartovaním, zrušte pripojenie a znova pripojte zariadenie z Azure AD. 

**Poznámka**: pri vykonávaní týchto krokov by ste mali byť v podnikovej sieti. Nevykonávajte tieto kroky, keď sa nebudete môcť pripojiť k podnikovej infraštruktúre (napríklad pri cestovaní). 

- Otvorte príkazový riadok s právami správcu. 
- Ak chcete otvoriť príkazový riadok s právami správcu, kliknite na tlačidlo **Štart**, kliknite pravým tlačidlom myši na položku **Príkazový riadok**a potom kliknite na položku **Spustiť ako správca**.
- Typ *dsregcmd/opustiť* a stlačte kláves **Enter**.
- Po dokončení zadajte *dsregcmd/JOIN* a stlačte kláves **Enter**.
- Po dokončení zatvorte príkazový riadok.
- Reštartujte počítač a prihláste sa do OneDrivu.
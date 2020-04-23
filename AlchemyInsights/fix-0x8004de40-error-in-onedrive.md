---
title: Fix 0x8004de40 chyba v OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 5da4271f242597b195ef61d553fd4a2ffb313025
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716043"
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
---
title: Oprava chyby 0x8004de40 vo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745145"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Oprava chyby 0x8004de40 vo OneDrive

Ak sa v službe OneDrive zobrazí chyba 0x8004de40:

- Reštartujte postihnutý počítač pri pripojení k doméne adresára Acitve.
- Ak sa problém nevyrieši reštartovaním, odhláste sa a znova sa prihláste do svojho zariadenia zo služby Azure AD. 

**Poznámka**: pri vykonaní týchto krokov by ste sa mali nachádzať v podnikovej sieti. Nevykonávajte tieto kroky, ak sa nedokážete pripojiť k podnikovej infraštruktúre (napríklad na cestách). 

- Otvorte príkazový riadok s právami správcu. 
- Ak chcete otvoriť príkazový riadok s právami správcu, kliknite na tlačidlo **Štart**, kliknite pravým tlačidlom myši na **Príkazový riadok**a potom kliknite na položku **Spustiť ako správca**.
- Zadajte *dsregcmd/Leave* a stlačte kláves **Enter**.
- Po vyplnení zadajte *dsregcmd/JOIN* a stlačte kláves **Enter**.
- Po skončení zatvoríte príkazový riadok.
- Reštartujte počítač a prihláste sa do služby OneDrive.
---
title: Oprava 0x8004de40 chyby v službe OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525074"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Oprava 0x8004de40 chyby v službe OneDrive

Ak sa zobrazí chybové hlásenie 0x8004de40 s OneDrive:

- Reštartujte postihnutého počítača, keď ste pripojení k doméne atívny adresár.
- Ak sa problém nevyrieši reštartovaním počítača, odpojenie a opusťte zariadenia z Azure AD. 

**Poznámka**: mali by ste byť na vašej firemnej sieti pri vykonávaní týchto krokov. Nemusíte vykonávať tieto kroky, keď nie ste schopní sa pripojiť k vašej firemnej infraštruktúry (napríklad pri cestovaní). 

- Otvorte námer kontrolovať vrtký. 
- Otvorte námer kontrolovať vrtký, kliknutím na tlačidlo - **Štart**, kliknite pravým tlačidlom myši **Príkazový riadok**a potom kliknite na položku **Spustiť ako správca**.
- Zadajte *dsregcmd /leave* a stlačte kláves **Enter**.
- Po dokončení *zadajte/JOIN dsregcmd* a stlačte kláves **Enter**.
- Keď kompletné, zatvorte príkazový riadok.
- Reštartujte počítač a prihláste sa do OneDrive.
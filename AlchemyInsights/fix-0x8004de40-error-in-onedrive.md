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
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133991"
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
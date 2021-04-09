---
title: Oprava 0x8004de40 vo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649763"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>Oprava 0x8004de40 vo OneDrive

Ak používate Windows 7 a zobrazí sa táto chyba, pri aktualizácii zapnite protokol [TLS 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ako predvolené zabezpečené protokoly v systéme WinHTTP vo Windowse.

Ak používate Windows 10 a vo OneDrive sa 0x8004de40 chyba:

- Po pripojení k doméne adresára Acitve reštartujte ovplyvnený počítač.
- Ak reštartovanie nepomôže problém vyriešiť, odpojte sa a znova sa pripojiť k zariadeniu zo služby Azure AD. 

**Poznámka:** Pri vykonávaní týchto krokov by ste sa mali nachádzať vo vašej podnikovej sieti. Tieto kroky nepoužívajte, keď nie ste pripojení k podnikovej infraštruktúre (napríklad na cestách). 

1. Výberom tlačidla Štart otvorte príkazový riadok bez **oprávnení**, kliknite pravým tlačidlom myši na **položku Príkazový** riadok a potom **vyberte položku Spustiť ako správca.**

1. Zadajte *dsregcmd /leave a* stlačte kláves **Enter.**

1. Po dokončení zadajte *dsregcmd /join a* stlačte kláves **Enter.**

1. Po dokončení zatvorte príkazový riadok.

1. Reštartujte počítač a prihláste sa do služby OneDrive.
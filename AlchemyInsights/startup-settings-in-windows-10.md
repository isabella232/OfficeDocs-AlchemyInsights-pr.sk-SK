---
title: Nastavenie spustenia v Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909841"
---
# <a name="startup-settings-in-windows-10"></a>Nastavenie spustenia v Windows 10

**Zmena aplikácií, ktoré sa spúšťajú automaticky pri spustení**

1. Prejdite do [Nastavenia > Aplikácie > Spustenie.](ms-settings:startupapps?activationSource=GetHelp)

2. Skontrolujte, či je aplikácia, ktorú chcete spustiť pri spustení, **zapnutá.**

**Pridanie aplikácie na automatické spustenie pri spustení**

1. Kliknite alebo **ťuknite na** tlačidlo Štart a vyhľadajte aplikáciu, ktorú chcete spustiť pri spustení.

2. Kliknite pravým tlačidlom myši na aplikáciu, kliknite **na položku** Ďalšie a potom kliknite na položku Otvoriť **umiestnenie súboru**. Otvorí sa umiestnenie, kde je uložená odkaz na aplikáciu. Ak nie je k dispozícii možnosť Otvoriť umiestnenie súboru, znamená to, že aplikácia sa nemôže spustiť pri spustení.

3. V otvorenom umiestnení súboru stlačte kombináciu klávesov Windows kláves s **logom + R,** zadajte **reťazec shell:startup** a potom kliknite na tlačidlo **OK**. Otvorí sa priečinok Pri spustení.

4. Skopírujte a prilepte odkaz na aplikáciu z umiestnenia súboru do priečinka Pri spustení.

**Rozšírené možnosti spustenia (vrátane Trezor UEFI a spúšťania z iného zariadenia)**

1. Uložte svoju prácu a zavrite všetky otvorené dokumenty, pretože pomocou týchto krokov sa počítač reštartuje.

2. Prejdite na [Nastavenia > Aktualizácia & obnovenie > zabezpečenia.](ms-settings:recovery?activationSource=GetHelp)

3. V **časti Rozšírené spustenie** kliknite na položku **Reštartovať.** 

4. Po reštartovaní počítača na obrazovke Výber možnosti:

    - Ak chcete spustiť systém zo zariadenia, ako je napríklad USB kľúč, **kliknite na položku Použiť zariadenie.**

    - Ak chcete zadať nastavenia UEFI (niekedy sa nazývajú aj NASTAVENIA FIRME), kliknite na položku **> rozšírené možnosti > firmvéru UEFI Nastavenia.** 

    - Ak chcete spustiť Trezor alebo zmeniť rozšírené nastavenia spustenia, kliknite na položku **Riešiť problémy > rozšírených > ponuke Nastavenia** a potom kliknite na položku **Reštartovať**. Môže sa zobraziť výzva na zadanie kľúča na obnovenie [pre šifrovanie BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Po reštartovaní počítača znova kliknite na nastavenie spustenia, ktoré chcete použiť.
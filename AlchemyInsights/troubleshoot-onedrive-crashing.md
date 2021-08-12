---
title: Riešenie OneDrive zlyhaní
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921022"
---
# <a name="troubleshoot-onedrive-crashes"></a>Riešenie OneDrive zlyhaní

Ak OneDrive opakovane zlyhá, vyskúšajte tieto kroky na riešenie problémov:

**Presvedčte sa, že kľúče databázy Registry nie sú nastavené:**

1. Pomocou Editora databázy Registry prejdite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ak je k dispozícii DisableFileSyncNGSC a je nastavený na možnosť 1, otvorte kľúč a zmeňte hodnotu na 0.
3. Manuálne spustenie OneDrive v ponuke Štart ![Stlačte kláves Windows klávesov](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), zadajte OneDrive do vyhľadávacieho poľa a potom kliknite na počítačovú OneDrive aplikáciu.

**Vynulovanie OneDrive:**

Poznámky:

- Obnovenie OneDrive odpojí všetky existujúce synchronizačné pripojenia (vrátane vášho OneDrive, ak máte nastavené).
- Vynulovaním nastavení údajov v počítači nestratíte OneDrive súbory ani údaje.

**Vynulovanie OneDrive:**

1. Stlačením klávesu R otvorte dialógové Windows Spustiť.
2. Zadajte príkaz %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stlačte tlačidlo OK. Na chvíľu sa môže zobraziť okno Príkazový riadok.
3. Manuálne spustenie OneDrive v ponuke Štart ![Stlačte kláves Windows klávesov](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), zadajte OneDrive do vyhľadávacieho poľa a potom kliknite na počítačovú OneDrive aplikáciu.

Poznámky:

- Ak ste pred vynulním nastavení vybrali synchronizáciu iba niektorých priečinkov, budete to po synchronizácii musieť urobiť ešte raz. Ďalšie [informácie nájdete v OneDrive Výber priečinkov na synchronizáciu](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)s   počítačom.
- Toto budete musieť dokončiť pre svoje osobné OneDrive a OneDrive for Business.
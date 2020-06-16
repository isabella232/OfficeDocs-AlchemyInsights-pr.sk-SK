---
title: Riešenie problémov s onedrivom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749168"
---
# <a name="troubleshoot-onedrive-crashes"></a>Riešenie problémov s onedrivom

Ak OneDrive opakovane zlyhá, vyskúšajte tieto kroky na riešenie problémov:

**Uistite sa, že kľúče databázy registry nie sú nastavené:**

1. Pomocou Editora databázy Registry prejdite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ak DisableFileSyncNGSC je prítomný a nastavená na 1, otvorte kľúč a zmeňte hodnotu 0.
3. Manuálne spustenie OneDrivu prechodom na domovskú obrazovku ![Stlačte kláves s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.

**Obnovenie onedrivu:**

Poznámky:

- Obnovením výrobných nastavení OneDrivu sa odpojí všetky existujúce pripojenia synchronizácie (vrátane osobného OneDrivu, ak je nastavený).
- Nestratíte súbory ani údaje obnovením nastavenia OneDrivu v počítači.

**Obnovenie nastavenia OneDrivu:**

1. Stlačením klávesu s logom Windows a R otvorte dialógové okno Spustiť.
2. Zadajte reťazec %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stlačte tlačidlo OK. Krátko sa môže zobraziť okno príkazu.
3. Manuálne spustenie OneDrivu prechodom na domovskú obrazovku ![Stlačte kláves s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.

Poznámky:

- Ak ste sa rozhodli synchronizovať iba niektoré priečinky pred obnovením, budete musieť urobiť znova po dokončení synchronizácie. Ďalšie informácie nájdete v téme [Výber priečinkov onedrivu, ktoré sa majú synchronizovať s počítačom.](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)  
- Budete ho musieť dokončiť pre svoj osobný OneDrive a OneDrive for Business.
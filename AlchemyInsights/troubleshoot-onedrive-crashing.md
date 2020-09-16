---
title: Riešenie problémov s zlyhávaním OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665013"
---
# <a name="troubleshoot-onedrive-crashes"></a>Riešenie problémov s zlyhávaním OneDrivu

Ak OneDrive opakovane zlyháva, vyskúšajte tieto kroky na riešenie problémov:

**Uistite sa, že kľúče databázy Registry nie sú nastavené:**

1. Pomocou editora databázy Registry prejdite na HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Ak je DisableFileSyncNGSC prítomný a nastavený na hodnotu 1, otvorte kľúč a zmeňte hodnotu na 0.
3. Manuálne spustenie OneDrivu prechodom na domovskú obrazovku ![Stlačenie klávesu s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.

**Obnoviť OneDrive:**

Poznámok

- Obnovením nastavenia služby OneDrive sa odpojí všetky existujúce synchronizačné pripojenia (vrátane vášho osobného OneDrivu, ak je nastavené).
- Nestratíte žiadne súbory ani údaje vykonaním nastavenia služby OneDrive v počítači.

**Obnovenie služby OneDrive:**

1. Stlačením klávesu s logom Windows a klávesu R otvorte dialógové okno spustiť.
2. Zadajte výraz% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset a stlačte tlačidlo OK. Okno s príkazom sa môže zobraziť stručne.
3. Manuálne spustenie OneDrivu prechodom na domovskú obrazovku ![Stlačenie klávesu s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.

Poznámok

- Ak ste sa pred vynulovaním rozhodli synchronizovať iba niektoré priečinky, bude potrebné vykonať túto operáciu znova po dokončení synchronizácie. Ďalšie informácie nájdete v [téme Výber priečinkov OneDrivu, ktoré sa majú synchronizovať s počítačom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   .
- Túto možnosť budete musieť vyplniť pre svoje osobné služby OneDrive a OneDrive for Business.
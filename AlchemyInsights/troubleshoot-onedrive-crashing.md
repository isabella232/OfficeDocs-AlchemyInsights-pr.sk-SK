---
title: Riešenie problémov so zlyhaním OneDrivu
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826214"
---
# <a name="troubleshoot-onedrive-crashes"></a>Riešenie problémov so zlyhaním OneDrivu

Ak OneDrive opakovane zlyhá, vyskúšajte tieto kroky na riešenie problémov:

**Presvedčte sa, že kľúče databázy Registry nie sú nastavené:**

1. Pomocou Editora databázy Registry prejdite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ak je k dispozícii DisableFileSyncNGSC a je nastavený na možnosť 1, otvorte kľúč a zmeňte hodnotu na 0.
3. Manuálne spustenie OneDrivu pomocou ponuky Štart ![Stlačte kláves s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.

**Vynulovanie nastavenia pre OneDrive:**

Poznámky:

- Vynulovaním nastavenia pre OneDrive sa odpoja všetky existujúce synchronizačné pripojenia (vrátane vášho osobného konta vo OneDrive, ak ho máte nastavené).
- Vynulovaním nastavení služby OneDrive v počítači nestratíte žiadne súbory ani údaje.

**Vynulovanie nastavenia pre OneDrive:**

1. Otvorte dialógové okno Spustiť stlačením klávesu s logom Windows a klávesu R.
2. Zadajte príkaz %localappdata%\Microsoft\OneDrive\onedrive.exe /reset a stlačte tlačidlo OK. Na chvíľu sa môže zobraziť okno Príkazový riadok.
3. Manuálne spustenie OneDrivu pomocou ponuky Štart ![Stlačte kláves s logom Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), do vyhľadávacieho poľa zadajte výraz OneDrive a potom kliknite na počítačovú aplikáciu OneDrive.

Poznámky:

- Ak ste pred vynulním nastavení vybrali synchronizáciu iba niektorých priečinkov, budete to po synchronizácii musieť urobiť ešte raz. Ďalšie [informácie nájdete v článku Výber priečinkov OneDrivu na synchronizáciu](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)s   počítačom.
- Tento problém budete musieť dokončiť pre svoj osobný OneDrive a OneDrive for Business.
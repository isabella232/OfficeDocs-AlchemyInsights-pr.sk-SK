---
title: Klient Teams zlyháva?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030673"
---
# <a name="teams-client-crashing"></a>Klient Teams zlyháva?

Ak váš klient Teams zlyháva, vyskúšajte tento postup:

- Ak používate počítačovú aplikáciu Teams, [uistite sa, že aplikácia je aktualizovaná na najnovšiu verziu](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Uistite sa, že všetky [URL adresy a rozsahy adries služby Office 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) sú dostupné.

- Prihláste sa so svojím kontom správcu a na [tabuli stavu služby](https://docs.microsoft.com/office365/enterprise/view-service-health) overte, či nedochádza k výpadku alebo zhoršeniu služby.

 - Ako posledný krok sa môžete pokúsiť vymazať vyrovnávaciu pamäť klienta Teams:

    1.  Úplne ukončite počítačového klienta Microsoft Teams. Môžete kliknúť pravým tlačidlom myši na ikonu **Teams** na paneli úloh a kliknúť na položku **Ukončiť** alebo spustiť správcu úloh a ukončiť proces.

    2.  Prejdite do Prieskumníka a zadajte %appdata%\Microsoft\teams.

    3.  Keď sa budete nachádzať v uvedenom adresári, zobrazia sa niektoré z týchto priečinkov:

         - V priečinku **Application Cache** prejdite do priečinka Cache a odstráňte všetky súbory v priečinku Cache: %appdata%\Microsoft\teams\application cache\cache.

        - V priečinku **Blob_storage** odstráňte všetky súbory: %appdata%\Microsoft\teams\blob_storage.

        - V priečinku **Cache** odstráňte všetky súbory: %appdata%\Microsoft\teams\Cache.

        - V priečinku **databases** odstráňte všetky súbory: %appdata%\Microsoft\teams\databases.

        - V priečinku **GPUCache** odstráňte všetky súbory: %appdata%\Microsoft\teams\GPUcache.

        - V priečinku **IndexedDB** odstráňte súbor .db: %appdata%\Microsoft\teams\IndexedDB.

        - V priečinku **Local Storage** odstráňte všetky súbory: %appdata%\Microsoft\teams\Local Storage.

        - A napokon v priečinku **tmp** odstráňte všetky súbory: %appdata%\Microsoft\teams\tmp.

    4. Znova spustite klienta Teams.

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
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354068"
---
# <a name="teams-client-crashing"></a>Klient Teams zlyháva?

Ak váš klient Teams zlyháva, vyskúšajte tento postup:

- Ak používate počítačovú aplikáciu Teams, [uistite sa, že aplikácia je aktualizovaná na najnovšiu verziu](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Uistite sa, že všetky [Microsoft 365 adresy URL a rozsahy adries](https://docs.microsoft.com/microsoftteams/connectivity-issues) sú prístupné.

- Prihláste sa pomocou konta správcu nájomníka a skontrolujte, či sa v [informačnom paneli služby](https://docs.microsoft.com/office365/enterprise/view-service-health) nenachádza žiadna výpadok alebo degradácia služieb.

- Odinštalovanie a preinštalovanie aplikácie Teams (prepojenie)
    - Prejdite do priečinka%appdata%\Microsoft\teams\ v počítači a odstráňte všetky súbory v tomto adresári.
    - [Prevezmite a nainštalujte aplikáciu teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)a ak je to možné, nainštalujte tímy ako správca (kliknite pravým tlačidlom myši na Inštalátor tímov a vyberte možnosť "spustiť ako správca", ak je k dispozícii).

Ak vaše tímy klient je stále havaruje, môžete reprodukovať problém? Ak áno:

1. Použite postup rekordér zachytiť vaše kroky.
    - Zatvorte všetky nepotrebné alebo dôverné aplikácie.
    - Spustenie postupu rekordér a reprodukovať problém pri prihlásení pomocou príslušného používateľského konta.
    - [Zbierať tímy denníky, ktoré zachytávajú zaznamenané repro kroky](https://docs.microsoft.com/microsoftteams/log-files). **Poznámka**: Uistite sa, že zachytiť adresu prihlásenia ovplyvnenej používateľa.
    - Zhromažďovať dump a/alebo chyba vedierko info (Windows). Spustenie prostredia Windows PowerShell na stroji, kde dochádza k zlyhaniu a spustite nasledujúce príkazy:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Priložte súbor k vášmu prípadu podpory.

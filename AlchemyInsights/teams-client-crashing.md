---
title: Klient Teams zlyháva?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826286"
---
# <a name="teams-client-crashing"></a>Klient Teams zlyháva?

Ak váš klient Teams zlyháva, vyskúšajte tento postup:

- Ak používate počítačovú aplikáciu Teams, [uistite sa, že aplikácia je aktualizovaná na najnovšiu verziu](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Skontrolujte, či sú všetky URL adresy a rozsahy adries v Microsoft [365](https://docs.microsoft.com/microsoftteams/connectivity-issues) prístupné.

- Prihláste sa pomocou svojho konta správcu nájomníka a skontrolujte tabuľu [stavu](https://docs.microsoft.com/office365/enterprise/view-service-health) služby a overte, či k dispozícii nie sú žiadne výpadky ani zníženie úrovne služieb.

- Odinštalovanie a opätovné nainštalovanie aplikácie Teams (prepojenie)
    - Prejdite do priečinka %appdata%\Microsoft\teams\ v počítači a odstráňte všetky súbory v tomto adresári.
    - [Stiahnite a nainštalujte aplikáciu Teams.](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)Ak je to možné, nainštalujte si Teams ako správca (kliknite pravým tlačidlom myši na inštalátor aplikácie Teams a vyberte možnosť "Spustiť ako správca", ak je k dispozícii).

Ak váš klient Teams stále zlyháva, môžete problém reprodukovať? Ak áno:

1. Pomocou diktafónu krokov zaznamenajte svoje kroky.
    - Zavrite všetky nepotrebné alebo dôverné aplikácie.
    - Spustite záznam krokov a reprodukovať problém, keď ste prihlásení pomocou príslušného používateľského konta.
    - [Zhromaždite záznamy o tímoch, ktoré zaznamenávajú zaznamenané kroky opätovného zabezpečenia.](https://docs.microsoft.com/microsoftteams/log-files) **Poznámka:** Nezabudnite zaznamenať prihlasovaciu adresu o vplyve používateľa.
    - Zhromaždenie informácií o výpise alebo chybe kontajnera (Windows). Spustite prostredie Windows Powershell v počítači, v ktorom dochádza k zlyhaiu, a spustite nasledujúce príkazy:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Priložte súbor k prípadu podpory.

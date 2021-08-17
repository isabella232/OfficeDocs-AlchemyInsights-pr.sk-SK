---
title: Teams klient zlyháva
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
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890353"
---
# <a name="teams-client-crashing"></a>Teams klient zlyháva

Ak váš klient Teams zlyháva, vyskúšajte tento postup:

- Ak používate počítačovú aplikáciu Teams, [uistite sa, že aplikácia je aktualizovaná na najnovšiu verziu](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Skontrolujte, či sú [všetky Microsoft 365 URL adresy a rozsahy adries](https://docs.microsoft.com/microsoftteams/connectivity-issues) prístupné.

- Prihláste sa pomocou svojho konta správcu nájomníka a skontrolujte tabuľu [stavu](https://docs.microsoft.com/office365/enterprise/view-service-health) služby a overte, či k dispozícii nie sú žiadne výpadky ani zníženie úrovne služieb.

- Odinštalovanie a opätovné nainštalovanie Teams aplikácie
    - Prejdite do priečinka %appdata%\Microsoft\Teams\ v počítači a odstráňte všetky súbory z tohto adresára.
    - [Stiahnite](https://www.microsoft.com/microsoft-teams/download-app)a nainštalujte Teams App a ak je to možné, nainštalujte Teams ako správca (kliknite pravým tlačidlom myši na inštalátor balíka Teams a vyberte položku Spustiť ako **správca,** ak je k dispozícii).

Ak Teams klienta stále zlyháva, pokúste sa problém reprodukovať. Ak môžete:

1. Pomocou diktafónu krokov zaznamenajte svoje kroky.
    - Zavrite všetky nepotrebné alebo dôverné aplikácie.
    - Spustite záznam krokov a reprodukovať problém, keď ste prihlásení pomocou príslušného používateľského konta.
    - [Zhromaždite záznamy o tímoch, ktoré zaznamenávajú zaznamenané kroky opätovného zabezpečenia.](https://docs.microsoft.com/microsoftteams/log-files) **Poznámka:** Nezabudnite zaznamenať prihlasovaciu adresu o vplyve používateľa.
    - Zhromaždenie informácií o výpise alebo chybe kontajnera (Windows). Spustite Windows PowerShell v počítači, v ktorom sa vyskytuje zlyhanie, a spustite nasledujúce príkazy (po každom príkaze stlačte kláves Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Po vygenerovaní textového súboru, ktorý sa zobrazí na obrazovke, uložte súbor a priložte ho k žiadosti o službu. 

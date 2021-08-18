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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321640"
---
# <a name="teams-client-crashing"></a>Teams klient zlyháva

Ak váš klient Teams zlyháva, vyskúšajte tento postup:

- Ak používate počítačovú aplikáciu Teams, [uistite sa, že aplikácia je aktualizovaná na najnovšiu verziu](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Skontrolujte, či sú [všetky Microsoft 365 URL adresy a rozsahy adries](https://docs.microsoft.com/microsoftteams/connectivity-issues) prístupné.

- Prihláste sa pomocou svojho konta správcu nájomníka a skontrolujte tabuľu [stavu](https://docs.microsoft.com/office365/enterprise/view-service-health) služby a overte, či k dispozícii nie sú žiadne výpadky ani zníženie úrovne služieb.

- Odinštalovanie a opätovné nainštalovanie Teams aplikácie
    - Prejdite do priečinka %appdata%\Microsoft\Teams\ v počítači a odstráňte všetky súbory z tohto adresára.
    - [Stiahnite a nainštalujte aplikáciu Teams](https://www.microsoft.com/microsoft-teams/download-app)a ak je Teams možné, nainštalujte ako správcu (kliknite pravým tlačidlom myši na inštalátor balíka Teams a vyberte položku Spustiť ako **správca,** ak je k dispozícii).

Ak Teams klienta stále zlyháva, pokúste sa problém reprodukovať. Ak môžete:

1. Pomocou diktafónu krokov zaznamenajte svoje kroky.
    - Zavrite všetky nepotrebné alebo dôverné aplikácie.
    - Spustite záznam krokov a reprodukovať problém, keď ste prihlásení pomocou príslušného používateľského konta.
    - [Zhromaždite záznamy o tímoch, ktoré zaznamenávajú zaznamenané kroky opätovného zabezpečenia.](https://docs.microsoft.com/microsoftteams/log-files) 
    
    **Poznámka:** Nezabudnite zaznamenať prihlasovaciu adresu o vplyve používateľa.
    - Zhromaždenie informácií o výpise alebo chybe kontajnera (Windows). Spustite Windows Powershell v počítači, v ktorom sa vyskytuje zlyhanie, a spustite nasledujúce príkazy (po každom príkaze stlačte kláves Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Po vygenerovaní textového súboru, ktorý sa zobrazí na obrazovke, uložte súbor a priložte ho k žiadosti o službu. 

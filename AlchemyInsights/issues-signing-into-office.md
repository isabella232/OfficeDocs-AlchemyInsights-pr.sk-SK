---
title: Problémy s prihlásením do aplikácie balíka Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938334"
---
# <a name="issues-signing-in-to-office-apps"></a>Problémy s prihlásením do aplikácie balíka Office

Vyriešiť prihlasovaním s kancelárskymi aplikáciami, vyskúšajte nasledujúci postup:

- Odstráňte všetky pracovné účty, okrem postihnutých konta pomocou nastavenia systému Windows > **prístup k práci alebo v škole**.
- [Jasné úradu poverení](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou poverení správcu systému Windows.<br/>
    **Poznámka:** Cesty databázy registry Office 2016 zmenili 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorte aplikáciu balíka Office, vyberte **súbor** > **účet** > **Odhlásiť**. Potom sa prihláste pomocou používateľského konta s platnou licenciou. Podrobné informácie nájdete v téme [kontá v kancelárii](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- Pre Mac, pozri [nemôžete prihlásiť do Office 2016 pre Mac aplikácie](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Ak chyby sa vyskytuje pri pripájaní k Office 365 pomocou Office 2013, umožňujú moderné overenie Office klienta.

Ďalšie informácie nájdete v téme:
- [Nemôžete prihlásiť k Office 365, Azure alebo Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Problémy s pripojením v sign-in po aktualizácii Office 2016 build 16.0.7967 v systéme Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Prepáč, iný účet z vašej organizácie je už prihlásený na tomto počítači" v kancelárii](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Riešenie problémov prihlasovacích Office moderných overovanie pri používaní ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)
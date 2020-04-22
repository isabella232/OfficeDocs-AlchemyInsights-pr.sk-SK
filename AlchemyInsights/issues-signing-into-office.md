---
title: Problémy s prihlásením do aplikácií balíka Office
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763016"
---
# <a name="issues-signing-in-to-office-apps"></a>Problémy s prihlásením do aplikácií balíka Office

Ak chcete opraviť problémy s prihlásením v aplikáciách balíka Office, vyskúšajte nasledujúce kroky:

- Odstráňte všetky pracovné kontá okrem príslušného konta pomocou nastavenia systému Windows > **prístup k práci alebo škole**.
- [Vymažte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br/>
    **Poznámka:** Cesty databázy Registry pre balík Office 2016 sa zmenili na 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorte aplikáciu balíka Office, vyberte položku**konto** >  **súboru** > **odhlásiť**. Potom sa prihláste pomocou používateľského konta s platnou licenciou. Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- V prípade Macu si pozrite tému [Nemôžem sa prihlásiť do aplikácie balíka Office 2016 pre Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).
- Ak sa chyby pri pripájaní k Microsoft 365 pomocou Office 2013, povoliť moderné overovanie pre klienta Office.

Ďalšie informácie nájdete v témach:
- [Nemôžete sa prihlásiť do Microsoft 365, Azure alebo Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [Problémy s pripojením v prihlásenie po aktualizácii na balík Office 2016 build 16.0.7967 v systéme Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["Ľutujeme, iný účet z vašej organizácie je už prihlásený na tomto počítači" v balíku Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [Riešenie problémov s prihlásením s Office moderné overovanie pri použití ADFS](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)
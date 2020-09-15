---
title: Problémy s prihlásením do aplikácií Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695338"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Riešenie problémov s aplikáciou Microsoft 365 Ľutujeme, ale v správe je už prihlásení ďalšie konto z vašej organizácie

Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:

- Odstráňte všetky pracovné kontá okrem príslušného konta pomocou nastavení Windowsu > **Accessu alebo v škole**.
- [Vymazanie poverení balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br/>
    **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorte aplikáciu balíka Office, vyberte **File**možnosť  >  **Account**  >  **odhlásiť sa z**konta súboru. Potom sa prihláste pomocou používateľského konta s platnou licenciou. Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- V prípade Macu si pozrite tému [Nemôžem sa prihlásiť do aplikácie balíka Office 2016 pre Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Ďalšie informácie nájdete v téme [Ľutujeme, ďalšie konto z vašej organizácie je už v tomto počítači prihlásení v Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).
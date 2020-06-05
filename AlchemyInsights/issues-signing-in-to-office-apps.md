---
title: Problémy s prihlásením do aplikácií Microsoft 365
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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579952"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Správa O nastavení aplikácie Microsoft 365 Ľutujeme, ďalšie konto z vašej organizácie je už prihlásený

Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:

- Odstráňte všetky pracovné kontá okrem príslušného konta pomocou nastavení systému Windows > **accessovej práce alebo školy**.
- [Vymažte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou správcu poverení systému Windows.<br/>
    **Upozornenie:** Cesty databázy registry pre Office 2016 sa zmenili na 16.0. (Napr.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorte aplikáciu balíka Office a vyberte položku **File**  >  **Account**  >  **Odhláste sa**v konte súboru . Potom sa prihláste pomocou používateľského konta s platnou licenciou. Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- V prípade Macu si pozrite tému [Nemôžem sa prihlásiť do aplikácie balíka Office 2016 pre Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Ďalšie informácie nájdete v časti ["Ľutujeme, v tomto počítači je už prihlásenie iného konta z vašej organizácie" v balíku Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).
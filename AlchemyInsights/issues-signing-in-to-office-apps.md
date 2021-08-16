---
title: Problémy pri prihlasovaní do Microsoft 365 aplikácií
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028055"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>Oprava Microsoft 365 s hlásením "Ľutujeme, iné konto z vašej organizácie je už prihlásené"

Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:

- Odstráňte všetky pracovné kontá s výnimkou príslušného konta pomocou Windows Nastavenia > **pracovného alebo školského konta**.
- [Zrušte začiarknutie Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Windows Správca poverení.<br/>
    **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na hodnotu 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Otvorte konto aplikácia Office položku File  >  **Account**  >  **Sign Out (Odhlásiť sa).** Potom sa prihláste pomocou používateľského konta s platnou licenciou. Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- V prípade Macu si pozrite tému [Nemôžem sa prihlásiť do aplikácie balíka Office 2016 pre Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).

Ďalšie informácie nájdete v téme Ľutujeme, v téme Iné konto z vašej organizácie je už v tomto počítači [prihlásené Office.](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
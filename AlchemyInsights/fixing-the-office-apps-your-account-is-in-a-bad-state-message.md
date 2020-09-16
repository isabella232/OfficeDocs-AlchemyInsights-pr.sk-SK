---
title: Oprava aplikácií Microsoft 365, ktoré sa vo vašom konte nachádzajú v chybnom stave
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744560"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Oprava aplikácií Microsoft 365 "vaše konto je v chybnom stave"

Ak chcete túto chybu odstrániť, vyskúšajte v dotknutom počítači nasledovné možnosti:

- Otvorte aplikáciu balíka Office, vyberte položku **súbor**  >  **konta**sa  >  **odhláste zo všetkých kont**. Znova sa prihláste pomocou používateľského konta s platnou licenciou. Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Vymazanie poverení balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br>
  **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na 16,0. Napríklad \Software\Microsoft\Office\16.0\Common\Identity\
- Ak sa chyba vyskytuje pri pripájaní k balíku Office 365 pomocou balíka Office 2013, [povolenie moderného overovania](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) pre klienta balíka Office.

Ďalšie informácie nájdete v téme [Riešenie problémov s aplikáciami mimo prehliadača, ktoré sa nemôžu prihlásiť do služieb Microsoft 365, Azure alebo Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).


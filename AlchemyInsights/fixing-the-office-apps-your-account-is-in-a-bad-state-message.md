---
title: Oprava Microsoft 365 aplikácií Vaše konto je v chybom stave
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
- "2558"
- "9000571"
ms.openlocfilehash: 68c4dfcc0500761f8ce5090fddb9f2ad58af77bc411c9e714b14c383fef177de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068251"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Oprava Microsoft 365 chyby Vaše konto je v zlom stave

Ak chcete túto chybu opraviť, skúste v ovplyvnenému počítači použiť tieto možnosti:

- Otvorte aplikáciu aplikácia Office vyberte položku **File** Account Sign Out of all accounts (Konto súboru sa  >    >  **odhlásiť zo všetkých kont).** Znova sa prihláste pomocou používateľského konta s platnou licenciou. Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Zrušte začiarknutie Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Windows Správca poverení.<br>
  **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na hodnotu 16.0. Príklad: \Software\Microsoft\Office\16.0\Common\Identity\
- Ak sa chyba vyskytne pri pripájaní k Office 365 pomocou Office 2013, zapnite [moderné](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) overovanie Office klienta.

Ďalšie informácie nájdete v téme Riešenie problémov s aplikáciami, ktoré nie sú prehliadačmi a nemôže sa prihlásiť do služieb [Microsoft 365, Azure alebo Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)


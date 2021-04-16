---
title: Oprava aplikácií služby Microsoft 365 V hlásení o stave vášho konta sa zobrazuje chybná správa
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
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812551"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>Oprava chyby aplikácie Microsoft 365 Vaše konto je v chybovom stave

Ak chcete túto chybu opraviť, skúste v ovplyvnenému počítači použiť tieto možnosti:

- Otvorte aplikáciu balíka Office, vyberte **položku File**  >  **Account** Sign Out of all  >  **accounts (Odhlásiť sa zo všetkých kont).** Znova sa prihláste pomocou používateľského konta s platnou licenciou. Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Odstráňte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br>
  **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na hodnotu 16.0. Príklad: \Software\Microsoft\Office\16.0\Common\Identity\
- Ak sa pri pripájaní k balíku Office 365 pomocou balíka Office 2013 vyskytne chyba, zapnite [pre](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) klienta Office moderné overovanie.

Ďalšie informácie nájdete v téme Riešenie problémov s aplikáciami, ktoré nie sú prehliadačmi a nemôže sa prihlásiť do služieb [Microsoft 365, Azure alebo Intune.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)


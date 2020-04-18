---
title: Oprava aplikácií balíka Office váš účet je v zlom stave správy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: b28865ff1da434a254c9051183074be35cdd0252
ms.sourcegitcommit: 9b2b162ad651e2c3d9d0c746f67a78334592f076
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/17/2020
ms.locfileid: "43547977"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Oprava aplikácie balíka Office "váš účet je v zlom stave" chyba

Ak chcete opraviť túto chybu, vyskúšajte nasledujúce možnosti na postihnutý počítač:

- Otvorte aplikáciu balíka Office, vyberte položku**konto** >  **súboru** > **odhlásiť zo všetkých účtov**. Prihláste sa znova pomocou používateľského konta s platnou licenciou. Podrobné informácie sa nachádzajú v téme [Kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Vymažte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br>
  **Poznámka:** Cesty databázy Registry pre balík Office 2016 sa zmenili na 16,0. Napríklad \Software\Microsoft\Office\16.0\Common\Identity\
- Ak sa vyskytne chyba pri pripájaní k Office 365 pomocou Office 2013, [Povoliť moderné overovanie](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) pre klienta Office.

Ďalšie informácie nájdete v téme [Riešenie problémov s aplikáciami, ktoré nie sú prehľadávačom, ktoré sa nedajú prihlásiť do balíka Office 365, Azure alebo Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).


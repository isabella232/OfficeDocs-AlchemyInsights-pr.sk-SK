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
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969781"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>Oprava aplikácie balíka Office "váš účet je v zlom stave" chyba

Ak chcete opraviť túto chybu, vyskúšajte nasledujúce možnosti na postihnutý počítač:

- Otvorte aplikáciu balíka Office, vyberte položku**konto** >  **súboru** > **odhlásiť zo všetkých účtov**. Prihláste sa znova pomocou používateľského konta s platnou licenciou. Podrobné informácie nájdete v téme [kontá v balíku Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [Vymažte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br>
  **Poznámka:** Cesty databázy Registry pre balík Office 2016 sa zmenili na 16,0. Napríklad \Software\Microsoft\Office\16.0\Common\Identity\
- Na postihnutý počítač, nastavte EnableADAL = 0 pomocou nasledujúcich krokov:  
     1. Kliknite pravým tlačidlom myši na tlačidlo Windows a vyberte **Spustiť**. Do poľa **Otvoriť** zadajte **príkaz regedit**a potom kliknite na **tlačidlo OK**.
     2. Ak sa zobrazí výzva na povolenie editora databázy Registry, vyberte možnosť **Yes (Áno** ), čím vykonáte zmeny v zariadení.
    3. V editore databázy Registry pridajte hodnotu DWORD EnableADAL s nastavením 0 podľa HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.
- Ak sa vyskytne chyba pri pripájaní k Office 365 pomocou Office 2013, [Povoliť moderné overovanie](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) pre klienta Office.

Ďalšie informácie nájdete v téme [Riešenie problémov s aplikáciami, ktoré nie sú prehľadávačom, ktoré sa nedajú prihlásiť do balíka Office 365, Azure alebo Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).


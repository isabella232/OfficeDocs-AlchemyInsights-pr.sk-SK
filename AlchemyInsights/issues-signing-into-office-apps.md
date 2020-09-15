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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695194"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Oprava aplikácií Microsoft 365 "Trusted Platform Module počítača nefunguje správne" správa

Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:

- Nainštalujte si najnovšie aktualizácie pre [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Vymazanie poverení balíka Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br/>
    **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Vyskúšajte [proces obnovenia používateľa](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) na opravu zlyhaní modulu TPM (Trusted Platform Module).
- Nastavte Povoliťadal = 0 pomocou týchto krokov:  
    1. Kliknite pravým tlačidlom myši na tlačidlo Štart systému Windows, vyberte položku **Spustiť**, zadajte **príkaz regedit**a potom kliknite na **tlačidlo OK**.
    2. Vyberte možnosť **Áno** , ak chcete povoliť Editor databázy Registry vykonávať zmeny v zariadení.
    3. V editore databázy Registry pridajte hodnotu DWORD **povoliťadal** s nastavením **0** v časti HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.

Ďalšie informácie nájdete v téme [problémy s pripojením pri prihlasovaní po aktualizácii na Office 2016 build 16.0.7967 vo Windowse 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
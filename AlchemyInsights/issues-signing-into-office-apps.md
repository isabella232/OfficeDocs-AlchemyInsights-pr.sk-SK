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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579880"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Oprava správy microsoft 365 aplikácie "Modul dôveryhodnej platformy počítača nefunguje správne"

Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:

- Nainštalujte najnovšie aktualizácie pre [systém Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Vymažte poverenia balíka Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou správcu poverení systému Windows.<br/>
    **Upozornenie:** Cesty databázy registry pre Office 2016 sa zmenili na 16.0. (Napr.: \Software\Microsoft\Office\16.0\Common\Identity\)
- Skúste [proces obnovenia používateľa](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) opraviť zlyhania modulu TPM (Trusted Platform Module).
- Nastavte EnableADAL = 0 pomocou nasledujúcich krokov:  
    1. Kliknite pravým tlačidlom myši na tlačidlo Štart systému Windows, vyberte položku **Spustiť**, zadajte **príkaz regedit**a potom vyberte tlačidlo **OK**.
    2. Ak chcete, aby Editor databázy Registry mohol vykonávať zmeny v zariadení, vyberte možnosť **Áno.**
    3. V Editore databázy Registry pridajte hodnotu DWORD **EnableADAL** s nastavením **0** v HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Ďalšie informácie nájdete v téme [Problémy s pripojením pri prihlasovaní po aktualizácii office 2016 stavať 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
---
title: Problémy s prihlásením do aplikácie balíka Office
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
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938336"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Stanovenie Office apps "Trusted Platform module počítača nepracuje správne" správy

Opraviť túto chybu, skúste nasledujúce:

- Nainštalujte najnovšie aktualizácie pre [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- [Jasné úradu poverení](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou poverení správcu systému Windows.<br/>
    **Poznámka:** Cesty databázy registry Office 2016 zmenili 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Skúste [používateľa ozdravný proces](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) opraviť zlyhania Trusted Platform Module (TPM).
- Nastaviť EnableADAL = 0 pomocou nasledujúcich krokov:  
    1. Kliknite pravým tlačidlom myši na tlačidlo Štart, vyberte **Spustiť**, zadajte **príkaz regedit**a potom kliknite na **tlačidlo OK**.
    2. Vyberte **Áno** povoliť Editor databázy Registry zmeny do vášho zariadenia.
    3. V editore databázy Registry pridajte hodnotu DWORD **EnableADAL** s nastavením **0** pod HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Ďalšie informácie nájdete v téme [pripojenie problémy v sign-in po aktualizácii Office 2016 build 16.0.7967 v systéme Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
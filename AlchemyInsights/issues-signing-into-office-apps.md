---
title: Problémy pri prihlasovaní do aplikácií Microsoft 365
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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833030"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>Hlásenie o oprave aplikácií služby Microsoft 365 "Modul dôveryhodnej platformy vášho počítača nefunkčný správne"

Ak chcete vyriešiť túto chybu, vyskúšajte nasledovný postup:

- Nainštalujte najnovšie aktualizácie pre [Windows a](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- [Odstráňte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br/>
    **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na hodnotu 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)
- Skúste v [procese obnovenia používateľa](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) opraviť zlyhanie Trusted Platform Module (TPM).
- Nastavte položku EnableADAL = 0 pomocou týchto krokov:  
    1. Kliknite pravým tlačidlom myši na tlačidlo Štart vo Windowse, vyberte **položku Spustiť**, zadajte **príkaz regedit** a potom vyberte tlačidlo **OK.**
    2. Ak **chcete editoru** databázy Registry povoliť vykonávať zmeny v zariadení, vyberte možnosť Áno.
    3. V Editore databázy Registry pridajte hodnotu DWORD **položky EnableADAL** s nastavením **0 v** časti HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.

Ďalšie informácie nájdete v téme Problémy s pripojením pri prihlasovaní po aktualizácii na [zostavu 16.0.7967 balíka Office 2016 vo Windowse 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
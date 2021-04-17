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
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833054"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prázdna prihlasovacia obrazovka v aplikáciách Microsoft 365

Ak chcete tento problém vyriešiť, vyskúšajte tento postup:
- Nainštalujte najnovšie aktualizácie pre [Windows a](https://support.microsoft.com/help/4027667/windows-10-update) [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Obnovenie možností programu Internet Explorer: Prejdite na položku Nástroje – možnosti siete Internet – rozšírené obnovenie výrobných nastavení  >    >    >  **programu Internet Explorer** (upozorňujeme, že stratíte vlastné nastavenia) a potom sa znova prihláste do balíka Office.
- Zakážte Windows Defender Application Guard (WDAG) alebo podobný firewall či antivírusový program:
    1. V ovládacom paneli prejdite na **položku Programy** a potom vyberte položku Zapnúť alebo vypnúť funkcie **systému Windows.**
    2. Ak je funkcia Windows Defender Application Guard zapnutá, skúste ju vypnúť.<br/>
    **Poznámka:** Je možné, že budete musieť reštartovať počítač.
- Skontrolujte, či doplnok Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie je blokovaný aplikáciou, bránou firewall/antivírusovým programom.
- [Odstráňte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br/>
    **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na hodnotu 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Ďalšie informácie nájdete v téme Problémy s pripojením pri prihlasovaní po aktualizácii na [zostavu 16.0.7967 balíka Office 2016 vo Windowse 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
---
title: Problémy pri prihlasovaní do Microsoft 365 aplikácií
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
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088051"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prázdna prihlasovacia obrazovka v Microsoft 365 aplikáciách

Ak chcete tento problém vyriešiť, vyskúšajte tento postup:
- Nainštalujte si najnovšie aktualizácie [pre Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)
- Obnovenie možností programu Internet Explorer: Prejdite na položku Nástroje Možnosti siete Internet – rozšírené obnovenie výrobných nastavení internet explorera Nastavenia (upozorňujeme, že stratíte vlastné nastavenia) a potom sa znova  >    >    >   prihláste Office internetového pripojenia.
- Vypnite Windows Defender Application Guard (WDAG) alebo podobný firewall či antivírusový program:
    1. V ovládacom paneli prejdite na **položku Programy** a potom vyberte položku Windows zapnúť alebo vypnúť **funkcie doplnku**.
    2. Ak Windows Defender Application Guard možnosť zapnutá, skúste ju vypnúť.<br/>
    **Poznámka:** Je možné, že budete musieť reštartovať počítač.
- Skontrolujte, či doplnok Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie je blokovaný aplikáciou, bránou firewall/antivírusovým programom.
- [Zrušte začiarknutie Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Windows Správca poverení.<br/>
    **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na hodnotu 16.0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Ďalšie informácie nájdete v téme Problémy s pripojením pri prihlasovaní po aktualizácii na [Office 2016, zostava 16.0.7967 v Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
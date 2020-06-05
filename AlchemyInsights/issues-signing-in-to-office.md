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
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579916"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prázdna prihlasovacia obrazovka v aplikáciách Microsoft 365

Ak chcete vyriešiť tento problém, vyskúšajte nasledujúci postup:
- Nainštalujte najnovšie aktualizácie pre [systém Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Obnovenie možností programu Internet Explorer: Prejdite na **položku Nástroje**  >  **Internet Options**  >  **Advanced**  >  **rozšíreného nastavenia programu Internet Explorer** (všimnite si, že stratíte vlastné nastavenia) a potom sa znova pokúste prihlásiť do balíka Office.
- Vypnite windows Defender Application Guard (WDAG) alebo akékoľvek podobné firewall alebo anti-virus program:
    1. V ovládacom paneli prejdite do **ponuky Programs (Programy)** a potom vyberte položku **Turn Windows features on /off (Zapnúť alebo vypnúť súčasti systému Windows**).
    2. Ak je zapnutá funkcia Windows Defender Application Guard, skúste ju vypnúť.<br/>
    **Upozornenie:** Možno bude potrebné reštartovať počítač.
- Uistite sa, že Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie je blokovaný žiadne aplikácie alebo firewall/anti-virus program.
- [Vymažte poverenia balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou správcu poverení systému Windows.<br/>
    **Upozornenie:** Cesty databázy registry pre Office 2016 sa zmenili na 16.0. (Napr.: \Software\Microsoft\Office\16.0\Common\Identity\)

Ďalšie informácie nájdete v téme [Problémy s pripojením pri prihlasovaní po aktualizácii office 2016 stavať 16.0.7967 Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
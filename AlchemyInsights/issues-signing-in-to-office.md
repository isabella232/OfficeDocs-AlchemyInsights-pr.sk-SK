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
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695302"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Prázdna prihlasovacia obrazovka v aplikáciách Microsoft 365

Ak chcete tento problém vyriešiť, vyskúšajte tento postup:
- Nainštalujte si najnovšie aktualizácie pre [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Obnovenie možností programu Internet Explorer: prechod na položku **Nástroje**  >  **internetu**–  >  **Rozšírené**  >  **Obnovenie nastavení programu Internet Explorer** (Všimnite si, že stratíte vlastné nastavenia) a potom sa znova skúste prihlásiť do balíka Office.
- Vypnite funkciu Windows Defender Application Guard (WDAG) alebo podobnú bránu firewall alebo program na ochranu pred vírusmi:
    1. V ovládacom paneli prejdite na položku **programy**a potom vyberte položku **Zapnúť alebo vypnúť súčasti systému Windows**.
    2. Ak je zapnutá ochrana aplikácií Windows Defender, skúste ju vypnúť.<br/>
    **Poznámka:** Možno bude potrebné reštartovať počítač.
- Uistite sa, že doplnok Microsoft. AAD. BrokerPlugin [AAD](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) nie je blokovaný žiadnou aplikáciou alebo bránou firewall alebo programom na ochranu pred vírusmi.
- [Vymazanie poverení balíka Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou Správcu poverení systému Windows.<br/>
    **Poznámka:** Cesty databázy Registry pre Office 2016 sa zmenili na 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Ďalšie informácie nájdete v téme [problémy s pripojením pri prihlasovaní po aktualizácii na Office 2016 build 16.0.7967 vo Windowse 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
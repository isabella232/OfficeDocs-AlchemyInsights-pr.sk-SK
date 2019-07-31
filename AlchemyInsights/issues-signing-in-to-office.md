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
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938335"
---
# <a name="blank-sign-in-screen-in-office-apps"></a>Prázdne prihlasovacej obrazovky v aplikáciách balíka Office

Ak chcete vyriešiť tento problém, skúste nasledovné:
- Nainštalujte najnovšie aktualizácie pre [Windows](https://support.microsoft.com/help/4027667/windows-10-update) a [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).
- Vynulovanie nastavení programu Internet Explorer: Prejdite na **Nástroje** > **Možnosti siete Internet** > **Rozšírené** > **Internet Explorer – obnovenie pôvodného nastavenia** (Všimnite si, že stratíte vlastné nastavenia) a potom sa pokúste znova prihlásiť do kancelárie.
- Zakázať Windows Defender aplikácie stráž (WDAG) alebo akýkoľvek podobný firewall alebo anti-virus program:
    1. V ovládacom paneli, prejdite na položku **programy**a potom vyberte **alebo vypnúť súčasti systému Windows**.
    2. Ak je zapnutý Windows Defender aplikačného ochrancu, skúste ju vypnúť.<br/>
    **Poznámka:** Budete musieť reštartovať počítač.
- Uistite sa, že Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) je neblokuje žiadne aplikácie alebo firewall/anti-anti-virus program.
- [Jasné úradu poverení](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomocou poverení správcu systému Windows.<br/>
    **Poznámka:** Cesty databázy registry Office 2016 zmenili 16,0. (Ex: \Software\Microsoft\Office\16.0\Common\Identity\)

Ďalšie informácie nájdete v téme [pripojenie problémy v sign-in po aktualizácii Office 2016 build 16.0.7967 v systéme Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).
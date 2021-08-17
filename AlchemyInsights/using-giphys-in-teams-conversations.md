---
title: Používanie giphy v Teams konverzáciách
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104323"
---
# <a name="using-giphys-in-teams-conversations"></a>Používanie giphy v Teams konverzáciách

Giphys access in Teams chat is enabled by default. Ako správca môžete kontrolovať, či sú giphy k dispozícii používateľom, [nastavením](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) politiky výmeny správ a zabezpečením, že možnosť Používať **giphy v konverzáciách je** má byť **.**

Ak súbory GIF v konverzáciách vo formáte GIF Teams podľa očakávaní, overte, či:

Politika [odosielania správ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) musí umožniť giphy. Overenie pomocou rutín typu cmdlet prostredia PowerShell:

- Overte, či môžete [spravovať Teams pomocou prostredia PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Spustite príkaz prostredia PowerShell [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) a overte, či je možnosť **AllowGiphy** nastavená na hodnotu **TRUE.**
- Ak je možnosť **AllowGiphy** nastavená na **hodnotu FALSE,** spustite nasledujúci príkaz prostredia PowerShell [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Voliteľné pripojené funkcie musia](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) byť povolené, aby ste povolili prístup k URL adrese giphy.

> [!NOTE]
> Ak máte pre nájomníka nakonfigurované viaceré politiky výmeny správ Teams, môžete zistiť identitu politiky priradenú používateľovi s vplyvom na príkaz prostredia PowerShell [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Vyberte položku TeamsMessagingPolicy.

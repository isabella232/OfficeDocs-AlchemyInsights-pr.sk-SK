---
title: Používanie Giphy v konverzáciách v aplikácii teams
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
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982578"
---
# <a name="using-giphys-in-teams-conversations"></a>Používanie Giphy v konverzáciách v aplikácii teams

Giphy Access v aplikácii teams chat je predvolene zapnutý. Ako správca môžete ovládať, či sú Giphy k dispozícii pre používateľov [nastavením politiky odosielania správ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) a zabezpečte, aby bolo **zapnuté** **Používanie giphy v konverzáciách** .

Ak GIF nefungujú podľa očakávaní v konverzáciách v aplikácii Teams, overte:

[Politika odosielania správ](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) musí povoľovať giphy. Overenie pomocou rutiny typu cmdlet prostredia PowerShell:

- Overte, či môžete [Spravovať tímy s prostredím PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Spustite príkaz prostredia PowerShell [Get-CsTeamsMessagingPolicy-identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) a overte, či je **AllowGiphy** nastavený na **hodnotu True**.
- Ak je **AllowGiphy** nastavený na **hodnotu False** , spustite nasledujúci príkaz v prostredí PowerShell – [CsTeamsMessagingPolicy-identity Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Voliteľné pripojené](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) funkcie je potrebné povoliť na umožnenie prístupu k URL adrese Giphy.

> [!NOTE]
> Ak máte v nájomníkovi nakonfigurované viaceré politiky na výmenu správ, môžete určiť identitu politiky priradenej k ovplyvnenému používateľovi s príkazom prostredia PowerShell [Get-CsOnlineUser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Vyberte položku TeamsMessagingPolicy.

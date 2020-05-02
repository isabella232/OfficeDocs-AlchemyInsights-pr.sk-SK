---
title: Súkromný kanál
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001223"
- "3205"
ms.openlocfilehash: be518df0d40123c1f0da6596bd6e2e91a0c2c8fa
ms.sourcegitcommit: 057d87c9d866fa1371d02350420d13774545c028
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/02/2020
ms.locfileid: "44005453"
---
# <a name="private-channels-in-microsoft-teams"></a>Súkromné kanály v Microsoft teams

Súkromné kanály sú novou funkciou v Microsoft teams. Upozorňujeme, že súkromné kanály nemožno konvertovať zo štandardných kanálov ani naopak.

Podrobnosti o súkromných kanáloch, ako sú napríklad informácie o [vytváraní privátneho kanála a o členstve](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-creation-and-membership) a [súkromných kanáloch lokality SharePoint](https://docs.microsoft.com/MicrosoftTeams/private-channels#private-channel-sharepoint-sites), nájdete [v téme súkromné kanály v Microsoft teams](https://docs.microsoft.com/MicrosoftTeams/private-channels). 

**Poznámka:** Keďže Konfigurácia uchovávania súkromných správ kanála ešte nie je podporovaná, nájomníci s povolenými politikami uchovávania údajov nebudú mať predvolene povolené súkromné kanály. Súkromné kanály môžu byť povolené v tíme admin Center. Všimnite si tiež, že zatiaľ čo uchovávanie súkromných kanálov správ nie je podporovaný, je podporovaný uchovávanie súborov zdieľaných v súkromných kanáloch.

**Potrebujete nového vlastníka tímu?**

Ak váš súkromný kanál vlastník opustí, môžete pridať nového vlastníka tímu cez tímy PowerShell.


- Choď [sem](https://www.powershellgallery.com/packages/MicrosoftTeams/1.0.6) nainštalovať tímy PowerShell.

Tu je rutina cmdlet budete potrebovať:

`
    Add-TeamChannelUser -GroupId <group_id> -DisplayName "<channel_name>" -User <UPN> -Role Owner
`

Ďalšie informácie o tímových PowerShell, pozri [tímy PowerShell prehľad](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).

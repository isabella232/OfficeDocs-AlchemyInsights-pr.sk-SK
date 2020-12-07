---
title: Čo robiť, ak funkcie Azure v prehliadači Microsoft Edge nefungujú správne
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583783"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Čo robiť, ak funkcie Azure v prehliadači Microsoft Edge nefungujú správne

Microsoft Edge obsahuje [známe problémy](https://go.microsoft.com/fwlink/?linkid=2140608) týkajúce sa zón zabezpečenia a môže ovplyvniť spôsob prihlasovania používateľov služby Azure do centra spravovania pre Windows. Ak máte problémy s používaním funkcií Azure v prehliadači Microsoft Edge, vyskúšajte tieto kroky:

1. V ponuke **Štart** vyhľadajte položku **Možnosti siete Internet** a vyberte ju.
2. V dialógovom okne **Vlastnosti siete Internet** prejdite na kartu **zabezpečenie** .
3. Vyberte zónu **Dôveryhodné lokality** a potom kliknite na tlačidlo **lokality** .
4. V dialógovom okne **Dôveryhodné lokality** pridajte URL adresu brány, ako aj [https://login.microsoftonline.com](https://login.microsoftonline.com) a [https://login.live.com](https://login.live.com) potom vyberte položku **zatvorenie**.
5. V dialógovom okne **Vlastnosti siete Internet** prejdite na kartu **Ochrana osobných údajov** .
6. V časti **Blokovanie automaticky otváraných okien** vyberte položku **nastavenia**. V dialógovom okne, ktoré sa otvorí, pridajte URL adresu brány, ako aj [https://login.microsoftonline.com](https://login.microsoftonline.com) a [https://login.live.com](https://login.live.com) potom vyberte položku **zatvorenie**.

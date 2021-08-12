---
title: Čo robiť, ak funkcie služby Azure v službe Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812878"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Čo robiť, ak funkcie služby Azure v službe Microsoft Edge

Microsoft Edge sa známe problémy týkajúce sa zón zabezpečenia, ktoré môžu ovplyvniť spôsob, akým sa používatelia služby Azure prihlasovať Windows spravovania. Ďalšie informácie nájdete v téme Známe [problémy v Edgei.](https://go.microsoft.com/fwlink/?linkid=2140608) Ak máte problémy s používaním funkcií platformy Azure so Microsoft Edge, vyskúšajte tento postup:

1. Na paneli ponuka Štart zadajte **do** vyhľadávacieho panela **položku Možnosti siete internet** a vyberte ju.
1. V **časti Vlastnosti** siete Internet vyberte **kartu** Zabezpečenie.
1. Vyberte **položku Dôveryhodné lokality** a potom vyberte položku **Lokality**.
1. Pridajte URL adresu brány aj a <https://login.microsoftonline.com> a vyberte položku <https://login.live.com> **Zavrieť**.
1. V **časti Vlastnosti** internetu vyberte kartu Ochrana **osobných** údajov.
1. V časti Blokovanie automaticky otváraných okien vyberte položku **Nastavenia.** Pridajte URL adresu brány aj a <https://login.microsoftonline.com> potom vyberte položku <https://login.live.com> **Zavrieť**.
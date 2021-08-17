---
title: Čo robiť, ak funkcie služby Azure v službe Microsoft Edge
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
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117103"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>Čo robiť, ak funkcie služby Azure v službe Microsoft Edge

Microsoft Edge má [známe problémy súvisiace](https://go.microsoft.com/fwlink/?linkid=2140608) so zónami zabezpečenia a môže ovplyvniť spôsob, akým sa používatelia služby Azure prihlásia Windows spravovania služieb. Ak máte problémy s používaním funkcií platformy Azure so Microsoft Edge, vyskúšajte tieto kroky:

1. V ponuke **Štart** vyhľadajte položku **Možnosti siete Internet a** vyberte ju.
2. V **dialógovom** okne Internetové vlastnosti prejdite na **kartu** Zabezpečenie.
3. Vyberte **zónu Dôveryhodné** lokality a potom vyberte **tlačidlo** Lokality.
4. V **dialógovom okne** Dôveryhodné lokality pridajte AJ URL adresu brány a [https://login.microsoftonline.com](https://login.microsoftonline.com) potom vyberte položku [https://login.live.com](https://login.live.com) **Zavrieť**.
5. V **dialógovom okne** Internetové vlastnosti prejdite na kartu **Ochrana osobných** údajov.
6. V časti **Blokovanie automaticky otváraných** okien vyberte položku **Nastavenia**. V dialógovom okne, ktoré sa otvorí, pridajte aj URL adresu brány [https://login.microsoftonline.com](https://login.microsoftonline.com) a potom vyberte položku [https://login.live.com](https://login.live.com) **Zavrieť**.

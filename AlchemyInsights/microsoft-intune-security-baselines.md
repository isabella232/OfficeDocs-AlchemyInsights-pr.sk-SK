---
title: Konfigurácia Microsoft Intune zabezpečenia pomocou pôvodných Windows 10 zabezpečenia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794132"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfigurácia Microsoft Intune zabezpečenia pomocou pôvodných Windows 10 zabezpečenia

Základné hodnoty zabezpečenia služby Intune pomáhajú chrániť používateľov a zariadenia. Pôvodné hodnoty zabezpečenia Windows predkonfigurované skupiny používané na použitie známej skupiny nastavení a predvolených hodnôt odporúčaných príslušnými tímami zabezpečenia. Vytvorením profilu pôvodného plánu zabezpečenia v programe Intune vytvoríte šablónu, ktorá sa skladá z viacerých profilov konfigurácie zariadení.

Keď nasadzujete pôvodné hodnoty zabezpečenia skupinám používateľov alebo zariadení, nastavenia sa použijú na zariadenia, ktoré sú Windows 10 novšej verzie. Pôvodný plán zabezpečenia správy mobilných zariadení Microsoft (MDM) napríklad automaticky zapne šifrovanie BitLocker vymeniteľné jednotky, vyžaduje heslo na odomknutie zariadenia a vypne základné overovanie. Ak predvolená hodnota vo vašom prostredí nefunguje, môžete prispôsobiť pôvodný plán a použiť potrebné nastavenia.

Pôvodné hodnoty zabezpečenia tiež pomáhajú vytvoriť end-to-end secure workflow v Microsoft 365. Základná hodnota zabezpečenia obsahuje osvedčené postupy a odporúčania pre nastavenia, ktoré majú vplyv na zabezpečenie. Partneri Intune s tímom zabezpečenia Windows, ktorý vytvára pôvodné hodnoty pre skupinové politiky, takže tieto odporúčania vychádzajú z rozsiahlych pokynov a rozsiahlej skúsenosti.

Ak so služby Intune iba začínate a nie ste si istí, kde začať, základné hodnoty zabezpečenia vám pomôžu rýchlo vytvoriť a nasadiť zabezpečený profil. Ak momentálne používate skupinovú politiku, migrácia do služby Intune na účely správy je s pôvodnými plánmi zabezpečenia omnoho jednoduchšia, pretože sú zabudované do služby Intune a zahŕňajú špičkové možnosti správy.

Ďalšie informácie nájdete v téme Windows [zabezpečenia a správa](/windows/security/threat-protection/windows-security-baselines) [mobilných zariadení.](/windows/client-management/mdm/)


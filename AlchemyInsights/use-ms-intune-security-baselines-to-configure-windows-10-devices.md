---
title: Konfigurácia Microsoft Intune zabezpečenia pomocou pôvodných Windows 10 zabezpečenia
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104359"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Konfigurácia Microsoft Intune zabezpečenia pomocou pôvodných Windows 10 zabezpečenia

Základné hodnoty zabezpečenia služby Intune pomáhajú chrániť používateľov a zariadenia. Pôvodné hodnoty zabezpečenia Windows predkonfigurované skupiny nastavení na použitie známej skupiny nastavení a predvolených hodnôt odporúčaných príslušnými tímami zabezpečenia. Vytvorením profilu pôvodného plánu zabezpečenia v programe Intune vytvoríte šablónu, ktorá sa skladá z viacerých profilov konfigurácie zariadení.

Keď nasadzujete pôvodné hodnoty zabezpečenia skupinám používateľov alebo zariadení, nastavenia sa použijú na zariadenia, ktoré sú Windows 10 novšej verzie. Pôvodný plán zabezpečenia MDM automaticky (1) napríklad umožňuje šifrovanie BitLocker pre vymeniteľné jednotky, (2) vyžaduje heslo na odomknutie zariadenia a (3) vypne základné overovanie. Ak predvolená hodnota pre vaše prostredie nefunguje, prispôsobte pôvodný plán a použite potrebné nastavenia.

Pôvodné hodnoty zabezpečenia tiež pomáhajú vytvoriť end-to-end secure workflow v Microsoft 365. Prinášame vám niekoľko výhod:

- Základná hodnota zabezpečenia obsahuje osvedčené postupy a odporúčania pre nastavenia, ktoré majú vplyv na zabezpečenie. Keďže partneri spoločnosti Intune s tímom zabezpečenia spoločnosti Windows, ktorí vytvárajú pôvodné hodnoty pre skupinové politiky, tieto odporúčania vychádzajú z rozsiahlych pokynov a rozsiahlej skúsenosti.
- Ak so služby Intune iba začínate a nie ste si istí, kde začať, pôvodné hodnoty zabezpečenia vám pomôžu rýchlo vytvoriť a nasadiť zabezpečený profil.
- Ak v súčasnosti používate skupinovú politiku, migrácia do služby Intune na účely správy je s pôvodnými plánmi zabezpečenia omnoho jednoduchšia, pretože sú zabudované do služby Intune a zahŕňajú špičkové možnosti správy.

Ďalšie informácie nájdete v téme Windows [zabezpečenia a správa](https://go.microsoft.com/fwlink/?linkid=2141503) [mobilných zariadení.](https://go.microsoft.com/fwlink/?linkid=2141701)
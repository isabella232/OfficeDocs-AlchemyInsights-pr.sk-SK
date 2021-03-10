---
title: Použitie pôvodných plánov zabezpečenia služby Microsoft Intune na konfiguráciu zariadení s Windowsom 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696381"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Použitie základných čiar zabezpečenia služby Microsoft Intune na konfigurovanie zariadení s Windowsom 10

Základné údaje zabezpečenia služby Intune pomáhajú chrániť používateľov a zariadenia. Základné údaje zabezpečenia sú predkonfigurované skupiny nastavení Windowsu, ktoré sa používajú na použitie známej skupiny nastavení a predvolených hodnôt odporúčaných príslušnými tímami zabezpečenia. Vytvorením základného profilu zabezpečenia v službe Intune vytvoríte šablónu, ktorá sa skladá z viacerých profilov konfigurácie zariadenia.

Keď nasadíte základné údaje zabezpečenia do skupín používateľov alebo zariadení, nastavenia sa použijú na zariadenia spustené vo Windowse 10 alebo novších verziách. Napríklad automatické vytvorenie pôvodného plánu Microsoft Mobile Device Management (MDM) (1) zapne funkciu BitLocker for vymeniteľných jednotiek, (2) vyžaduje heslo na odomknutie zariadenia a (3) zakáže základné overovanie. Ak predvolená hodnota v prostredí nie je funkčná, môžete prispôsobiť základnú čiaru tak, aby používala požadované nastavenia.

Základné informácie o zabezpečení tiež pomáhajú pri vytváraní pracovného postupu koncového zabezpečenia v programe Microsoft 365. Nižšie sú uvedené niektoré výhody tejto funkcie:
- Základná hodnota zabezpečenia obsahuje najvhodnejšie postupy a odporúčania pre nastavenia, ktoré majú vplyv na zabezpečenie. Keďže partneri služby Intune s tímom zabezpečenia systému Windows, ktorý vytvára základné hodnoty pre politiky skupiny, sú tieto odporúčania založené na solídnom poradenstve a rozsiahlych skúsenostiach.
- Ak sa v službe Intune nachádzate a neviete, kde začať, základné informácie o zabezpečení vám pomôžu rýchlo vytvoriť a nasadiť zabezpečený profil.
- Ak v súčasnosti používate skupinovú politiku, migrácia do služby Intune na účely správy je oveľa jednoduchšia s pôvodnými bezpečnostnými hodnotami, pretože tieto základné prvky zabezpečenia sú vstavané do služby Intune a obsahujú najmodernejšie možnosti spravovania.

Ďalšie informácie nájdete v téme [základné informácie o zabezpečení systému Windows](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) a [Správa mobilných zariadení](https://docs.microsoft.com/windows/client-management/mdm/).
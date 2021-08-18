---
title: Riešenie problémov s inštaláciou MDATP v Macu
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091077"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Riešenie problémov s inštaláciou MDATP v Macu

Ak manuálna inštalácia zlyhá, **na stránke** Súhrn sprievodcu inštaláciou sa zobrazí nasledujúca chyba:

Počas inštalácie sa vyskytla chyba. Inštalátor zistil chybu, ktorá spôsobila zlyhanie inštalácie. Požiadajte o pomoc výrobcu softvéru.

V prípade nasadení MDM sa na stránke zobrazuje aj všeobecné zlyhanie inštalácie.

Napriek tomu, že pre koncových používateľov nezobrazujeme presné chyby, v **/Library/Logs/Microsoft/mdatp/install.log** sa uchová súbor denníka s priebehom inštalácie. Každá relácia inštalácie sa pripojí k tomuto súboru denníka. Ak chcete vytvoriť výstup iba poslednej relácie inštalácie, použite `sed` .

Ďalšie informácie nájdete v téme Riešenie [problémov s inštaláciou aplikácie Microsoft Defender ATP pre Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)

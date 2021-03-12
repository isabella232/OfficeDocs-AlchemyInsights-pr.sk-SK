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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749769"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>Riešenie problémov s inštaláciou MDATP v Macu

Ak manuálna inštalácia zlyhá, **súhrnná** stránka Sprievodcu inštaláciou zobrazí sa nasledujúca chyba:

Počas inštalácie sa vyskytla chyba. Inštalátor zistil chybu, ktorá spôsobila zlyhanie inštalácie. Požiadajte o pomoc výrobcu softvéru.

Pri nasadení MDM sa na stránke zobrazuje zlyhanie všeobecného inštalácie.

Hoci sa na koncových používateľov nezobrazujú presné chyby, v **/Library/logs/Microsoft/mdatp/Install.log** sa uchová súbor denníka s priebehom inštalácie. Každá relácia inštalácie sa pridá do tohto súboru denníka. Ak chcete použiť len poslednú reláciu inštalácie, použite `sed` .

Ďalšie informácie nájdete v téme [Riešenie problémov s inštaláciou programu Microsoft Defender ATP pre Mac](https://go.microsoft.com/fwlink/?linkid=2144615).

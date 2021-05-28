---
title: Nahrávanie hovoru 1:1
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696973"
---
# <a name="11-call-recording"></a>Nahrávanie hovoru 1:1

Ak je **tlačidlo Spustiť** nahrávanie neaktívne počas hovoru s 1:1, je potrebné zmeniť nastavenie politiky pre o vplyve používateľa.   

Od 31. mája 2021 začneme vynucovať novú politiku Teams *volanie AllowCloudRecordingForCalls.* Pred touto zmenou sa nahrávanie hovoru vo forme 1:1 riadi politikou *schôdze AllowCloudRecording* Teams schôdze. Táto zmena je zdokumentovaná v príspevku v Centre správ: [(Aktualizované) 1:1 Úvod do politiky nahrávania hovoru.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   politika volanie je predvolene **nastavená $False** na možnosť Vypnuté. Ak chcete všetkým používateľom zablokovať nahrávanie hovorov vo veľkosť 1 :1, nemusíte urobiť nič.  

Ak chcete zapnúť nahrávanie hovorov pre všetkých používateľov vo hovoroch vo Teams 1:1, pomocou prostredia PowerShell spustite túto rutinu cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Prípadne môžete vytvoriť novú politiku a nastaviť **nastavenie -AllowCloudRecordingForCalls** **na $true** a priradiť túto politiku používateľom. 

Ďalšie informácie nájdete v téme [1:1 Ovládacie prvky politiky nahrávania hovoru sú (takmer!) Tu .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)

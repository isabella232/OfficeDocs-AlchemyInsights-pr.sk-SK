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
ms.openlocfilehash: 29383643e6867bca7fd31774a9594b82fdc080bb0e7254141e8c883ad861075e
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886154"
---
# <a name="11-call-recording"></a>Nahrávanie hovoru 1:1

Ak je **tlačidlo Spustiť** nahrávanie neaktívne počas hovoru s 1:1, je potrebné zmeniť nastavenie politiky pre o vplyve používateľa. Ak chcete skontrolovať nastavenie politiky, spustite Diagnostiku pre o vplyv používateľa zadaním **Diag: Teams 1:1 Nahrávanie hovoru** vyššie.     

Od 31. mája 2021 začneme vynucovať novú politiku Teams *volanie AllowCloudRecordingForCalls.* Pred touto zmenou sa nahrávanie hovoru vo forme 1:1 riadi politikou *schôdzí AllowCloudRecording* Teams schôdze. Táto zmena je zdokumentovaná v príspevku v Centre správ: [(Aktualizované) 1:1 Úvod do politiky nahrávania hovoru.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)  

*AllowCloudRecordingForCalls*   politika volanie je predvolene **nastavená $False** na volanie. Ak chcete všetkým používateľom zablokovať nahrávanie hovorov vo veľkosť 1 :1, nemusíte urobiť nič.  

Ak chcete zapnúť nahrávanie hovorov pre všetkých používateľov vo hovoroch vo Teams 1:1, pomocou [prostredia PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install) spustite túto rutinu cmdlet: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Prípadne môžete vytvoriť novú politiku a nastaviť **nastavenie -AllowCloudRecordingForCalls** **na $true** a priradiť túto politiku používateľom. 

Ďalšie informácie nájdete v téme [1:1 Ovládacie prvky politiky nahrávania hovoru sú (takmer!) Tu .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)

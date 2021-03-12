---
title: nahrávanie hovoru cez 1:1
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733864"
---
# <a name="11-call-recording"></a>nahrávanie hovoru cez 1:1

Správcovia musia teraz konať, aby mohli používatelia nahrávať hovory 1:1.
 
Začiatok 12. apríla 2021, začneme vynútenie novej možnosti *AllowCloudRecordingForCalls* politiky pre teams. 

Možnosti nahrávania hovoru v súčasnosti 1:1 ovláda možnosť *AllowCloudRecording* v politikách schôdze v aplikácii teams. Ak majú používatelia povolené nahrávať schôdze v aplikácii Teams, môžu tiež nahrávať hovory 1:1.

Ak chcete blokovať všetkých používateľov, ktorí zaznamenávajú hovory 1:1, nemusíte vykonať žiadnu akciu. Možnosť *AllowCloudRecordingForCalls* Calling Policy sa predvolene $FALSE.

Táto zmena sa zdokumentuje v nasledujúcom príspevku centra správ: [(aktualizované) úvodné informácie o zavedení hovoru](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) v službe teams – 1:1 je nutné použiť [tímové prostredie PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Povolenie nahrávania hovorov v programe 1:1 hovory:** Set-CsTeamsCallingPolicy globálnych identít – AllowCloudRecordingForCalls $True

**Vypnutie nahrávania hovorov v programe 1:1 hovory:** Set-CsTeamsCallingPolicy – globálna identita – AllowCloudRecordingForCalls $FALSE


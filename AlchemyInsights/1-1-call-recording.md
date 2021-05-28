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
# <a name="11-call-recording"></a><span data-ttu-id="b0e1c-102">Nahrávanie hovoru 1:1</span><span class="sxs-lookup"><span data-stu-id="b0e1c-102">1:1 call recording</span></span>

<span data-ttu-id="b0e1c-103">Ak je **tlačidlo Spustiť** nahrávanie neaktívne počas hovoru s 1:1, je potrebné zmeniť nastavenie politiky pre o vplyve používateľa.</span><span class="sxs-lookup"><span data-stu-id="b0e1c-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="b0e1c-104">Od 31. mája 2021 začneme vynucovať novú politiku Teams *volanie AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="b0e1c-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="b0e1c-105">Pred touto zmenou sa nahrávanie hovoru vo forme 1:1 riadi politikou *schôdze AllowCloudRecording* Teams schôdze.</span><span class="sxs-lookup"><span data-stu-id="b0e1c-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="b0e1c-106">Táto zmena je zdokumentovaná v príspevku v Centre správ: [(Aktualizované) 1:1 Úvod do politiky nahrávania hovoru.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="b0e1c-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="b0e1c-107">*AllowCloudRecordingForCalls*   politika volanie je predvolene **nastavená $False** na možnosť Vypnuté.</span><span class="sxs-lookup"><span data-stu-id="b0e1c-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="b0e1c-108">Ak chcete všetkým používateľom zablokovať nahrávanie hovorov vo veľkosť 1 :1, nemusíte urobiť nič.</span><span class="sxs-lookup"><span data-stu-id="b0e1c-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="b0e1c-109">Ak chcete zapnúť nahrávanie hovorov pre všetkých používateľov vo hovoroch vo Teams 1:1, pomocou prostredia PowerShell spustite túto rutinu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="b0e1c-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="b0e1c-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="b0e1c-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="b0e1c-111">Prípadne môžete vytvoriť novú politiku a nastaviť **nastavenie -AllowCloudRecordingForCalls** **na $true** a priradiť túto politiku používateľom.</span><span class="sxs-lookup"><span data-stu-id="b0e1c-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="b0e1c-112">Ďalšie informácie nájdete v téme [1:1 Ovládacie prvky politiky nahrávania hovoru sú (takmer!) Tu .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)</span><span class="sxs-lookup"><span data-stu-id="b0e1c-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>

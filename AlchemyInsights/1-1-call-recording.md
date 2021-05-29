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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702105"
---
# <a name="11-call-recording"></a><span data-ttu-id="21d15-102">Nahrávanie hovoru 1:1</span><span class="sxs-lookup"><span data-stu-id="21d15-102">1:1 call recording</span></span>

<span data-ttu-id="21d15-103">Ak je **tlačidlo Spustiť** nahrávanie neaktívne počas hovoru s 1:1, je potrebné zmeniť nastavenie politiky pre o vplyve používateľa.</span><span class="sxs-lookup"><span data-stu-id="21d15-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span> <span data-ttu-id="21d15-104">Ak chcete skontrolovať nastavenie politiky, spustite Diagnostiku pre o vplyv používateľa zadaním **Diag: Teams 1:1 Nahrávanie hovoru** vyššie.</span><span class="sxs-lookup"><span data-stu-id="21d15-104">To check the policy setting, run the Diagnostic for the impacted user by typing **Diag: Teams 1:1 Call Recording** above.</span></span>     

<span data-ttu-id="21d15-105">Od 31. mája 2021 začneme vynucovať novú politiku Teams *volanie AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="21d15-105">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="21d15-106">Pred touto zmenou sa nahrávanie hovoru vo forme 1:1 riadi politikou *schôdze AllowCloudRecording* Teams schôdze.</span><span class="sxs-lookup"><span data-stu-id="21d15-106">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="21d15-107">Táto zmena je zdokumentovaná v príspevku v Centre správ: [(Aktualizované) 1:1 Úvod do politiky nahrávania hovoru.](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)</span><span class="sxs-lookup"><span data-stu-id="21d15-107">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="21d15-108">*AllowCloudRecordingForCalls*   politika volanie je predvolene **nastavená $False** na možnosť Vypnuté.</span><span class="sxs-lookup"><span data-stu-id="21d15-108">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="21d15-109">Ak chcete všetkým používateľom zablokovať nahrávanie hovorov vo veľkosť 1 :1, nemusíte urobiť nič.</span><span class="sxs-lookup"><span data-stu-id="21d15-109">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="21d15-110">Ak chcete zapnúť nahrávanie hovorov pre všetkých používateľov vo hovoroch vo Teams 1:1, [pomocou prostredia PowerShell](/microsoftteams/teams-powershell-install) spustite túto rutinu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="21d15-110">To enable call recording for all users in 1:1 calls use [Teams PowerShell](/microsoftteams/teams-powershell-install) to run the following cmdlet:</span></span> 

<span data-ttu-id="21d15-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="21d15-111">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="21d15-112">Prípadne môžete vytvoriť novú politiku a nastaviť **nastavenie -AllowCloudRecordingForCalls** **na $true** a priradiť túto politiku používateľom.</span><span class="sxs-lookup"><span data-stu-id="21d15-112">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="21d15-113">Ďalšie informácie nájdete v téme [1:1 Ovládacie prvky politiky nahrávania hovoru sú (takmer!) Tu .](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)</span><span class="sxs-lookup"><span data-stu-id="21d15-113">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>

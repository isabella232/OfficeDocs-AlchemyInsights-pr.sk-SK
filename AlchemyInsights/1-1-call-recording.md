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
# <a name="11-call-recording"></a><span data-ttu-id="f5eb0-102">nahrávanie hovoru cez 1:1</span><span class="sxs-lookup"><span data-stu-id="f5eb0-102">1:1 call recording</span></span>

<span data-ttu-id="f5eb0-103">Správcovia musia teraz konať, aby mohli používatelia nahrávať hovory 1:1.</span><span class="sxs-lookup"><span data-stu-id="f5eb0-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="f5eb0-104">Začiatok 12. apríla 2021, začneme vynútenie novej možnosti *AllowCloudRecordingForCalls* politiky pre teams.</span><span class="sxs-lookup"><span data-stu-id="f5eb0-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="f5eb0-105">Možnosti nahrávania hovoru v súčasnosti 1:1 ovláda možnosť *AllowCloudRecording* v politikách schôdze v aplikácii teams.</span><span class="sxs-lookup"><span data-stu-id="f5eb0-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="f5eb0-106">Ak majú používatelia povolené nahrávať schôdze v aplikácii Teams, môžu tiež nahrávať hovory 1:1.</span><span class="sxs-lookup"><span data-stu-id="f5eb0-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="f5eb0-107">Ak chcete blokovať všetkých používateľov, ktorí zaznamenávajú hovory 1:1, nemusíte vykonať žiadnu akciu.</span><span class="sxs-lookup"><span data-stu-id="f5eb0-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="f5eb0-108">Možnosť *AllowCloudRecordingForCalls* Calling Policy sa predvolene $FALSE.</span><span class="sxs-lookup"><span data-stu-id="f5eb0-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="f5eb0-109">Táto zmena sa zdokumentuje v nasledujúcom príspevku centra správ: [(aktualizované) úvodné informácie o zavedení hovoru](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) v službe teams – 1:1 je nutné použiť [tímové prostredie PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="f5eb0-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="f5eb0-110">**Povolenie nahrávania hovorov v programe 1:1 hovory:** Set-CsTeamsCallingPolicy globálnych identít – AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="f5eb0-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="f5eb0-111">**Vypnutie nahrávania hovorov v programe 1:1 hovory:** Set-CsTeamsCallingPolicy – globálna identita – AllowCloudRecordingForCalls $FALSE</span><span class="sxs-lookup"><span data-stu-id="f5eb0-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>


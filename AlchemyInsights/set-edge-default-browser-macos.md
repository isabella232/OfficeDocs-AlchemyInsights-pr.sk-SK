---
title: Nastavenie Microsoft Edgeu ako predvoleného prehliadača v zariadení so systémom macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491814"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="e405d-102">Nastavenie Microsoft Edgeu ako predvoleného prehliadača v zariadení so systémom macOS</span><span class="sxs-lookup"><span data-stu-id="e405d-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="e405d-103">Ak chcete nastaviť Microsoft Edge ako predvolený prehliadač, použite jeden z týchto dvoch spôsobov:</span><span class="sxs-lookup"><span data-stu-id="e405d-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="e405d-104">Metóda 1: Flash zariadenie s obrázkom macOS, kde Microsoft Edge už bol nastavený ako predvolený prehliadač.</span><span class="sxs-lookup"><span data-stu-id="e405d-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="e405d-105">Metóda 2: Nastavenie politiky DefaultBrowserSettingEnabled tak, aby sa používateľovi výzva na nastavenie prehliadača Microsoft Edge ako predvoleného prehliadača.</span><span class="sxs-lookup"><span data-stu-id="e405d-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="e405d-106">Ktorá z týchto metód umožňuje používateľovi zmeniť predvolený prehliadač.</span><span class="sxs-lookup"><span data-stu-id="e405d-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="e405d-107">Z tohto dôvodu odporúčame nasadiť politiku DefaultBrowserSettingEnabled aj vtedy, ak ste použili metódu 1.</span><span class="sxs-lookup"><span data-stu-id="e405d-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="e405d-108">Ak používateľ po nasadení politiky zmení predvolený prehliadač, zobrazí sa výzva na nastavenie predvoleného prehliadača späť na Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="e405d-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>

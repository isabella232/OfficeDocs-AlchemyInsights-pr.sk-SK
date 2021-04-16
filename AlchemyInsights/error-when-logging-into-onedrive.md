---
title: 0x8004de40 pri spúšťaní OneDrivu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813667"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="b554a-102">0x8004de40 pri spúšťaní OneDrivu</span><span class="sxs-lookup"><span data-stu-id="b554a-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="b554a-103">Ak sa pri prihlasovaní **do 0x8004de40** OneDrive zobrazí chybové hlásenie, reštartujte počítač po pripojení k pracovnej alebo školskej doméne.</span><span class="sxs-lookup"><span data-stu-id="b554a-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="b554a-104">Ak sa táto chyba zobrazí po reštartovaní, skúste to po pripojení k pracovnej alebo školskej doméne:</span><span class="sxs-lookup"><span data-stu-id="b554a-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="b554a-105">Kliknite na tlačidlo Štart a zadajte **výraz cmd** alebo **príkazový** riadok do vyhľadávacieho poľa, kliknite pravým tlačidlom myši na aplikáciu príkazového riadka a vyberte položku **Spustiť ako správca.**</span><span class="sxs-lookup"><span data-stu-id="b554a-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="b554a-106">Ak sa zobrazí výzva na zadanie hesla správcu alebo potvrdenie, zadajte heslo alebo kliknite na položku **Povoliť**.</span><span class="sxs-lookup"><span data-stu-id="b554a-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="b554a-107">V okne príkazového riadka zadajte **príkaz dsregcmd /leave**  a počkajte, kým sa príkaz dokončí.</span><span class="sxs-lookup"><span data-stu-id="b554a-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="b554a-108">Potom zadajte **dsregcmd /join** a počkajte, kým sa dokončí príkaz.</span><span class="sxs-lookup"><span data-stu-id="b554a-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="b554a-109">Reštartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="b554a-109">Reboot your computer.</span></span>

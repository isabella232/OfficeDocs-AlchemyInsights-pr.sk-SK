---
title: chyba 0x8004de40 pri spúšťaní OneDrivu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823117"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="fab40-102">chyba 0x8004de40 pri spúšťaní OneDrivu</span><span class="sxs-lookup"><span data-stu-id="fab40-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="fab40-103">Ak sa pri prihlasovaní do služby OneDrive zobrazí chybové hlásenie **0x8004de40** , reštartujte počítač pri pripojení k pracovnej alebo školskej doméne.</span><span class="sxs-lookup"><span data-stu-id="fab40-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="fab40-104">Ak sa po reštartovaní zobrazí táto chyba, skúste to pri pripojení k pracovnej alebo školskej doméne:</span><span class="sxs-lookup"><span data-stu-id="fab40-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="fab40-105">Kliknite na tlačidlo Štart a do vyhľadávacieho poľa zadajte príkaz **cmd** alebo **Príkazový riadok**  , kliknite pravým tlačidlom myši na aplikáciu príkazového riadka a vyberte položku  **Spustiť ako správca** .</span><span class="sxs-lookup"><span data-stu-id="fab40-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator** .</span></span> <span data-ttu-id="fab40-106">Ak sa zobrazí výzva na zadanie hesla správcu alebo na potvrdenie, zadajte heslo alebo kliknite na položku **Povoliť** .</span><span class="sxs-lookup"><span data-stu-id="fab40-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow** .</span></span>  

2. <span data-ttu-id="fab40-107">V okne príkazového riadka zadajte **dsregcmd/Leave**  a počkajte, kým sa príkaz dokončí.</span><span class="sxs-lookup"><span data-stu-id="fab40-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="fab40-108">Potom zadajte **dsregcmd/JOIN** a počkajte, kým sa príkaz dokončí.</span><span class="sxs-lookup"><span data-stu-id="fab40-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="fab40-109">Reštartujte počítač.</span><span class="sxs-lookup"><span data-stu-id="fab40-109">Reboot your computer.</span></span>

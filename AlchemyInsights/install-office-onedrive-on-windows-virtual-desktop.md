---
title: Inštalácia balíka Office a OneDrivu vo virtuálnej pracovnej ploche Windowsu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596027"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="63506-102">Inštalácia balíka Office a OneDrivu vo virtuálnej pracovnej ploche Windowsu</span><span class="sxs-lookup"><span data-stu-id="63506-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="63506-103">[Pripravte a prispôsobte nadradený obrázok VHD.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)</span><span class="sxs-lookup"><span data-stu-id="63506-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="63506-104">Vytvorte virtuálny počítač (VM), ak ešte nebol vytvorený.</span><span class="sxs-lookup"><span data-stu-id="63506-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="63506-105">[Inštalácia balíka Office v režime aktivácie zdieľaného počítača.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="63506-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="63506-106">Aktivácia zdieľaného počítača umožňuje viacerým používateľom prístup k balíku Office.</span><span class="sxs-lookup"><span data-stu-id="63506-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="63506-107">[Nainštalujte OneDrive v režime pre počítač.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="63506-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="63506-108">Zvyčajne sa OneDrive inštaluje pre jedného používateľa, ale tu by sa mal nainštalovať do počítača.</span><span class="sxs-lookup"><span data-stu-id="63506-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>
---
title: Oprava chyby 0x8004de40 vo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745145"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="de39b-102">Oprava chyby 0x8004de40 vo OneDrive</span><span class="sxs-lookup"><span data-stu-id="de39b-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="de39b-103">Ak sa v službe OneDrive zobrazí chyba 0x8004de40:</span><span class="sxs-lookup"><span data-stu-id="de39b-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="de39b-104">Reštartujte postihnutý počítač pri pripojení k doméne adresára Acitve.</span><span class="sxs-lookup"><span data-stu-id="de39b-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="de39b-105">Ak sa problém nevyrieši reštartovaním, odhláste sa a znova sa prihláste do svojho zariadenia zo služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="de39b-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="de39b-106">**Poznámka**: pri vykonaní týchto krokov by ste sa mali nachádzať v podnikovej sieti.</span><span class="sxs-lookup"><span data-stu-id="de39b-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="de39b-107">Nevykonávajte tieto kroky, ak sa nedokážete pripojiť k podnikovej infraštruktúre (napríklad na cestách).</span><span class="sxs-lookup"><span data-stu-id="de39b-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="de39b-108">Otvorte príkazový riadok s právami správcu.</span><span class="sxs-lookup"><span data-stu-id="de39b-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="de39b-109">Ak chcete otvoriť príkazový riadok s právami správcu, kliknite na tlačidlo **Štart**, kliknite pravým tlačidlom myši na **Príkazový riadok**a potom kliknite na položku **Spustiť ako správca**.</span><span class="sxs-lookup"><span data-stu-id="de39b-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="de39b-110">Zadajte *dsregcmd/Leave* a stlačte kláves **Enter**.</span><span class="sxs-lookup"><span data-stu-id="de39b-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="de39b-111">Po vyplnení zadajte *dsregcmd/JOIN* a stlačte kláves **Enter**.</span><span class="sxs-lookup"><span data-stu-id="de39b-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="de39b-112">Po skončení zatvoríte príkazový riadok.</span><span class="sxs-lookup"><span data-stu-id="de39b-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="de39b-113">Reštartujte počítač a prihláste sa do služby OneDrive.</span><span class="sxs-lookup"><span data-stu-id="de39b-113">Reboot the computer, and log into OneDrive.</span></span>
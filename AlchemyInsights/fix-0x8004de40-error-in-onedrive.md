---
title: Fix 0x8004de40 chyba v OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755863"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="26254-102">Fix 0x8004de40 chyba v OneDrive</span><span class="sxs-lookup"><span data-stu-id="26254-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="26254-103">Ak sa zobrazí chyba 0x8004de40 OneDrive:</span><span class="sxs-lookup"><span data-stu-id="26254-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="26254-104">Reštartujte postihnutého počítača pri pripojení k doméne Acitve adresára.</span><span class="sxs-lookup"><span data-stu-id="26254-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="26254-105">Ak sa problém nevyrieši reštartovaním, zrušte pripojenie a znova pripojte zariadenie z Azure AD.</span><span class="sxs-lookup"><span data-stu-id="26254-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="26254-106">**Poznámka**: pri vykonávaní týchto krokov by ste mali byť v podnikovej sieti.</span><span class="sxs-lookup"><span data-stu-id="26254-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="26254-107">Nevykonávajte tieto kroky, keď sa nebudete môcť pripojiť k podnikovej infraštruktúre (napríklad pri cestovaní).</span><span class="sxs-lookup"><span data-stu-id="26254-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="26254-108">Otvorte príkazový riadok s právami správcu.</span><span class="sxs-lookup"><span data-stu-id="26254-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="26254-109">Ak chcete otvoriť príkazový riadok s právami správcu, kliknite na tlačidlo **Štart**, kliknite pravým tlačidlom myši na položku **Príkazový riadok**a potom kliknite na položku **Spustiť ako správca**.</span><span class="sxs-lookup"><span data-stu-id="26254-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="26254-110">Typ *dsregcmd/opustiť* a stlačte kláves **Enter**.</span><span class="sxs-lookup"><span data-stu-id="26254-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="26254-111">Po dokončení zadajte *dsregcmd/JOIN* a stlačte kláves **Enter**.</span><span class="sxs-lookup"><span data-stu-id="26254-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="26254-112">Po dokončení zatvorte príkazový riadok.</span><span class="sxs-lookup"><span data-stu-id="26254-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="26254-113">Reštartujte počítač a prihláste sa do OneDrivu.</span><span class="sxs-lookup"><span data-stu-id="26254-113">Reboot the computer, and log into OneDrive.</span></span>
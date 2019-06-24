---
title: Oprava 0x8004de40 chyby v službe OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133991"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="7ba22-102">Oprava 0x8004de40 chyby v službe OneDrive</span><span class="sxs-lookup"><span data-stu-id="7ba22-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="7ba22-103">Ak sa zobrazí chybové hlásenie 0x8004de40 s OneDrive:</span><span class="sxs-lookup"><span data-stu-id="7ba22-103">If you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="7ba22-104">Reštartujte postihnutého počítača, keď ste pripojení k doméne atívny adresár.</span><span class="sxs-lookup"><span data-stu-id="7ba22-104">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="7ba22-105">Ak sa problém nevyrieši reštartovaním počítača, odpojenie a opusťte zariadenia z Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7ba22-105">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="7ba22-106">**Poznámka**: mali by ste byť na vašej firemnej sieti pri vykonávaní týchto krokov.</span><span class="sxs-lookup"><span data-stu-id="7ba22-106">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="7ba22-107">Nemusíte vykonávať tieto kroky, keď nie ste schopní sa pripojiť k vašej firemnej infraštruktúry (napríklad pri cestovaní).</span><span class="sxs-lookup"><span data-stu-id="7ba22-107">Don't perform these steps when you aren't able to connect to your corporate infrastructure (for example, while traveling).</span></span> 

- <span data-ttu-id="7ba22-108">Otvorte námer kontrolovať vrtký.</span><span class="sxs-lookup"><span data-stu-id="7ba22-108">Open an elevated command prompt.</span></span> 
- <span data-ttu-id="7ba22-109">Otvorte námer kontrolovať vrtký, kliknutím na tlačidlo - **Štart**, kliknite pravým tlačidlom myši **Príkazový riadok**a potom kliknite na položku **Spustiť ako správca**.</span><span class="sxs-lookup"><span data-stu-id="7ba22-109">To open an elevated command prompt, click - **Start**, right-click **Command Prompt**, and then click **Run as administrator**.</span></span>
- <span data-ttu-id="7ba22-110">Zadajte *dsregcmd /leave* a stlačte kláves **Enter**.</span><span class="sxs-lookup"><span data-stu-id="7ba22-110">Type *dsregcmd /leave* and press **Enter**.</span></span>
- <span data-ttu-id="7ba22-111">Po dokončení *zadajte/JOIN dsregcmd* a stlačte kláves **Enter**.</span><span class="sxs-lookup"><span data-stu-id="7ba22-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>
- <span data-ttu-id="7ba22-112">Keď kompletné, zatvorte príkazový riadok.</span><span class="sxs-lookup"><span data-stu-id="7ba22-112">When complete, close the command prompt.</span></span>
- <span data-ttu-id="7ba22-113">Reštartujte počítač a prihláste sa do OneDrive.</span><span class="sxs-lookup"><span data-stu-id="7ba22-113">Reboot the computer, and log into OneDrive.</span></span>
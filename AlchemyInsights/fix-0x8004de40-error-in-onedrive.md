---
title: Oprava 0x8004de40 vo OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649763"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="a65fb-102">Oprava 0x8004de40 vo OneDrive</span><span class="sxs-lookup"><span data-stu-id="a65fb-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="a65fb-103">Ak používate Windows 7 a zobrazí sa táto chyba, pri aktualizácii zapnite protokol [TLS 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ako predvolené zabezpečené protokoly v systéme WinHTTP vo Windowse.</span><span class="sxs-lookup"><span data-stu-id="a65fb-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="a65fb-104">Ak používate Windows 10 a vo OneDrive sa 0x8004de40 chyba:</span><span class="sxs-lookup"><span data-stu-id="a65fb-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="a65fb-105">Po pripojení k doméne adresára Acitve reštartujte ovplyvnený počítač.</span><span class="sxs-lookup"><span data-stu-id="a65fb-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="a65fb-106">Ak reštartovanie nepomôže problém vyriešiť, odpojte sa a znova sa pripojiť k zariadeniu zo služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a65fb-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="a65fb-107">**Poznámka:** Pri vykonávaní týchto krokov by ste sa mali nachádzať vo vašej podnikovej sieti.</span><span class="sxs-lookup"><span data-stu-id="a65fb-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="a65fb-108">Tieto kroky nepoužívajte, keď nie ste pripojení k podnikovej infraštruktúre (napríklad na cestách).</span><span class="sxs-lookup"><span data-stu-id="a65fb-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="a65fb-109">Výberom tlačidla Štart otvorte príkazový riadok bez **oprávnení**, kliknite pravým tlačidlom myši na **položku Príkazový** riadok a potom **vyberte položku Spustiť ako správca.**</span><span class="sxs-lookup"><span data-stu-id="a65fb-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="a65fb-110">Zadajte *dsregcmd /leave a* stlačte kláves **Enter.**</span><span class="sxs-lookup"><span data-stu-id="a65fb-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="a65fb-111">Po dokončení zadajte *dsregcmd /join a* stlačte kláves **Enter.**</span><span class="sxs-lookup"><span data-stu-id="a65fb-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="a65fb-112">Po dokončení zatvorte príkazový riadok.</span><span class="sxs-lookup"><span data-stu-id="a65fb-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="a65fb-113">Reštartujte počítač a prihláste sa do služby OneDrive.</span><span class="sxs-lookup"><span data-stu-id="a65fb-113">Reboot the computer, and log into OneDrive.</span></span>
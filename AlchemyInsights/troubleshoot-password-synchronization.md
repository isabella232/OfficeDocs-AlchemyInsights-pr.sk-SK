---
title: Riešenie problémov s synchronizáciou hesla
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732525"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="d2d40-102">Riešenie problémov s synchronizáciou hesla</span><span class="sxs-lookup"><span data-stu-id="d2d40-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="d2d40-103">Riešenie problémov, kde žiadne heslá sú synchronizované s Azure AD Connect verzie 1.1.614.0 alebo novšej:</span><span class="sxs-lookup"><span data-stu-id="d2d40-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="d2d40-104">Otvorte novú reláciu prostredia Windows PowerShell na serveri Azure AD Connect s možnosťou **Spustiť ako správca** .</span><span class="sxs-lookup"><span data-stu-id="d2d40-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="d2d40-105">Spustiť **súbor executionpolicy RemoteSigned** alebo **set-executionpolicy neobmedzený**.</span><span class="sxs-lookup"><span data-stu-id="d2d40-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="d2d40-106">Spustite Sprievodcu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d2d40-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="d2d40-107">Prejdite na stránku **ďalšie úlohy** , vyberte **Riešenie problémov**a kliknite na tlačidlo **ďalej**.</span><span class="sxs-lookup"><span data-stu-id="d2d40-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="d2d40-108">Na stránke Riešenie problémov, kliknite na tlačidlo **Spustiť spustite ponuku riešenie problémov** v prostredí PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d2d40-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="d2d40-109">V hlavnej ponuke vyberte položku **Riešenie problémov s synchronizáciou hesiel**.</span><span class="sxs-lookup"><span data-stu-id="d2d40-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="d2d40-110">V sub menu, vyberte **heslo synchronizácia nefunguje vôbec**.</span><span class="sxs-lookup"><span data-stu-id="d2d40-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="d2d40-111">**Pochopenie výsledkov úlohy pri riešení problémov**</span><span class="sxs-lookup"><span data-stu-id="d2d40-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="d2d40-112">Riešenie problémov úloha vykonáva nasledujúce kontroly:</span><span class="sxs-lookup"><span data-stu-id="d2d40-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="d2d40-113">Overuje, či je zapnutá funkcia synchronizácie hesiel pre nájomcu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d2d40-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="d2d40-114">Overuje, či server Azure AD Connect nie je v režime oddychové.</span><span class="sxs-lookup"><span data-stu-id="d2d40-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="d2d40-115">Pre každý existujúci lokálny konektor služby Active Directory (ktorý zodpovedá existujúcej doménovej štruktúre služby Active Directory):</span><span class="sxs-lookup"><span data-stu-id="d2d40-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="d2d40-116">Overuje, či je zapnutá funkcia synchronizácie hesiel.</span><span class="sxs-lookup"><span data-stu-id="d2d40-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="d2d40-117">Vyhľadáva heslo synchronizácia heartbeat udalosti v denníku udalostí aplikácie systému Windows.</span><span class="sxs-lookup"><span data-stu-id="d2d40-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="d2d40-118">Pre každú doménu služby Active Directory v lokálnom konektor služby Active Directory:</span><span class="sxs-lookup"><span data-stu-id="d2d40-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="d2d40-119">Overuje, či je doména dostupná zo servera Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d2d40-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="d2d40-120">Overuje, či kontá služby Active Directory Domain (AD DS), ktoré používa lokálny konektor služby Active Directory, má správne používateľské meno, heslo a povolenia potrebné na synchronizáciu hesla.</span><span class="sxs-lookup"><span data-stu-id="d2d40-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="d2d40-121">Ďalšie pomoc pri riešení problémov so synchronizáciou hesiel nájdete v téme [Riešenie problémov s synchronizáciou hesiel pomocou synchronizácie Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d2d40-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  
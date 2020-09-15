---
title: Inštalácia balíka Office na terminálový server – bez platnej licencie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663132"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="5c9e3-102">Inštalácia balíka Office na terminálový Server</span><span class="sxs-lookup"><span data-stu-id="5c9e3-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="5c9e3-103">Nasadenie aplikácií Microsoft 365 pre podniky na serveri Windows pomocou služby Remote Desktop Services (RDS), predtým pomenovaných terminálových služieb:</span><span class="sxs-lookup"><span data-stu-id="5c9e3-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="5c9e3-104">Musíte mať predplatné na Microsoft 365, ktoré zahŕňa aplikácie Microsoft 365 pre podniky, ako napríklad Office 365 Enterprise E3 alebo Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="5c9e3-105">Aplikácie Microsoft 365 for Business a Microsoft 365 Apps for Business Premium nezahŕňajú aplikácie Microsoft 365 pre podniky.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="5c9e3-106">Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="5c9e3-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="5c9e3-107">Ak chcete nainštalovať aplikácie Microsoft 365 pre podniky z RDS z centra spravovania služby Microsoft 365, v ***ktorom sa používajú predvolené nastavenia inštalácie***, postupujte podľa nasledujúcich krokov.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="5c9e3-108">Môžete si tiež stiahnuť a spustiť [nástroj Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) na inštaláciu aplikácií Microsoft 365 pre podniky v režime aktivácie zdieľaného počítača.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="5c9e3-109">Skontrolujte, aké predplatné služieb Microsoft 365 máte.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="5c9e3-110">Zistite, ako</span><span class="sxs-lookup"><span data-stu-id="5c9e3-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="5c9e3-111">Ak je to potrebné, prepnite na iné predplatné na Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="5c9e3-112">Zistite, ako</span><span class="sxs-lookup"><span data-stu-id="5c9e3-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="5c9e3-113">Ak je Office už nainštalovaný na serveri RDS pomocou akéhokoľvek iného predplatného služby Microsoft 365, odinštalujte ho.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="5c9e3-114">Ak napríklad prejdete na položku Ovládací panel, \> odinštalujte program.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="5c9e3-115">Ak máte problémy, odinštalujte ho pomocou [podpory spoločnosti Microsoft a Sprievodcu obnovením](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="5c9e3-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="5c9e3-116">Na serveri RDS sa prihláste do centra spravovania služby Microsoft 365 s kontom správcu a [nainštalujte si aplikácie microsoft 365 pre podniky](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="5c9e3-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="5c9e3-117">Po nainštalovaní balíka Office sa ***neotvárajte ani sa prihláste*** do žiadnej aplikácie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="5c9e3-118">Na serveri RDS zapnite aktiváciu zdieľaného počítača úpravou databázy registry vykonaním týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="5c9e3-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="5c9e3-119">Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku spustiť.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="5c9e3-120">Do poľa Otvoriť zadajte **príkaz regedit**a potom kliknite na tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="5c9e3-121">Keď sa zobrazí výzva, vyberte možnosť Áno, ak chcete povoliť Editor databázy Registry vykonávať zmeny v zariadení.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="5c9e3-122">V editore databázy Registry pridajte hodnotu reťazca **SharedComputerLicensing** s nastavením 1 v časti HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="5c9e3-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="5c9e3-123">Na serveri RDS sa ***prihláste ako koncový používateľ*** a [overte, či je povolená Aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="5c9e3-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="5c9e3-124">Ďalšie podrobnosti o predpokladoch, pokyny na nastavenie a pokyny na prispôsobených inštaláciách pomocou nástroja na nasadenie balíka Office nájdete v téme [nasadenie aplikácií Microsoft 365 pre podniky pomocou služby Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="5c9e3-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="5c9e3-125">Ak chcete opraviť chyby súvisiace s aktiváciou zdieľaného počítača, prečítajte si tému [Riešenie problémov s aktiváciou zdieľania počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="5c9e3-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  
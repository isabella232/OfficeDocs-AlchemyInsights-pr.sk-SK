---
title: Inštalácia balíka Office na terminálový Server - bez licencie
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508643"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="cf3d4-102">Inštalácia balíka Office na terminálový Server</span><span class="sxs-lookup"><span data-stu-id="cf3d4-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="cf3d4-103">Nasadenie aplikácií Microsoft 365 pre podniky na serveri Windows Server pomocou služieb vzdialenej skúsenosti s prácou s počítačom (RDS), predtým s názvom Terminálové služby:</span><span class="sxs-lookup"><span data-stu-id="cf3d4-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="cf3d4-104">Musíte mať predplatné na Microsoft 365, ktoré zahŕňa aplikácie Microsoft 365 pre podniky, napríklad Office 365 Enterprise E3 alebo Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="cf3d4-105">Plány Microsoft 365 Apps for business a Microsoft 365 Apps for business Premium nezahŕňajú aplikácie Microsoft 365 pre podniky.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="cf3d4-106">Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="cf3d4-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="cf3d4-107">Ak chcete nainštalovať Microsoft 365 Aplikácie pre podniky na RDS z Centra spravovania Služby Microsoft 365, ***ktorý používa predvolené nastavenia inštalácie***, postupujte nasledovne.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="cf3d4-108">Môžete tiež prevziať a spustiť [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) nainštalovať Microsoft 365 Apps pre podniky v režime aktivácie zdieľaného počítača.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="cf3d4-109">Skontrolujte, aké predplatné na Microsoft 365 máte.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="cf3d4-110">Prečítajte si, ako</span><span class="sxs-lookup"><span data-stu-id="cf3d4-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="cf3d4-111">V prípade potreby prepnite na iné predplatné služby Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="cf3d4-112">Prečítajte si, ako</span><span class="sxs-lookup"><span data-stu-id="cf3d4-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="cf3d4-113">Ak je balík Office už nainštalovaný na serveri RDS pomocou iných predplatných služieb Microsoft 365, odinštalujte ho.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="cf3d4-114">Napríklad tým, že prejdete na Ovládací panel \> Odinštalovať program.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="cf3d4-115">Ak sa vyskytnú problémy, odinštalujte ju pomocou [nástroja Microsoft Support and Recovery Assistant.](https://aka.ms/SARA-OfficeUninstall-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="cf3d4-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="cf3d4-116">Na serveri RDS sa prihláste do Centra spravovania služby Microsoft 365 pomocou konta správcu a [nainštalujte aplikácie Microsoft 365 apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="cf3d4-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="cf3d4-117">Po nainštalovaní balíka Office ***sa neotvárajte ani neprihlasujte*** do žiadnych aplikácií balíka Office.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="cf3d4-118">Na serveri RDS, povoliť aktiváciu zdieľaného počítača úpravou databázy registry pomocou nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="cf3d4-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="cf3d4-119">Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku Spustiť.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="cf3d4-120">Do poľa Otvoriť zadajte **regedit**a potom kliknite na tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="cf3d4-121">Po zobrazení výzvy vyberte možnosť Yes (Áno), aby Editor databázy Registry mohol vykonať zmeny v zariadení.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="cf3d4-122">V Editore databázy Registry pridajte hodnotu reťazca **SharedComputerLicensing** s nastavením 1 v časti HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="cf3d4-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="cf3d4-123">Na serveri RDS ***sa prihláste ako koncový používateľ*** a [overte, či je zapnutá aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="cf3d4-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="cf3d4-124">Ďalšie podrobnosti o predpokladoch, pokynoch na nastavenie a pokynoch na prispôsobené inštalácie pomocou nástroja na nasadenie balíka Office nájdete v téme [Nasadenie aplikácií Microsoft 365 pre podniky pomocou služieb vzdialenej pracovnej plochy](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="cf3d4-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="cf3d4-125">Ak chcete opraviť chyby súvisiace s aktiváciou zdieľaného počítača, pozrite si tému [Riešenie problémov so zdieľanou aktiváciou počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="cf3d4-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  
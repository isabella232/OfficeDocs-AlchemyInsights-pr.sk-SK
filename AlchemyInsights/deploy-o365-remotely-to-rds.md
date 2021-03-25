---
title: Nasadenie aplikácií Microsoft 365 pre podniky na zdieľané používanie v RDS, terminálovom serveri alebo VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200688"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="73b71-102">Nasadenie aplikácií Microsoft 365 pre podniky na zdieľané používanie v RDS, terminálovom serveri alebo VDI</span><span class="sxs-lookup"><span data-stu-id="73b71-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="73b71-103">Nasadenie aplikácií Microsoft 365 pre podniky pomocou služieb Remote Desktop Services (RDS), predtým pomenovaných terminálových služieb:</span><span class="sxs-lookup"><span data-stu-id="73b71-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="73b71-104">Musíte mať plán služieb Microsoft 365 for Business alebo plán Office 365, ktorý zahŕňa aplikácie Microsoft 365 pre podniky, ako napríklad Office 365 Enterprise E3 alebo Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="73b71-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="73b71-105">Microsoft 365 Apps for Business a Microsoft 365 Business Standard plány nezahŕňajú aplikácie Microsoft 365 pre podniky.</span><span class="sxs-lookup"><span data-stu-id="73b71-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="73b71-106">Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="73b71-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="73b71-107">Môžete si tiež stiahnuť a spustiť [nástroj Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) na inštaláciu aplikácií Microsoft 365 pre podniky v režime aktivácie zdieľaného počítača.</span><span class="sxs-lookup"><span data-stu-id="73b71-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="73b71-108">Ďalšie informácie o predpokladoch, pokyny na nastavenie a pokyny týkajúce sa prispôsobených inštalácií pomocou nástroja na nasadenie balíka Office nájdete v téme [nasadenie aplikácií Microsoft 365 pre podniky pomocou služby Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="73b71-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="73b71-109">Riešenie chýb súvisiacich s aktiváciou zdieľaného počítača:</span><span class="sxs-lookup"><span data-stu-id="73b71-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="73b71-110">Pozrite si tému [Riešenie problémov s aktiváciou zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="73b71-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="73b71-111">Pozrite si tému [Resetovanie stavu aktivácie služby Aplikácie Microsoft 365 pre veľké organizácie](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="73b71-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="73b71-112">Ak chcete nainštalovať aplikácie Microsoft 365 pre podniky z RDS z centra spravovania služby Microsoft 365, v ***ktorom sa používajú predvolené nastavenia inštalácie***, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="73b71-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="73b71-113">Skontrolujte, aké predplatné máte.</span><span class="sxs-lookup"><span data-stu-id="73b71-113">Check what subscription you have.</span></span> <span data-ttu-id="73b71-114">[Zistite, ako](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)na to.</span><span class="sxs-lookup"><span data-stu-id="73b71-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="73b71-115">Ak je to potrebné, prepnite na iné predplatné.</span><span class="sxs-lookup"><span data-stu-id="73b71-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="73b71-116">[Zistite, ako](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)na to.</span><span class="sxs-lookup"><span data-stu-id="73b71-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="73b71-117">Ak je balík Office už nainštalovaný na serveri RDS pomocou iného predplatného služby Microsoft, odinštalujte ho.</span><span class="sxs-lookup"><span data-stu-id="73b71-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="73b71-118">Ak napríklad prejdete na položku **Ovládací panel**,  >  **odinštalujte program**.</span><span class="sxs-lookup"><span data-stu-id="73b71-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="73b71-119">Ak máte problémy, odinštalujte ho pomocou [podpory spoločnosti Microsoft a Sprievodcu obnovením](https://aka.ms/SARA-OfficeUninstall-Alchemy) .</span><span class="sxs-lookup"><span data-stu-id="73b71-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="73b71-120">Na serveri RDS sa prihláste do centra spravovania služby Microsoft 365 s kontom správcu a [nainštalujte si aplikácie microsoft 365 pre podniky](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="73b71-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="73b71-121">Po nainštalovaní balíka Office sa ***neotvárajte ani sa prihláste*** do žiadnej aplikácie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="73b71-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="73b71-122">Na serveri RDS zapnite aktiváciu zdieľaného počítača úpravou databázy registry vykonaním týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="73b71-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="73b71-123">Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku **Spustiť**.</span><span class="sxs-lookup"><span data-stu-id="73b71-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="73b71-124">Do poľa Otvoriť zadajte **príkaz regedit** a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="73b71-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="73b71-125">Keď sa zobrazí výzva, vyberte možnosť **Áno** , ak chcete povoliť Editor databázy Registry vykonávať zmeny v zariadení.</span><span class="sxs-lookup"><span data-stu-id="73b71-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="73b71-126">V editore databázy Registry pridajte hodnotu reťazca **SharedComputerLicensing** s nastavením 1 v časti HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="73b71-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="73b71-127">Na serveri RDS sa ***prihláste ako koncový používateľ*** a [overte, či je povolená Aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="73b71-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

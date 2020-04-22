---
title: Inštalácia balíka Office na terminálový server-bez licencie
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
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763232"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="484c6-102">Inštalácia balíka Office na terminálový Server</span><span class="sxs-lookup"><span data-stu-id="484c6-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="484c6-103">Nasadenie Microsoft 365 aplikácie pre podniky na Windows Server pomocou Remote Desktop Services (RDS), predtým pomenované terminálové služby:</span><span class="sxs-lookup"><span data-stu-id="484c6-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="484c6-104">Musíte mať predplatné Microsoft 365, ktorý obsahuje Microsoft 365 aplikácie pre podniky, napríklad Office 365 Enterprise E3 alebo Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="484c6-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="484c6-105">Microsoft 365 aplikácie pre podniky a Microsoft 365 aplikácie Business Premium plány nezahŕňajú Microsoft 365 aplikácie pre podniky.</span><span class="sxs-lookup"><span data-stu-id="484c6-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="484c6-106">Musíte zapnúť [aktiváciu zdieľaného počítača](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="484c6-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="484c6-107">Ak chcete nainštalovať Microsoft 365 aplikácie pre Enterprise na RDS z Microsoft 365 admin Center, ***ktorý používa predvolené nastavenie inštalácie***, použite nasledovný postup.</span><span class="sxs-lookup"><span data-stu-id="484c6-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="484c6-108">Môžete tiež stiahnuť a spustiť [Microsoft Support a zotavenie asistent](https://aka.ms/SaRA_OfficeSCA_M365Portal) nainštalovať Microsoft 365 aplikácie pre podniky v režime zdieľaného počítača aktivácie.</span><span class="sxs-lookup"><span data-stu-id="484c6-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="484c6-109">Skontrolujte, čo Microsoft 365 predplatné máte.</span><span class="sxs-lookup"><span data-stu-id="484c6-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="484c6-110">Zistite, ako</span><span class="sxs-lookup"><span data-stu-id="484c6-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="484c6-111">Ak je to potrebné, prepnite na iný Microsoft 365 predplatné.</span><span class="sxs-lookup"><span data-stu-id="484c6-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="484c6-112">Zistite, ako</span><span class="sxs-lookup"><span data-stu-id="484c6-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="484c6-113">Ak Office je už nainštalovaný na serveri RDS pomocou iných Microsoft 365 predplatné, odinštalujte ho.</span><span class="sxs-lookup"><span data-stu-id="484c6-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="484c6-114">Napríklad prechodom na Ovládací panel \> odinštalujte program.</span><span class="sxs-lookup"><span data-stu-id="484c6-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="484c6-115">Odinštalovanie pomocou [technickej podpory spoločnosti Microsoft a obnovenie asistent](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ak používate problémy.</span><span class="sxs-lookup"><span data-stu-id="484c6-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="484c6-116">Na serveri RDS, prihláste sa do Microsoft 365 admin Center s kontom správcu a [nainštalovať Microsoft 365 aplikácie pre podniky](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="484c6-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="484c6-117">Po nainštalovaní balíka Office, ***neotvárajte ani sa prihlásiť*** do žiadnej aplikácie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="484c6-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="484c6-118">Na serveri RDS zapnúť aktiváciu zdieľaného počítača úpravou databázy Registry pomocou nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="484c6-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="484c6-119">Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku spustiť.</span><span class="sxs-lookup"><span data-stu-id="484c6-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="484c6-120">Do poľa Otvoriť zadajte **príkaz regedit**a potom kliknite na tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="484c6-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="484c6-121">Ak sa zobrazí výzva na povolenie editora databázy Registry, vyberte možnosť Yes (Áno), čím vykonáte zmeny v zariadení.</span><span class="sxs-lookup"><span data-stu-id="484c6-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="484c6-122">V editore databázy Registry pridajte hodnotu reťazca **Sharedcomputerlicensing** s nastavením 1 podľa HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="484c6-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="484c6-123">Na serveri RDS sa ***prihláste ako koncový používateľ*** a [overte, či je zapnutá Aktivácia zdieľaného počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="484c6-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="484c6-124">Ďalšie informácie o predpoklady, pokyny na nastavenie a pokyny na prispôsobené inštalácie pomocou nástroja Office Deployment, nájdete [nasadenie Microsoft 365 aplikácie pre podniky pomocou služby vzdialenej skúsenosti s prácou s počítačom](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="484c6-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="484c6-125">Ak chcete opraviť chyby súvisiace so zdieľanou aktiváciou počítača, prečítajte si článok [Riešenie problémov so zdieľanou aktiváciou počítača pre aplikácie Microsoft 365 pre podniky](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="484c6-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  
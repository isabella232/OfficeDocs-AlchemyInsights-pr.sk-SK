---
title: Inštalácia office na terminálový Server - bez licencie
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 6fc4bd5f6971ca833084a6a8ad6c25b3fdafb8dc
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35381744"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="8e40c-102">Inštalácia balíka Office na terminálový Server</span><span class="sxs-lookup"><span data-stu-id="8e40c-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="8e40c-103">Na nasadenie balíka Office 365 ProPlus na serveri Windows Server pomocou Remote Desktop Services (RDS), pôvodne pomenovaný terminálových služieb:</span><span class="sxs-lookup"><span data-stu-id="8e40c-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="8e40c-104">Musíte mať plán služieb Office 365, ktorý obsahuje Office 365 ProPlus, napríklad Office 365 Enterprise E3 alebo Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="8e40c-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="8e40c-105">Plány Office 365 Business a Office 365 Business Premium nezahŕňajú Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="8e40c-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="8e40c-106">Musíte zapnúť [aktiváciou zdieľaný počítač](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8e40c-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="8e40c-107">Ak chcete nainštalovať Office 365 ProPlus na RDS z Office 365 portálu, \*\* *ktoré používa predvolené nastavenia inštalácie* \*\*, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="8e40c-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, \*\* *which uses default installation settings* \*\*, follow these steps:</span></span>
  
1. <span data-ttu-id="8e40c-108">Skontrolujte, aký máte plán služieb Office 365.</span><span class="sxs-lookup"><span data-stu-id="8e40c-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="8e40c-109">Zistite ako</span><span class="sxs-lookup"><span data-stu-id="8e40c-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="8e40c-110">Ak potrebné, prepnúť na rôzne Office 365 plánu.</span><span class="sxs-lookup"><span data-stu-id="8e40c-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="8e40c-111">Zistite ako</span><span class="sxs-lookup"><span data-stu-id="8e40c-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="8e40c-112">Ak Office je už nainštalovaný na serveri RDS používať iné plány služieb Office 365, odinštalujte ju.</span><span class="sxs-lookup"><span data-stu-id="8e40c-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="8e40c-113">Napríklad tým, že pôjdete do ovládacieho panela \> odinštalovať program.</span><span class="sxs-lookup"><span data-stu-id="8e40c-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="8e40c-114">Odinštalovať pomocou [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ak ste beží do problémov.</span><span class="sxs-lookup"><span data-stu-id="8e40c-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="8e40c-115">RDS serveri, prihláste sa na portáli Office 365 konto správcu a [inštaláciu balíka Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="8e40c-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="8e40c-116">Po nainštalovaní balíka Office \*\* *neotvárajte ani prihlásiť* \*\* všetky aplikácie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="8e40c-116">After Office is installed, \*\* *don't open or sign in* \*\* to any Office applications.</span></span>

6. <span data-ttu-id="8e40c-117">Na serveri RDS povoliť aktiváciou zdieľaný počítač úpravou databázy registry pomocou nasledujúcich krokov:</span><span class="sxs-lookup"><span data-stu-id="8e40c-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="8e40c-118">Kliknite pravým tlačidlom myši na tlačidlo Windows v ľavom dolnom rohu obrazovky a vyberte položku spustiť.</span><span class="sxs-lookup"><span data-stu-id="8e40c-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="8e40c-119">Do poľa Otvoriť zadajte **príkaz regedit**a potom kliknite na tlačidlo OK.</span><span class="sxs-lookup"><span data-stu-id="8e40c-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="8e40c-120">Vybrať áno keď výzva na povolenie Editor databázy Registry zmeny do vášho zariadenia.</span><span class="sxs-lookup"><span data-stu-id="8e40c-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="8e40c-121">V editore databázy Registry pridajte hodnotu reťazca **SharedComputerLicensing** s nastavenie 1 pod HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="8e40c-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="8e40c-122">Na serveri RDS \*\* *Prihlásiť ako koncový používateľ* \*\* a [overiť, že aktiváciou zdieľaný počítač zapnutá pre Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="8e40c-122">On the RDS server, \*\* *sign in as an end user* \*\* and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="8e40c-123">Viac informácií o predpoklady, pokynov a usmernenia na prispôsobenej inštalácie pomocou nástroja nasadenia Office, nájdete [Nasadenie balíka Office 365 ProPlus pomocou služby vzdialenej pracovnej plochy](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="8e40c-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="8e40c-124">Opraviť chyby súvisiace s aktiváciou zdieľaný počítač nájdete v [článku Riešenie problémov s aktiváciou zdieľaný počítač pre Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="8e40c-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  
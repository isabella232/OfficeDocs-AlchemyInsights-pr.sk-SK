---
title: Intune nasadenie aplikácií Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461991"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="dff13-102">Intune nasadenie aplikácií Win32</span><span class="sxs-lookup"><span data-stu-id="dff13-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="dff13-103">Microsoft Intune povoľuje aplikácie Win32 vrátane, ale nie výhradne, MSI a. EXE, ktorý sa má nasadiť v zariadeniach s Windowsom 10.</span><span class="sxs-lookup"><span data-stu-id="dff13-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="dff13-104">Použitý mechanizmus nasadenia vyžaduje, aby sa v cieľovom zariadení nachádzalo rozšírenie správy služby Intune (IME).</span><span class="sxs-lookup"><span data-stu-id="dff13-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="dff13-105">Editor IME sa automaticky nainštaluje ako výsledok zamerania skriptu prostredia PowerShell alebo nasadenia aplikácie Win32 na používateľa alebo zariadenie.</span><span class="sxs-lookup"><span data-stu-id="dff13-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="dff13-106">K dispozícii je tiež množina predpokladov, ktoré musia byť splnené, aby sa nasadili aplikácie Win32, ktoré zahŕňajú:</span><span class="sxs-lookup"><span data-stu-id="dff13-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="dff13-107">Podporované platformy: Windows 10 version 1607 alebo novšia verzia (podnikové, Pro a vzdelávacie verzie).</span><span class="sxs-lookup"><span data-stu-id="dff13-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="dff13-108">Podporovaná architektúra: x86 a x64.</span><span class="sxs-lookup"><span data-stu-id="dff13-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="dff13-109">Správa zariadenia: AAD sa pripojil a automaticky zaregistroval (vrátane hybridnej domény pripojenej a skupinovej politiky automaticky zaregistrovaných).</span><span class="sxs-lookup"><span data-stu-id="dff13-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="dff13-110">Formát balíka aplikácií:. súbor **intunewin**  pripravený nástrojom na [prípravu obsahu Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="dff13-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="dff13-111">Obmedzenia</span><span class="sxs-lookup"><span data-stu-id="dff13-111">Limitations:</span></span>
    - <span data-ttu-id="dff13-112">Maximálna veľkosť: 8GB.</span><span class="sxs-lookup"><span data-stu-id="dff13-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="dff13-113">Nepodporovaná architektúra: zbrane.</span><span class="sxs-lookup"><span data-stu-id="dff13-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="dff13-114">Ďalšie informácie týkajúce sa týchto krokov nájdete[v téme Pridanie, priradenie a sledovanie aplikácie Win32 v službe Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add).</span><span class="sxs-lookup"><span data-stu-id="dff13-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="dff13-115">Podrobnosti o riešení problémov s nasadením aplikácií vo Windowse vrátane aplikácií Win32 je možné preskúmať v týchto dokumentoch</span><span class="sxs-lookup"><span data-stu-id="dff13-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="dff13-116">Riešenie problémov s inštaláciou aplikácie</span><span class="sxs-lookup"><span data-stu-id="dff13-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="dff13-117">Riešenie problémov s aplikáciami Win32</span><span class="sxs-lookup"><span data-stu-id="dff13-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)
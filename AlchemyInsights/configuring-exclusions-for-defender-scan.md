---
title: Konfigurácia výnimiek pre aplikáciu Microsoft Defender ATP scan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713905"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="fa107-102">Konfigurácia výnimiek pre aplikáciu Microsoft Defender ATP scan</span><span class="sxs-lookup"><span data-stu-id="fa107-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="fa107-103">Vo všeobecnosti môžete vylúčiť určité prípony súborov a umiestnenia priečinkov z kontroly ATP v programe Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="fa107-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="fa107-104">Môžete tiež nakonfigurovať vylúčenia pre súbory otvorené určitými procesmi.</span><span class="sxs-lookup"><span data-stu-id="fa107-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="fa107-105">Ďalšie informácie nájdete v téme [Konfigurácia a overenie výnimiek na základe prípony súboru a umiestnenia priečinka](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) a [Konfigurácia výnimiek pre súbory otvorené procesmi](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="fa107-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="fa107-106">Ak chcete nakonfigurovať vylúčenia pre  **Windows Server 2016 a 2019**, pozrite si tému [Konfigurácia výnimiek z antivírusového programu Microsoft Defender na Windows serveri](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="fa107-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="fa107-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="fa107-107">**Mac**</span></span>

<span data-ttu-id="fa107-108">Podrobné informácie o podporovaných typoch vylúčenia a konfigurácii zoznamu výnimiek pre Mac nájdete v téme [podporované typy vylúčenia](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) a [Konfigurovanie zoznamu výnimiek](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="fa107-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="fa107-109">**Poznámka:** Zoznamy výnimiek môžete tiež overiť pomocou skúšobného súboru EICAR.</span><span class="sxs-lookup"><span data-stu-id="fa107-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="fa107-110">Ďalšie informácie nájdete v téme [overenie zoznamov výnimiek pomocou skúšobného súboru eicar](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="fa107-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="fa107-111">**Linuxe**</span><span class="sxs-lookup"><span data-stu-id="fa107-111">**Linux**</span></span>

<span data-ttu-id="fa107-112">Podrobné informácie o podporovaných typoch vylúčenia a konfigurácii zoznamu výnimiek pre Linux nájdete v téme [podporované typy vylúčenia](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) a [Konfigurovanie a overenie výnimiek pre Microsoft Defender ATP pre Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="fa107-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="fa107-113">**Poznámka:** Zoznamy výnimiek môžete tiež overiť pomocou skúšobného súboru EICAR.</span><span class="sxs-lookup"><span data-stu-id="fa107-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="fa107-114">Ďalšie informácie nájdete v téme [overenie zoznamov výnimiek pomocou skúšobného súboru eicar](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="fa107-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 
---
title: Konfigurácia vylúčenia na Microsoft Defender ATP kontroly
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
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543700"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="9c600-102">Konfigurácia vylúčenia na Microsoft Defender ATP kontroly</span><span class="sxs-lookup"><span data-stu-id="9c600-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="9c600-103">Vo všeobecnosti môžete z kontroly vylúčiť určité prípony súborov a Microsoft Defender ATP priečinkov.</span><span class="sxs-lookup"><span data-stu-id="9c600-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="9c600-104">Môžete tiež nakonfigurovať vylúčenia pre súbory otvorené určitými procesmi.</span><span class="sxs-lookup"><span data-stu-id="9c600-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="9c600-105">Ďalšie informácie nájdete v téme Konfigurácia a overenie vylúčení na základe [prípony](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) súboru a umiestnenia priečinka a Konfigurácia vylúčení pre súbory [otvorené procesmi.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="9c600-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="9c600-106">Ak chcete nakonfigurovať vylúčenia **pre Windows Server 2016 a 2019,** pozrite si Microsoft Defender Antivirus Nastavenia vylúčenia [Windows Serveri.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="9c600-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="9c600-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="9c600-107">**Mac**</span></span>

<span data-ttu-id="9c600-108">Podrobnosti o podporovaných typoch výnimiek a konfigurácii [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) zoznamu vylúčení pre Mac nájdete v témach Podporované typy vylúčenia a Konfigurácia [zoznamu vylúčení.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="9c600-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="9c600-109">**Poznámka** Zoznamy výnimiek môžete overiť aj pomocou testovacieho súboru EICAR.</span><span class="sxs-lookup"><span data-stu-id="9c600-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="9c600-110">Ďalšie informácie nájdete v téme [Overenie zoznamov vylúčení pomocou testovacieho súboru systému EICAR.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="9c600-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="9c600-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="9c600-111">**Linux**</span></span>

<span data-ttu-id="9c600-112">Podrobnosti o podporovaných typoch výnimiek a konfigurácii [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) zoznamu vylúčení pre Linux nájdete v témach Podporované typy vylúčenia a Konfigurácia a overenie [vylúčení pre Microsoft Defender ATP Linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="9c600-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="9c600-113">**Poznámka** Zoznamy výnimiek môžete overiť aj pomocou testovacieho súboru EICAR.</span><span class="sxs-lookup"><span data-stu-id="9c600-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="9c600-114">Ďalšie informácie nájdete v téme [Overenie zoznamov vylúčení pomocou testovacieho súboru systému EICAR.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="9c600-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 
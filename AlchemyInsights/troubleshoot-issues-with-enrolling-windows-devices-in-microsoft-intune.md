---
title: Riešenie problémov s zapísať Windows zariadenia v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665847"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="9390e-102">Riešenie problémov s zapísať Windows zariadenia v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9390e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="9390e-103">Prečítajte si nižšie uvedené zdroje a vyriešte problém teraz.</span><span class="sxs-lookup"><span data-stu-id="9390e-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9390e-104">Niektoré bežné chybové hlásenia a kroky na vyriešenie:</span><span class="sxs-lookup"><span data-stu-id="9390e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="9390e-105">**Softvér nie je možné nainštalovať, 0x80cf4017:** Platnosť certifikátu vášho konta uplynula.</span><span class="sxs-lookup"><span data-stu-id="9390e-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="9390e-106">Re-download PC client softvérový balík v konzole Intune admin.</span><span class="sxs-lookup"><span data-stu-id="9390e-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="9390e-107">Prečítajte si túto dokumentáciu pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="9390e-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="9390e-108">**Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledovných prípadoch:</span><span class="sxs-lookup"><span data-stu-id="9390e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="9390e-109">Používateľ má viac zariadení zapísaných ako limit zariadenia.</span><span class="sxs-lookup"><span data-stu-id="9390e-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="9390e-110">Skontrolujte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="9390e-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="9390e-111">"Používatelia môžu pripojiť zariadenia k Azure AD" je nastavená na "none."</span><span class="sxs-lookup"><span data-stu-id="9390e-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="9390e-112">Nastavte ho na možnosť všetky alebo vyberte používateľov.</span><span class="sxs-lookup"><span data-stu-id="9390e-112">Set it to all or select users.</span></span> <span data-ttu-id="9390e-113">Prečítajte si [túto dokumentáciu](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="9390e-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="9390e-114">Zariadenie je už zapísané iným používateľom.</span><span class="sxs-lookup"><span data-stu-id="9390e-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="9390e-115">Ak je tomu tak, odstráňte zariadenie z konzoly Azure Intune alebo manuálne zrušte registráciu zariadenia pred pokusom znova.</span><span class="sxs-lookup"><span data-stu-id="9390e-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="9390e-116">Zariadenie je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="9390e-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="9390e-117">Azure Active Directory sa môže pripojiť iba Windows 10 Pro, vzdelávanie a Enterprise SKUs.</span><span class="sxs-lookup"><span data-stu-id="9390e-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="9390e-118">Ďalšie zdroje, ktoré vám pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="9390e-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="9390e-119">Použite [Intune riešenie problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné registrácie zlyhania.</span><span class="sxs-lookup"><span data-stu-id="9390e-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9390e-120">Prečítajte si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="9390e-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="9390e-121">Prečítajte si tieto dokumenty pre zoznam bežných chýb, ktoré bránia zápisu a uznesenia pre každého: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="9390e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="9390e-122">[Naučte sa, ako zapísať zariadenia Windows v Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="9390e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>

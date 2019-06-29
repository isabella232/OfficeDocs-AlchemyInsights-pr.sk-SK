---
title: Riešenie problémov s zapísať zariadenia so systémom Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353552"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="fe120-102">Riešenie problémov s zapísať zariadenia so systémom Windows Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="fe120-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="fe120-103">Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz.</span><span class="sxs-lookup"><span data-stu-id="fe120-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="fe120-104">Niektoré bežné chybové hlásenia a rozlíšenie kroky:</span><span class="sxs-lookup"><span data-stu-id="fe120-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="fe120-105">**Nemôže byť nainštalovaný softvér, 0x80cf4017:** Váš účet certifikátu skončila.</span><span class="sxs-lookup"><span data-stu-id="fe120-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="fe120-106">Re-Stiahnuť softvérový balík PC klienta v Intune Admin konzole.</span><span class="sxs-lookup"><span data-stu-id="fe120-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="fe120-107">Ďalšie informácie v tejto dokumentácii.</span><span class="sxs-lookup"><span data-stu-id="fe120-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="fe120-108">**Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledovných prípadoch:</span><span class="sxs-lookup"><span data-stu-id="fe120-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="fe120-109">Užívateľ má viac zariadení zaradených ako limit zariadenia.</span><span class="sxs-lookup"><span data-stu-id="fe120-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="fe120-110">Revidovať tieto dokumenty [Odstránenie zariadenia](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeniť limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="fe120-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="fe120-111">"Používatelia môžu pripojiť zariadenia Azure AD" je nastavený na "none".</span><span class="sxs-lookup"><span data-stu-id="fe120-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="fe120-112">Nastavte ju na všetky, alebo vybrať používateľov.</span><span class="sxs-lookup"><span data-stu-id="fe120-112">Set it to all or select users.</span></span> <span data-ttu-id="fe120-113">Prečítajte si [túto dokumentáciu](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) ďalšie informácie.</span><span class="sxs-lookup"><span data-stu-id="fe120-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="fe120-114">Zariadenie je už zaregistrovaná iným používateľom.</span><span class="sxs-lookup"><span data-stu-id="fe120-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="fe120-115">Ak je to prípad, odstrániť zariadenie z Azure Intune konzoly alebo manuálne unenroll zariadenie pred opätovným pokusom.</span><span class="sxs-lookup"><span data-stu-id="fe120-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="fe120-116">Zariadenie je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="fe120-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="fe120-117">Iba Windows 10 Pro, vzdelávanie a Enterprise SKU môžete pripojiť Azure služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fe120-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="fe120-118">Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="fe120-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="fe120-119">Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie.</span><span class="sxs-lookup"><span data-stu-id="fe120-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="fe120-120">Prečítať [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="fe120-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="fe120-121">Revidovať tieto dokumenty zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="fe120-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="fe120-122">[Naučte sa zapísať zariadenia so systémom Windows v spoločnosti Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="fe120-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>

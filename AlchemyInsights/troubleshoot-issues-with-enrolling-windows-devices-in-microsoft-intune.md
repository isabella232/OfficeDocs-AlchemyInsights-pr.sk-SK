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
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559676"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="9b5dc-102">Riešenie problémov s zapísať zariadenia so systémom Windows Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="9b5dc-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="9b5dc-103">Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9b5dc-104">Niektoré bežné chybové hlásenia a rozlíšenie kroky:</span><span class="sxs-lookup"><span data-stu-id="9b5dc-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="9b5dc-105">**Nemôže byť nainštalovaný softvér, 0x80cf4017:** Váš účet certifikátu skončila.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="9b5dc-106">Re-Stiahnuť softvérový balík PC klienta v Intune Admin konzole.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="9b5dc-107">Ďalšie informácie v tejto dokumentácii.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="9b5dc-108">**Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledovných prípadoch:</span><span class="sxs-lookup"><span data-stu-id="9b5dc-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="9b5dc-109">Užívateľ má viac zariadení zaradených ako limit zariadenia.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="9b5dc-110">Revidovať tieto dokumenty [Odstránenie zariadenia](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeniť limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="9b5dc-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="9b5dc-111">"Používatelia môžu pripojiť zariadenia Azure AD" je nastavený na "none".</span><span class="sxs-lookup"><span data-stu-id="9b5dc-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="9b5dc-112">Nastavte ju na všetky, alebo vybrať používateľov.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-112">Set it to all or select users.</span></span> <span data-ttu-id="9b5dc-113">Prečítajte si [túto dokumentáciu](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) ďalšie informácie.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="9b5dc-114">Zariadenie je už zaregistrovaná iným používateľom.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="9b5dc-115">Ak je to prípad, odstrániť zariadenie z Azure Intune konzoly alebo manuálne unenroll zariadenie pred opätovným pokusom.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="9b5dc-116">Zariadenie je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="9b5dc-117">Iba Windows 10 Pro, vzdelávanie a Enterprise SKU môžete pripojiť Azure služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="9b5dc-118">Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="9b5dc-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9b5dc-119">Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9b5dc-120">Prečítať [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="9b5dc-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="9b5dc-121">Revidovať tieto dokumenty zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="9b5dc-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="9b5dc-122">[Naučte sa zapísať zariadenia so systémom Windows v spoločnosti Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="9b5dc-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>

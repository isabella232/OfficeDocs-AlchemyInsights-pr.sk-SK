---
title: Riešenie problémov s zapísať zariadenia so systémom Windows Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29488847"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="20b06-102">Riešenie problémov s zapísať zariadenia so systémom Windows Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="20b06-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="20b06-103">Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz.</span><span class="sxs-lookup"><span data-stu-id="20b06-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="20b06-104">Niektoré bežné chybové hlásenia a rozlíšenie kroky:</span><span class="sxs-lookup"><span data-stu-id="20b06-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="20b06-p101">**Nemôže byť nainštalovaný softvér, 0x80cf4017:** Váš účet certifikátu skončila. Re-Stiahnuť softvérový balík PC klienta v Intune Admin konzole. Ďalšie informácie v tejto dokumentácii.</span><span class="sxs-lookup"><span data-stu-id="20b06-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="20b06-108">**Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledovných prípadoch:</span><span class="sxs-lookup"><span data-stu-id="20b06-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="20b06-p102">Užívateľ má viac zariadení zaradených ako limit zariadenia. Revidovať tieto dokumenty [Odstránenie zariadenia](https://docs.microsoft.com/en-us/intune/devices-wipe) alebo [zmeniť limit zariadenia](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="20b06-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="20b06-p103">"Používatelia môžu pripojiť zariadenia Azure AD" je nastavený na "none". Nastavte ju na všetky, alebo vybrať používateľov. Prečítajte si [túto dokumentáciu](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) ďalšie informácie.</span><span class="sxs-lookup"><span data-stu-id="20b06-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="20b06-p104">Zariadenie je už zaregistrovaná iným používateľom. Ak je to prípad, odstrániť zariadenie z Azure Intune konzoly alebo manuálne unenroll zariadenie pred opätovným pokusom.</span><span class="sxs-lookup"><span data-stu-id="20b06-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="20b06-p105">Zariadenie je Windows 10 Home. Iba Windows 10 Pro, vzdelávanie a Enterprise SKU môžete pripojiť Azure služby Active Directory.</span><span class="sxs-lookup"><span data-stu-id="20b06-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="20b06-118">Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="20b06-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="20b06-p106">Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie. Prečítať [Tento dokument](https://docs.microsoft.com/en-us/intune/help-desk-operators) pre ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="20b06-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="20b06-121">Revidovať tieto dokumenty zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému: [Riešenie problémov sprievodca](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [Riešenie problémov doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="20b06-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="20b06-122">[Naučte sa zapísať zariadenia so systémom Windows v spoločnosti Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="20b06-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  


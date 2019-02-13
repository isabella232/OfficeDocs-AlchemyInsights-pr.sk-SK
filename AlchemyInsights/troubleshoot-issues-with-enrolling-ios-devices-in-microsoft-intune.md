---
title: Riešenie problémov s zapísať iOS zariadení Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924783"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="0f9c1-102">Riešenie problémov s zapísať iOS zariadení Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0f9c1-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="0f9c1-103">Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz.</span><span class="sxs-lookup"><span data-stu-id="0f9c1-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="0f9c1-104">Niektoré bežné chybové hlásenia a rozlíšenie kroky:</span><span class="sxs-lookup"><span data-stu-id="0f9c1-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="0f9c1-p101">**Zariadenie SPP dosiahla** Užívateľ má viac zariadení zaradených ako limit zariadenia. Revidovať tieto dokumenty [Odstránenie zariadenia](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeniť limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="0f9c1-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="0f9c1-p102">**Táto služba nie je podporovaná. Žiadna politika Enrollment:** Apple Push oznámenia služby (APN) musí byť nakonfigurovaný alebo obnovené. Prečítať [Tento dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pre návod, ako na to.</span><span class="sxs-lookup"><span data-stu-id="0f9c1-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="0f9c1-p103">**Používateľ licenciu typu neplatný alebo meno používateľa nebol rozpoznaný:** Užívateľ musí prideliť licenciu Windows Intune alebo EMS. Revidovať tieto dokumenty priradiť licenciu prostredníctvom: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) alebo [Azure portál](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="0f9c1-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="0f9c1-111">Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="0f9c1-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0f9c1-p104">Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie. Prečítať [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="0f9c1-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="0f9c1-114">Revidovať tieto dokumenty zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="0f9c1-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="0f9c1-115">[Naučte sa registrovať iOS zariadenia Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="0f9c1-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    


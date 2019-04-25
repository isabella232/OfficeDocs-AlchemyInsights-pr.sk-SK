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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391022"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="31f79-102">Riešenie problémov s zapísať iOS zariadení Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="31f79-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="31f79-103">Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz.</span><span class="sxs-lookup"><span data-stu-id="31f79-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="31f79-104">Niektoré bežné chybové hlásenia a rozlíšenie kroky:</span><span class="sxs-lookup"><span data-stu-id="31f79-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="31f79-105">**Zariadenie SPP dosiahla** Užívateľ má viac zariadení zaradených ako limit zariadenia.</span><span class="sxs-lookup"><span data-stu-id="31f79-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="31f79-106">Revidovať tieto dokumenty [Odstránenie zariadenia](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeniť limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="31f79-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="31f79-107">**Táto služba nie je podporovaná. Žiadna politika Enrollment:** Apple Push oznámenia služby (APN) musí byť nakonfigurovaný alebo obnovené.</span><span class="sxs-lookup"><span data-stu-id="31f79-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="31f79-108">Prečítať [Tento dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) pre návod, ako na to.</span><span class="sxs-lookup"><span data-stu-id="31f79-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="31f79-109">**Používateľ licenciu typu neplatný alebo meno používateľa nebol rozpoznaný:** Užívateľ musí prideliť licenciu Windows Intune alebo EMS.</span><span class="sxs-lookup"><span data-stu-id="31f79-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="31f79-110">Revidovať tieto dokumenty priradiť licenciu prostredníctvom: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) alebo [Azure portál](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="31f79-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="31f79-111">Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="31f79-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="31f79-112">Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie.</span><span class="sxs-lookup"><span data-stu-id="31f79-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="31f79-113">Prečítať [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="31f79-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="31f79-114">Revidovať tieto dokumenty zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="31f79-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="31f79-115">[Naučte sa registrovať iOS zariadenia Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="31f79-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    


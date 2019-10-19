---
title: Riešenie problémov s zapísať iOS zariadenia v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/18/2019
ms.locfileid: "36507018"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="c57a5-102">Riešenie problémov s zapísať iOS zariadenia v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c57a5-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="c57a5-103">Prečítajte si nižšie uvedené zdroje a vyriešte problém teraz.</span><span class="sxs-lookup"><span data-stu-id="c57a5-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="c57a5-104">Niektoré bežné chybové hlásenia a kroky na vyriešenie:</span><span class="sxs-lookup"><span data-stu-id="c57a5-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="c57a5-105">**Dosiahnutá krytka zariadenia** Používateľ má viac zariadení zapísaných ako limit zariadenia.</span><span class="sxs-lookup"><span data-stu-id="c57a5-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c57a5-106">Skontrolujte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="c57a5-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="c57a5-107">**Táto služba nie je podporovaná. Žiadna politika zápisu:** Služba Apple push Notification (APNS) musí byť nakonfigurovaná alebo obnovená.</span><span class="sxs-lookup"><span data-stu-id="c57a5-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="c57a5-108">[V tomto dokumente](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) si prečítajte pokyny, ako to urobiť.</span><span class="sxs-lookup"><span data-stu-id="c57a5-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="c57a5-109">**Typ licencie používateľa neplatné alebo meno používateľa nie je rozpoznané:** Používateľ musí prideliť licenciu Intune alebo EMS.</span><span class="sxs-lookup"><span data-stu-id="c57a5-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c57a5-110">Skontrolujte tieto dokumenty a priraďte licenciu prostredníctvom: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) alebo [Azure Portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="c57a5-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="c57a5-111">Ďalšie zdroje, ktoré vám pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="c57a5-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c57a5-112">Použite [Intune riešenie problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné registrácie zlyhania.</span><span class="sxs-lookup"><span data-stu-id="c57a5-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c57a5-113">Prečítajte si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="c57a5-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="c57a5-114">Prečítajte si tieto dokumenty pre zoznam bežných chýb, ktoré bránia zápisu a uznesenia pre každého: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [Riešenie problémov doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c57a5-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="c57a5-115">[Zistite, ako zapísať zariadenia so systémom iOS do programu Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="c57a5-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    


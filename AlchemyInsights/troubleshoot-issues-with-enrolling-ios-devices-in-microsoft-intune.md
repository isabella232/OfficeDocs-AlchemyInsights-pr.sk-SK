---
title: Riešenie problémov s zaregistrovaním zariadení so systémom iOS v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823478"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="e8271-102">Riešenie problémov s zaregistrovaním zariadení so systémom iOS v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e8271-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="e8271-103">Ak chcete problém vyriešiť, pozrite si zdroje uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="e8271-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="e8271-104">Niektoré bežné chybové hlásenia a kroky na riešenie tohto problémov:</span><span class="sxs-lookup"><span data-stu-id="e8271-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="e8271-105">**Dosiahol sa kryt zariadenia** Používateľ má zaregistrovaných viac zariadení, ako je limit zariadení.</span><span class="sxs-lookup"><span data-stu-id="e8271-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e8271-106">Skontrolujte tieto dokumenty a [odstráňte zariadenie alebo](https://docs.microsoft.com/intune/devices-wipe) zmeňte limit [zariadení.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="e8271-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="e8271-107">**Táto služba nie je podporovaná. Žiadna politika registrácie: Službu** spoločnosti Apple Push Notification Service (APNS) je potrebné nakonfigurovať alebo obnoviť.</span><span class="sxs-lookup"><span data-stu-id="e8271-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="e8271-108">V [tomto dokumente](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) nájdete pokyny, ako to urobiť.</span><span class="sxs-lookup"><span data-stu-id="e8271-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="e8271-109">**Typ používateľskej licencie Neplatný alebo Meno používateľa sa nerozpoznalo:** Používateľovi je potrebné priradiť licenciu na Intune alebo EMS.</span><span class="sxs-lookup"><span data-stu-id="e8271-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e8271-110">Ak chcete priradiť licenciu, pozrite si tieto dokumenty: [Centrum spravovania balíka Office](https://docs.microsoft.com/intune/licenses-assign) alebo portál [Azure.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="e8271-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="e8271-111">Ďalšie zdroje informácií na vyriešenie problému:</span><span class="sxs-lookup"><span data-stu-id="e8271-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e8271-112">Pomocou [portálu na riešenie problémov služby Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) môžete diagnostikovať a vyriešiť bežné zlyhania registrácie.</span><span class="sxs-lookup"><span data-stu-id="e8271-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e8271-113">Ďalšie [podrobnosti nájdete](https://docs.microsoft.com/intune/help-desk-operators) v tomto dokumente.</span><span class="sxs-lookup"><span data-stu-id="e8271-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="e8271-114">V týchto dokumentoch nájdete zoznam bežných chýb, ktoré v každej z nich bránia registrácii a riešeniam: Príručka na [riešenie problémov](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a Riešenie problémov [s dokumentom.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="e8271-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="e8271-115">[Zistite, ako zaregistrovať zariadenia so systémom iOS v Microsoft Intune.](https://docs.microsoft.com/intune/ios-enroll)</span><span class="sxs-lookup"><span data-stu-id="e8271-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    


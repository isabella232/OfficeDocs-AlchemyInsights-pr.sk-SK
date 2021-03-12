---
title: Riešenie problémov s zaregistrovaním zariadení so systémom iOS v službe Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708977"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="14264-102">Riešenie problémov s zaregistrovaním zariadení so systémom iOS v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="14264-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="14264-103">Ak chcete problém vyriešiť, prečítajte si zdroje uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="14264-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="14264-104">Niektoré bežné chybové hlásenia a kroky na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="14264-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="14264-105">**Dosiahli ste uzáver zariadenia** Používateľ má viac zariadení zaregistrovaných ako limit zariadenia.</span><span class="sxs-lookup"><span data-stu-id="14264-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="14264-106">Preskúmajte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="14264-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="14264-107">**Táto služba nie je podporovaná. Žiadna politika registrácie:** službu Apple push Notification Service (APNS) je potrebné nakonfigurovať alebo obnoviť.</span><span class="sxs-lookup"><span data-stu-id="14264-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="14264-108">Pozrite si [Tento dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) a postupujte podľa pokynov.</span><span class="sxs-lookup"><span data-stu-id="14264-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="14264-109">**Typ licencie používateľa je neplatný alebo sa nerozpoznalo meno používateľa:** Používateľ musí mať priradenú licenciu služby Intune alebo EMS.</span><span class="sxs-lookup"><span data-stu-id="14264-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="14264-110">Pozrite si tieto dokumenty a priraďte licenciu: [centrum spravovania služieb Office](https://docs.microsoft.com/intune/licenses-assign) alebo [portál Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="14264-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="14264-111">Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="14264-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="14264-112">Použite [portál na riešenie problémov so službou Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) na diagnostikovanie a riešenie bežných zlyhaní registrácie.</span><span class="sxs-lookup"><span data-stu-id="14264-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="14264-113">Pozrite si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) a získajte ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="14264-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="14264-114">Pozrite si tieto dokumenty, kde nájdete zoznam bežných chýb, ktoré bránia každej registrácii a rozlíšeniam: [príručka na riešenie problémov](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [dokument na riešenie problémov](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="14264-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="14264-115">[Zistite, ako zapísať zariadenia so systémom iOS do služby Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="14264-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    


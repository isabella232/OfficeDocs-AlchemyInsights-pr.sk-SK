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
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669263"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="85ac1-102">Riešenie problémov s zaregistrovaním zariadení so systémom iOS v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="85ac1-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="85ac1-103">Ak chcete problém vyriešiť, prečítajte si zdroje uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="85ac1-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="85ac1-104">Niektoré bežné chybové hlásenia a kroky na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="85ac1-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="85ac1-105">**Dosiahli ste uzáver zariadenia** Používateľ má viac zariadení zaregistrovaných ako limit zariadenia.</span><span class="sxs-lookup"><span data-stu-id="85ac1-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="85ac1-106">Preskúmajte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="85ac1-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="85ac1-107">**Táto služba nie je podporovaná. Žiadna politika registrácie:** službu Apple push Notification Service (APNS) je potrebné nakonfigurovať alebo obnoviť.</span><span class="sxs-lookup"><span data-stu-id="85ac1-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="85ac1-108">Pozrite si [Tento dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) a postupujte podľa pokynov.</span><span class="sxs-lookup"><span data-stu-id="85ac1-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="85ac1-109">**Typ licencie používateľa je neplatný alebo sa nerozpoznalo meno používateľa:** Používateľ musí mať priradenú licenciu služby Intune alebo EMS.</span><span class="sxs-lookup"><span data-stu-id="85ac1-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="85ac1-110">Pozrite si tieto dokumenty a priraďte licenciu: [centrum spravovania služieb Office](https://docs.microsoft.com/intune/licenses-assign) alebo [portál Azure](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="85ac1-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="85ac1-111">Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="85ac1-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="85ac1-112">Použite [portál na riešenie problémov so službou Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) na diagnostikovanie a riešenie bežných zlyhaní registrácie.</span><span class="sxs-lookup"><span data-stu-id="85ac1-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="85ac1-113">Pozrite si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) a získajte ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="85ac1-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="85ac1-114">Pozrite si tieto dokumenty, kde nájdete zoznam bežných chýb, ktoré bránia každej registrácii a rozlíšeniam: [príručka na riešenie problémov](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [dokument na riešenie problémov](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="85ac1-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="85ac1-115">[Zistite, ako zapísať zariadenia so systémom iOS do služby Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="85ac1-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    


---
title: Riešenie problémov s zaregistrovaním zariadení s Androidom v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830957"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="747be-102">Riešenie problémov s zaregistrovaním zariadení s Androidom v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="747be-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="747be-103">Ak chcete problém vyriešiť, pozrite si zdroje uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="747be-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="747be-104">Niektoré bežné problémy a kroky na riešenie:</span><span class="sxs-lookup"><span data-stu-id="747be-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="747be-105">**Chyba Zariadenia nie je šifrovaná na portáli spoločnosti:** Novšie verzie Androidu, najmä verzie v7.0, vyžadujú prístupový kód na spustenie, aby bolo zariadenie plne šifrované.</span><span class="sxs-lookup"><span data-stu-id="747be-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="747be-106">Bežnými riešeniami sú zapnutie špendlíka pri spustení alebo úplné šifrovanie zariadenia.</span><span class="sxs-lookup"><span data-stu-id="747be-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="747be-107">Ďalšie [informácie nájdete](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) v tomto dokumente.</span><span class="sxs-lookup"><span data-stu-id="747be-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="747be-108">Zariadenia sa nedokážu pozrieť do služby Intune alebo sa v správcovskej konzole služby **Intune zobrazujú ako Nepovhodné:** Niektoré zariadenia Samsung 4.4 a 5.5 nemusia službu kontrolovať.</span><span class="sxs-lookup"><span data-stu-id="747be-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="747be-109">K dispozícii sú 3 možné riešenia tohto problému:</span><span class="sxs-lookup"><span data-stu-id="747be-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="747be-110">Manuálne otvorte aplikáciu Intune Company Portal, ktorá automaticky spustí synchronizáciu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="747be-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="747be-111">Aktualizujte zariadenie na Android 6.0 alebo jeho vyššiu verziu.</span><span class="sxs-lookup"><span data-stu-id="747be-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="747be-112">Zakážte aplikácii Samsung Smart Manager spravovanie portálu Intune Company Portal.</span><span class="sxs-lookup"><span data-stu-id="747be-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="747be-113">V [tomto dokumente](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) nájdete ďalšie podrobnosti o týchto problémoch a riešeniach.</span><span class="sxs-lookup"><span data-stu-id="747be-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="747be-114">**Chyba typu používateľskej** licencie Neplatný alebo Meno používateľa sa nerozpoznalo: Používateľovi je potrebné priradiť licenciu na Intune alebo EMS. </span><span class="sxs-lookup"><span data-stu-id="747be-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="747be-115">Ak chcete priradiť licenciu, pozrite si tieto dokumenty: Centrum spravovania balíka Office alebo portál Azure.</span><span class="sxs-lookup"><span data-stu-id="747be-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="747be-116">Ďalšie zdroje informácií na vyriešenie problému:</span><span class="sxs-lookup"><span data-stu-id="747be-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="747be-117">Pomocou [portálu na riešenie problémov služby Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) môžete diagnostikovať a vyriešiť bežné zlyhania registrácie.</span><span class="sxs-lookup"><span data-stu-id="747be-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="747be-118">Ďalšie [podrobnosti nájdete](https://docs.microsoft.com/intune/help-desk-operators) v tomto dokumente.</span><span class="sxs-lookup"><span data-stu-id="747be-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="747be-119">V [tomto dokumente](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) sa nachádza zoznam bežných chýb, ktoré bránia registrácii a riešeniam jednotlivých chýb.</span><span class="sxs-lookup"><span data-stu-id="747be-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="747be-120">[Zistite, ako zaregistrovať zariadenia s Androidom v Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)</span><span class="sxs-lookup"><span data-stu-id="747be-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>

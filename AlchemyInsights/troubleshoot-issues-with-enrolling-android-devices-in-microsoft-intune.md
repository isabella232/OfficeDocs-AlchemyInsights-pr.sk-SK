---
title: Riešenie problémov s zaregistrovaním zariadení s Androidom v službe Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689969"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="3b5a7-102">Riešenie problémov s zaregistrovaním zariadení s Androidom v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3b5a7-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="3b5a7-103">Ak chcete problém vyriešiť, prečítajte si zdroje uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="3b5a7-104">Niektoré bežné problémy a kroky na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="3b5a7-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="3b5a7-105">**Chyba zariadenia nie je šifrovaná na portáli spoločnosti:** Novšie verzie Androidu, najmä počnúc v 7.0, vyžadujú prístupový kód pri spustení, aby ste sa uistili, že vaše zariadenie je plne zašifrované.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="3b5a7-106">Bežné riešenia umožňujú spustenie PIN kódu alebo úplné zašifrovanie zariadenia.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="3b5a7-107">Pozrite si [Tento dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) a získajte ďalšie informácie.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="3b5a7-108">**Zariadenia sa nedokážu vrátiť do projektu so službou Intune alebo Zobraziť ako nezdravé v konzole správcu služby Intune:** Niektoré zariadenia Samsung 4,4 a 5,5 sa nemusia vrátiť do služby.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="3b5a7-109">K dispozícii sú 3 možné riešenia tohto problému:</span><span class="sxs-lookup"><span data-stu-id="3b5a7-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="3b5a7-110">Manuálne otvorte aplikáciu Intune Company Portal, ktorou sa automaticky spustí Synchronizácia zariadenia.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="3b5a7-111">Aktualizujte zariadenie na Android 6,0 alebo novšiu verziu.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="3b5a7-112">Vypnutie aplikácie Samsung Smart Manager na spravovanie portálu spoločnosti Intune.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="3b5a7-113">Pozrite si [Tento dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) a získajte ďalšie podrobnosti o týchto problémoch a rozlíšeniach.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="3b5a7-114">**Typ licencie používateľa neplatný** alebo **meno používateľa sa nerozpoznala chyba:** používateľ musí mať priradenú licenciu služby Intune alebo EMS.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="3b5a7-115">Pozrite si tieto dokumenty a priraďte licenciu: centrum spravovania služieb Office alebo portál Azure.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="3b5a7-116">Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="3b5a7-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="3b5a7-117">Použite [portál na riešenie problémov so službou Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) na diagnostikovanie a riešenie bežných zlyhaní registrácie.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3b5a7-118">Pozrite si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) a získajte ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="3b5a7-119">Pozrite si [Tento dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) so zoznamom bežných chýb, ktoré zabránia zápisu a rozlíšeniam.</span><span class="sxs-lookup"><span data-stu-id="3b5a7-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="3b5a7-120">[Zistite, ako prihlásiť zariadenia s Androidom v službe Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="3b5a7-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>

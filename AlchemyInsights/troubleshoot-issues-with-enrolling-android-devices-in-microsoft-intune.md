---
title: Riešenie problémov s zapísať Android zariadenia v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759635"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="1f1d9-102">Riešenie problémov s zapísať Android zariadenia v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="1f1d9-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="1f1d9-103">Prečítajte si nižšie uvedené zdroje a vyriešte problém teraz.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="1f1d9-104">Niektoré bežné problémy a kroky riešenia:</span><span class="sxs-lookup"><span data-stu-id="1f1d9-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="1f1d9-105">**Zariadenie nie je šifrovaná chyba v portáli spoločnosti:** Novšie verzie Androidu, najmä počnúc v 7.0, vyžadujú spúšťací prístupový kód, aby ste sa uistili, že vaše zariadenie je úplne šifrované.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="1f1d9-106">Bežné riešenia sú umožňujúce spúšťací kód PIN alebo úplne zašifrovať zariadenie.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="1f1d9-107">Ďalšie informácie si prečítajte [v tomto dokumente](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .</span><span class="sxs-lookup"><span data-stu-id="1f1d9-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="1f1d9-108">**Zariadenia nepodarí overiť pomocou služby Intune alebo Zobraziť ako "nezdravé" v konzole správcu Intune:** Niektoré zariadenia Samsung 4,4 a 5,5 nemusia do služby kontrolovať.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="1f1d9-109">Existujú 3 možné riešenia tohto problému:</span><span class="sxs-lookup"><span data-stu-id="1f1d9-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="1f1d9-110">Manuálne otvorte aplikáciu Intune Company Portal, ktorá automaticky spustí synchronizáciu zariadenia.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="1f1d9-111">Aktualizujte zariadenie na Android 6,0 alebo novší.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="1f1d9-112">Zakážte Samsung Smart Manager Spravovanie portálu Intune spoločnosti.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="1f1d9-113">Prečítajte si [Tento dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pre ďalšie podrobnosti o týchto otázkach a uzneseniach.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="1f1d9-114">**Typ licencie používateľa neplatné** alebo **meno používateľa nie je rozpoznaná chyba:** používateľ musí prideliť licenciu Intune alebo EMS.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="1f1d9-115">Skontrolujte tieto dokumenty a priraďte licenciu prostredníctvom: Office Admin Center alebo Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="1f1d9-116">Ďalšie zdroje, ktoré vám pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="1f1d9-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="1f1d9-117">Použite [Intune riešenie problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné registrácie zlyhania.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="1f1d9-118">Prečítajte si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="1f1d9-119">Skontrolujte [Tento dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pre zoznam bežných chýb, ktoré zabraňujú zápisu a rozlíšeniu.</span><span class="sxs-lookup"><span data-stu-id="1f1d9-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="1f1d9-120">[Naučte sa, ako zapísať zariadenia Android v Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="1f1d9-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>

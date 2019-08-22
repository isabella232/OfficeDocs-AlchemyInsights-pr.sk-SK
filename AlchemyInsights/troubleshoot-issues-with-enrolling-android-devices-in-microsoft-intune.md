---
title: Riešenie problémov s zapísať Android zariadení Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500086"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="d6ae7-102">Riešenie problémov s zapísať Android zariadení Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d6ae7-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="d6ae7-103">Preskúmanie zdrojov uvedených nižšie vyriešiť váš problém teraz.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="d6ae7-104">Niektoré spoločné problémy a rozlíšenie kroky:</span><span class="sxs-lookup"><span data-stu-id="d6ae7-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="d6ae7-105">**Zariadenia nie sú šifrované chyba v portáli spoločnosti:** Novšie verzie Androidu, najmä počnúc v7.0, požadovať heslo pri spustení uistite sa, že vaše zariadenie je plne šifrované.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="d6ae7-106">Povolenie kódu pin pri spustení alebo plne šifrovanie zariadenia sa spoločné riešenia.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="d6ae7-107">Prečítať [Tento dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) pre ďalšie informácie.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="d6ae7-108">**Zariadenia nedokážu skontrolovať pomocou služby Windows Intune alebo Zobraziť ako "Nezdravých" Intune admin konzole:** Niektoré Samsung 4.4 a 5,5 zariadenia môže skontrolovať do služby.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="d6ae7-109">Existujú 3 možné riešenia tohto problému:</span><span class="sxs-lookup"><span data-stu-id="d6ae7-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="d6ae7-110">Manuálne otvorenie aplikácie portáli spoločnosti Intune, ktorý sa automaticky spustí Synchronizácia zariadenia.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="d6ae7-111">Aktualizujte zariadenie na Android 6.0 alebo vyšší.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="d6ae7-112">Zakázať riadenie portáli Intune spoločnosti Samsung Smart Manager.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="d6ae7-113">Prečítať [Tento dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) pre ďalšie podrobnosti o týchto otázkach a uznesenia.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="d6ae7-114">**Užívateľ licencie typu neplatný** alebo **užívateľské meno nerozpozná chyba:** užívateľ musí prideliť licenciu Windows Intune alebo EMS.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="d6ae7-115">Revidovať tieto dokumenty priradiť licenciu prostredníctvom: Office Admin Center alebo Azure portál.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="d6ae7-116">Dodatočné zdroje, ktoré pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="d6ae7-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="d6ae7-117">Používajte [Windows Intune riešenia problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhania registrácie.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d6ae7-118">Prečítať [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) pre ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="d6ae7-119">Prečítať [Tento dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) pre zoznam bežných chýb, ktoré bránia zápisnice a uznesenia každému.</span><span class="sxs-lookup"><span data-stu-id="d6ae7-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="d6ae7-120">[Naučte sa zapísať Android zariadení Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="d6ae7-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>

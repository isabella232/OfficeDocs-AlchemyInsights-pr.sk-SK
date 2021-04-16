---
title: Riešenie problémov s zaregistrovaním zariadení s Windowsom v Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808986"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="0c4e6-102">Riešenie problémov s zaregistrovaním zariadení s Windowsom v Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="0c4e6-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="0c4e6-103">Ak chcete problém vyriešiť, pozrite si zdroje uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="0c4e6-104">Niektoré bežné chybové hlásenia a kroky na riešenie tohto problémov:</span><span class="sxs-lookup"><span data-stu-id="0c4e6-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="0c4e6-105">**Softvér nie je možné nainštalovať, 0x80cf4017:** Platnosť certifikátu konta uplynula.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="0c4e6-106">Znova si stiahnite softvérový balík PC Client v správcovskej konzole služby Intune.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="0c4e6-107">Ďalšie informácie nájdete v tejto dokumentácii.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="0c4e6-108">**Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledujúcich scenároch:</span><span class="sxs-lookup"><span data-stu-id="0c4e6-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="0c4e6-109">Používateľ má zaregistrovaných viac zariadení, ako je limit zariadení.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="0c4e6-110">Skontrolujte tieto dokumenty a [odstráňte zariadenie alebo](https://docs.microsoft.com/intune/devices-wipe) zmeňte limit [zariadení.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="0c4e6-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="0c4e6-111">Možnosť Používatelia môžu pripojiť zariadenia k službe Azure AD je nastavená na možnosť žiadne.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="0c4e6-112">Nastavte ho všetkým alebo vyberte používateľov.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-112">Set it to all or select users.</span></span> <span data-ttu-id="0c4e6-113">Ďalšie [informácie nájdete v](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) tejto dokumentácii.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="0c4e6-114">Zariadenie už zaregistroval iný používateľ.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="0c4e6-115">V takom prípade zariadenie odstráňte z konzoly služby Azure Intune alebo pred zopakovaním pokusu manuálne zariadenie znova zaregistrujte.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="0c4e6-116">Zariadenie je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="0c4e6-117">Do služby Azure Active Directory sa môžu pripojiť iba SKU Windowsu 10 Pro, Education a Enterprise.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="0c4e6-118">Ďalšie zdroje informácií na vyriešenie problému:</span><span class="sxs-lookup"><span data-stu-id="0c4e6-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="0c4e6-119">Pomocou [portálu na riešenie problémov služby Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) môžete diagnostikovať a vyriešiť bežné zlyhania registrácie.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0c4e6-120">Ďalšie [podrobnosti nájdete](https://docs.microsoft.com/intune/help-desk-operators) v tomto dokumente.</span><span class="sxs-lookup"><span data-stu-id="0c4e6-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="0c4e6-121">V týchto dokumentoch nájdete zoznam bežných chýb, ktoré v každej z nich bránia registrácii a riešeniam: Príručka na [riešenie problémov](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a Riešenie problémov [s dokumentom.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="0c4e6-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="0c4e6-122">[Zistite, ako zaregistrovať zariadenia s Windowsom v Microsoft Intune.](https://docs.microsoft.com/intune/windows-enroll)</span><span class="sxs-lookup"><span data-stu-id="0c4e6-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>

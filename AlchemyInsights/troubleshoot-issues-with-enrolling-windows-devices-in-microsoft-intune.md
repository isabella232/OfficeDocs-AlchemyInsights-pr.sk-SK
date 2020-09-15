---
title: Riešenie problémov s zaregistrovaním zariadení s Windowsom v službe Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658893"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="8d4b7-102">Riešenie problémov s zaregistrovaním zariadení s Windowsom v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8d4b7-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="8d4b7-103">Ak chcete problém vyriešiť, prečítajte si zdroje uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="8d4b7-104">Niektoré bežné chybové hlásenia a kroky na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="8d4b7-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="8d4b7-105">**Softvér nie je možné nainštalovať, 0x80cf4017:** Platnosť certifikátu konta uplynula.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="8d4b7-106">Opätovné stiahnutie balíka klientskeho softvéru PC v konzole správcu služby Intune.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="8d4b7-107">Ďalšie informácie nájdete v tejto dokumentácii.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="8d4b7-108">**Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledujúcich prípadoch:</span><span class="sxs-lookup"><span data-stu-id="8d4b7-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="8d4b7-109">Používateľ má viac zariadení zaregistrovaných ako limit zariadenia.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="8d4b7-110">Preskúmajte tieto dokumenty a [odstráňte zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo [zmeňte limit zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="8d4b7-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="8d4b7-111">"Používatelia sa môžu pripájať k zariadeniam Azure AD" je nastavená na hodnotu "none" (žiadne).</span><span class="sxs-lookup"><span data-stu-id="8d4b7-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="8d4b7-112">Nastavte ju na možnosť všetci alebo vyberte položku Používatelia.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-112">Set it to all or select users.</span></span> <span data-ttu-id="8d4b7-113">Ďalšie informácie nájdete v [tejto dokumentácii](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="8d4b7-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="8d4b7-114">Zariadenie je už zaregistrované iným používateľom.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="8d4b7-115">Ak ide o tento prípad, odstráňte zariadenie zo služby Azure Intune Console alebo manuálne zrušte registráciu zariadenia pred opätovným pokusom.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="8d4b7-116">Zariadenie je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="8d4b7-117">K službe Azure Active Directory sa môžu pridať len Windows 10 Pro, Education a Enterprise SKU.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="8d4b7-118">Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="8d4b7-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="8d4b7-119">Použite [portál na riešenie problémov so službou Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) na diagnostikovanie a riešenie bežných zlyhaní registrácie.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="8d4b7-120">Pozrite si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) a získajte ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="8d4b7-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="8d4b7-121">Pozrite si tieto dokumenty, kde nájdete zoznam bežných chýb, ktoré bránia každej registrácii a rozlíšeniam: [príručka na riešenie problémov](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a [dokument na riešenie problémov](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="8d4b7-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="8d4b7-122">[Zistite, ako sa prihlásiť do zariadení s Windowsom v službe Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="8d4b7-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>

---
title: Riešenie problémov s registráciou zariadení s Windowsom v službe Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665847"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="3d629-102">Riešenie problémov s registráciou zariadení s Windowsom v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="3d629-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="3d629-103">Skontrolujte zdroje uvedené nižšie a teraz vyriešte problém.</span><span class="sxs-lookup"><span data-stu-id="3d629-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="3d629-104">Niektoré bežné chybové hlásenia a kroky riešenia:</span><span class="sxs-lookup"><span data-stu-id="3d629-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="3d629-105">**Softvér sa nedá nainštalovať, 0x80cf4017:** Platnosť certifikátu konta uplynula.</span><span class="sxs-lookup"><span data-stu-id="3d629-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="3d629-106">Znova prevezmite softvérový balík pc client v konzole Intune Admin Console.</span><span class="sxs-lookup"><span data-stu-id="3d629-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="3d629-107">Ďalšie informácie nájdete v tejto dokumentácii.</span><span class="sxs-lookup"><span data-stu-id="3d629-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="3d629-108">**Kód chyby 0x801c0003:** Chyba sa môže vyskytnúť v nasledujúcich situáciách:</span><span class="sxs-lookup"><span data-stu-id="3d629-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="3d629-109">Používateľ má viac zariadení zaregistrovaných ako limit zariadenia.</span><span class="sxs-lookup"><span data-stu-id="3d629-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="3d629-110">Skontrolujte tieto dokumenty, ak [chcete odstrániť zariadenie](https://docs.microsoft.com/intune/devices-wipe) alebo zmeniť limit [zariadenia](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="3d629-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="3d629-111">"Používatelia môžu pripojiť zariadenia Azure AD" je nastavená na "none."</span><span class="sxs-lookup"><span data-stu-id="3d629-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="3d629-112">Nastavte ho na všetkých alebo vyberte používateľov.</span><span class="sxs-lookup"><span data-stu-id="3d629-112">Set it to all or select users.</span></span> <span data-ttu-id="3d629-113">Ďalšie informácie nájdete v [tejto dokumentácii.](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)</span><span class="sxs-lookup"><span data-stu-id="3d629-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="3d629-114">Zariadenie už zapísal iný používateľ.</span><span class="sxs-lookup"><span data-stu-id="3d629-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="3d629-115">Ak je to tak, odstráňte zariadenie z konzoly Azure Intune alebo manuálne zrušte registráciu zariadenia pred pokusom znova.</span><span class="sxs-lookup"><span data-stu-id="3d629-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="3d629-116">Zariadenie je Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="3d629-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="3d629-117">Iba Windows 10 Pro, Education a Enterprise SKU sa môžu pripojiť azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3d629-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="3d629-118">Ďalšie zdroje informácií, ktoré vám pomôžu vyriešiť váš problém:</span><span class="sxs-lookup"><span data-stu-id="3d629-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="3d629-119">Použite [Intune riešenie problémov portál](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) diagnostikovať a vyriešiť bežné zlyhanie registrácie.</span><span class="sxs-lookup"><span data-stu-id="3d629-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="3d629-120">Ďalšie podrobnosti [nájdete v tomto dokumente.](https://docs.microsoft.com/intune/help-desk-operators)</span><span class="sxs-lookup"><span data-stu-id="3d629-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="3d629-121">Skontrolujte tieto dokumenty pre zoznam bežných chýb, ktoré bránia registrácii a riešenia pre každý: [Riešenie problémov sprievodca](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) a Riešenie problémov [doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="3d629-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="3d629-122">[Zistite, ako zapísať zariadenia so systémom Windows v službe Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="3d629-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>

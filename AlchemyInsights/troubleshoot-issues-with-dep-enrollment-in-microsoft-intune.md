---
title: Riešenie problémov so zápisom funkcie Zamedzenie spustenia údajov v službe Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d32afde-47ab-4b1e-a669-662e5dbdc213
ms.custom:
- "783"
- "6200002"
ms.openlocfilehash: 50aab6e1e3c0d74d2e305e0bdd47c92b3a27c79f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797311"
---
# <a name="troubleshoot-issues-with-dep-enrollment-in-microsoft-intune"></a><span data-ttu-id="d9698-102">Riešenie problémov so zápisom funkcie Zamedzenie spustenia údajov v službe Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d9698-102">Troubleshoot issues with DEP enrollment in Microsoft Intune</span></span>

<span data-ttu-id="d9698-103">Ak chcete problém vyriešiť, prečítajte si zdroje uvedené nižšie.</span><span class="sxs-lookup"><span data-stu-id="d9698-103">Review the resources listed below to resolve your issue now.</span></span>
  
1. <span data-ttu-id="d9698-104">Ak sa zariadenie na zabránenie spusteniu údajov nedá zaregistrovať a MFA (viacnásobné overovanie) je zapnuté, zakážte MFA.</span><span class="sxs-lookup"><span data-stu-id="d9698-104">If DEP device is unable to enroll and MFA (Multi-Factor Authentication) is enabled, please disable MFA.</span></span> <span data-ttu-id="d9698-105">V súčasnosti MFA nie je podporovaná pre registráciu funkciou zamedzenie spustenia údajov</span><span class="sxs-lookup"><span data-stu-id="d9698-105">Currently MFA is not supported for DEP enrollment</span></span>

2. <span data-ttu-id="d9698-106">Použite [portál na riešenie problémov so službou Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) na diagnostikovanie a riešenie bežných zlyhaní registrácie.</span><span class="sxs-lookup"><span data-stu-id="d9698-106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="d9698-107">Pozrite si [Tento dokument](https://docs.microsoft.com/intune/help-desk-operators) a získajte ďalšie podrobnosti.</span><span class="sxs-lookup"><span data-stu-id="d9698-107">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

3. <span data-ttu-id="d9698-108">Pozrite si tieto dokumenty, kde nájdete zoznam bežných chýb, ktoré bránia každej registrácii a rozlíšeniam: [príručka na riešenie problémov](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) a [dokument na riešenie problémov](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span><span class="sxs-lookup"><span data-stu-id="d9698-108">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)</span></span>

4. <span data-ttu-id="d9698-109">[Ďalšie informácie o programe registrácie zariadení](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span><span class="sxs-lookup"><span data-stu-id="d9698-109">[Learn about device enrollment program](https://docs.microsoft.com/intune/device-enrollment-program-enroll-ios).</span></span>

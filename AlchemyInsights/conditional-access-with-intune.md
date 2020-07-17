---
title: Podmienený prístup pomocou služby Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: f852d3646b8e5b2c0fce15055daf59c801fb8240
ms.sourcegitcommit: 7a1ff0314df06e386f32a2439fe060baa480e8f8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/30/2020
ms.locfileid: "44931451"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="a0b0a-102">Podmienený prístup pomocou služby Intune</span><span class="sxs-lookup"><span data-stu-id="a0b0a-102">Conditional Access with Intune</span></span>

<span data-ttu-id="a0b0a-103">Použitie **podmieneného prístupu** pomocou služby Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="a0b0a-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="a0b0a-104">Vytvorte **politiku súladu** ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android), [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios), [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) na definovanie nastavení, ktoré musia byť splnené pred tým, ako sa zariadenie považuje za kompatibilné.</span><span class="sxs-lookup"><span data-stu-id="a0b0a-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="a0b0a-105">Zariadenie musí mať napríklad špendlík s číslom najmenej 6 číslic predtým, ako sa považuje za vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="a0b0a-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="a0b0a-106">Vytvorte **politiku podmieneného prístupu,** ktorá definuje, ktoré zdroje sú chránené a aké podmienky je potrebné splniť na prístup k týmto prostriedkom.</span><span class="sxs-lookup"><span data-stu-id="a0b0a-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="a0b0a-107">[Zariadenie](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) musí byť napríklad kompatibilné pred prístupom k podnikovým e-mailom.</span><span class="sxs-lookup"><span data-stu-id="a0b0a-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="a0b0a-108">Zabezpečte, aby boli **politiky súladu** aj **politiky podmieneného prístupu** zacielené na požadované skupiny používateľov.</span><span class="sxs-lookup"><span data-stu-id="a0b0a-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="a0b0a-109">To môže vyžadovať vytvorenie konkrétnych skupín používateľov v službe Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a0b0a-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="a0b0a-110">**Užitočné odkazy:**</span><span class="sxs-lookup"><span data-stu-id="a0b0a-110">**Helpful links:**</span></span>

[<span data-ttu-id="a0b0a-111">Prehľad súladu zariadenia</span><span class="sxs-lookup"><span data-stu-id="a0b0a-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="a0b0a-112">Riešenie problémov CA</span><span class="sxs-lookup"><span data-stu-id="a0b0a-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="a0b0a-113">Politika riešenia problémov</span><span class="sxs-lookup"><span data-stu-id="a0b0a-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="a0b0a-114">Na ochranu e-mailu (Exchange online) pred prístupom nevyhovujúcich zariadení, oba dokumenty musia byť dodržiavané:</span><span class="sxs-lookup"><span data-stu-id="a0b0a-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="a0b0a-115">Ochrana prístupu k e-mailu zo zariadení pomocou EAs</span><span class="sxs-lookup"><span data-stu-id="a0b0a-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="a0b0a-116">Chráňte prístup k e-mailom zo zariadení pomocou moderných klientov overovania, ako je napríklad Outlook</span><span class="sxs-lookup"><span data-stu-id="a0b0a-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)
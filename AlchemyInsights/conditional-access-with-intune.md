---
title: Podmienený prístup so službou Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 5eec5982118b4f0246afadf2af219b2d5f32f95c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807674"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="bf7b6-102">Podmienený prístup so službou Intune</span><span class="sxs-lookup"><span data-stu-id="bf7b6-102">Conditional Access with Intune</span></span>

<span data-ttu-id="bf7b6-103">Používanie  **podmieneného prístupu**  so službou Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="bf7b6-103">Using  **Conditional Access**  with Intune requires 3 steps:</span></span>

- <span data-ttu-id="bf7b6-104">Vytvorte  **politiku dodržiavania súladu**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) a definujte nastavenia, ktoré je potrebné splniť pred tým, ako sa zariadenie považuje za vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="bf7b6-104">Create a  **Compliance Policy**  ([Android](https://docs.microsoft.com/intune/compliance-policy-create-android),  [iOS](https://docs.microsoft.com/intune/compliance-policy-create-ios),  [Windows](https://docs.microsoft.com//intune/compliance-policy-create-windows)) to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="bf7b6-105">Zariadenie musí mať napríklad PIN kód aspoň 6 číslic, kým sa považuje za vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="bf7b6-105">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>
- <span data-ttu-id="bf7b6-106">Vytvorenie **politiky podmieneného prístupu**  , ktorá definuje, aké zdroje sú chránené, a aké podmienky je potrebné splniť na prístup k týmto zdrojom.</span><span class="sxs-lookup"><span data-stu-id="bf7b6-106">Create a **Conditional Access Policy**  that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span>  <span data-ttu-id="bf7b6-107">Zariadenie musí byť [napríklad](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies) kompatibilné pred prístupom k podnikovému e-mailu.</span><span class="sxs-lookup"><span data-stu-id="bf7b6-107">[For example,](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)  a device must be compliant before accessing corporate email.</span></span>
- <span data-ttu-id="bf7b6-108">Zabezpečte, aby **politiky dodržiavania súladu**  a  **politiky podmieneného prístupu**  boli zacielené na požadované skupiny používateľov.</span><span class="sxs-lookup"><span data-stu-id="bf7b6-108">Ensure both **Compliance Policies**  and  **Conditional Access Policies**  are targeted to the desired groups of users.</span></span> <span data-ttu-id="bf7b6-109">Môže to vyžadovať vytvorenie konkrétnych skupín používateľov v službe Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="bf7b6-109">This may require creating specific groups of users in Azure Active Directory.</span></span>

<span data-ttu-id="bf7b6-110">**Užitočné prepojenia:**</span><span class="sxs-lookup"><span data-stu-id="bf7b6-110">**Helpful links:**</span></span>

[<span data-ttu-id="bf7b6-111">Prehľad súladu zariadenia</span><span class="sxs-lookup"><span data-stu-id="bf7b6-111">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="bf7b6-112">Riešenie problémov s certifikačnou autoritou</span><span class="sxs-lookup"><span data-stu-id="bf7b6-112">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="bf7b6-113">Politika riešenia problémov</span><span class="sxs-lookup"><span data-stu-id="bf7b6-113">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

<span data-ttu-id="bf7b6-114">Ak chcete zabezpečiť e-maily (Exchange Online) z Accessu v nevyhovujúcich zariadeniach, musia sa použiť obidva dokumenty:</span><span class="sxs-lookup"><span data-stu-id="bf7b6-114">To protect Email (Exchange online) from access by noncompliant devices, both documents must be followed:</span></span>

1. [<span data-ttu-id="bf7b6-115">Ochrana e-mailového prístupu zo zariadení pomocou EAS</span><span class="sxs-lookup"><span data-stu-id="bf7b6-115">Protect email access from devices using EAS</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-unmanaged-devices)
2. [<span data-ttu-id="bf7b6-116">Ochrana e-mailového prístupu zo zariadení pomocou moderných klientov overovania, ako je Outlook</span><span class="sxs-lookup"><span data-stu-id="bf7b6-116">Protect email access from devices using modern authentication clients like Outlook</span></span>](https://docs.microsoft.com/intune/tutorial-protect-email-on-enrolled-devices)
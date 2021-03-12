---
title: Používanie podmieneného prístupu so službou Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749262"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="3091f-102">Používanie podmieneného prístupu so službou Intune</span><span class="sxs-lookup"><span data-stu-id="3091f-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="3091f-103">Používanie podmieneného prístupu so službou Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="3091f-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="3091f-104">Vytvorte politiku dodržiavania súladu a definujte nastavenia, ktoré je potrebné splniť pred tým, ako sa zariadenie považuje za vyhovujúce. Zariadenie musí mať napríklad PIN kód aspoň 6 číslic, kým sa považuje za vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="3091f-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="3091f-105">Vytvorenie politiky podmieneného prístupu, ktorá definuje, aké zdroje sú chránené, a aké podmienky je potrebné splniť na prístup k týmto zdrojom. Zariadenie musí byť napríklad kompatibilné pred prístupom k podnikovému e-mailu.</span><span class="sxs-lookup"><span data-stu-id="3091f-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="3091f-106">Zabezpečte, aby politiky dodržiavania súladu a politiky podmieneného prístupu boli zacielené na požadované skupiny používateľov. Môže to vyžadovať vytvorenie konkrétnych skupín používateľov v službe Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3091f-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="3091f-107">Ďalšie informácie...</span><span class="sxs-lookup"><span data-stu-id="3091f-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)

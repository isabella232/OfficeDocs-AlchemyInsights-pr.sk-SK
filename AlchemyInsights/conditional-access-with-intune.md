---
title: Podmienený prístup so službou Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662342"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="32ad1-102">Podmienený prístup so službou Intune</span><span class="sxs-lookup"><span data-stu-id="32ad1-102">Conditional Access with Intune</span></span>

<span data-ttu-id="32ad1-103">Používanie **Podmieneného prístupu** s Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="32ad1-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="32ad1-p101">Vytvorenie **Podmieneného prístupu politiky** , ktorá definuje aké zdroje sú chránené a aké podmienky musia byť splnené, aby prístup týchto zdrojov. Napríklad zariadenie musí byť kompatibilné s pred prístupom k podnikovým e-mailom.</span><span class="sxs-lookup"><span data-stu-id="32ad1-p101">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="32ad1-p102">Vytvoriť **Súlad politiky** definuje nastavenia, ktoré musia byť splnené pred zariadenie sa považuje za vyhovujúce. Napríklad zariadenie musí mať pin aspoň 6 číslice, predtým, než sa považuje za vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="32ad1-p102">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="32ad1-p103">Zabezpečiť **Súlad politík** a **Podmieneného prístupu politiky** sú zamerané na požadovanej skupiny používateľov. To môže vyžadovať vytvorenie konkrétnym skupinám používateľov Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="32ad1-p103">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="32ad1-110">Prečítajte si viac:</span><span class="sxs-lookup"><span data-stu-id="32ad1-110">Read more:</span></span>
  
- [<span data-ttu-id="32ad1-111">Podmieneného prístupu osvedčených postupov</span><span class="sxs-lookup"><span data-stu-id="32ad1-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="32ad1-112">Začíname s podmieneným prístupom</span><span class="sxs-lookup"><span data-stu-id="32ad1-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    


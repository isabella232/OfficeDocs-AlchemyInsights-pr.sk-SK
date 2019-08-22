---
title: Podmienený prístup so službou Intune
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36505009"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="e2432-102">Podmienený prístup so službou Intune</span><span class="sxs-lookup"><span data-stu-id="e2432-102">Conditional Access with Intune</span></span>

<span data-ttu-id="e2432-103">Používanie **Podmieneného prístupu** s Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="e2432-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="e2432-104">Vytvorenie **Podmieneného prístupu politiky** , ktorá definuje aké zdroje sú chránené a aké podmienky musia byť splnené, aby prístup týchto zdrojov.</span><span class="sxs-lookup"><span data-stu-id="e2432-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="e2432-105">Napríklad zariadenie musí byť kompatibilné s pred prístupom k podnikovým e-mailom.</span><span class="sxs-lookup"><span data-stu-id="e2432-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="e2432-106">Vytvoriť **Súlad politiky** definuje nastavenia, ktoré musia byť splnené pred zariadenie sa považuje za vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="e2432-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="e2432-107">Napríklad zariadenie musí mať pin aspoň 6 číslice, predtým, než sa považuje za vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="e2432-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="e2432-108">Zabezpečiť **Súlad politík** a **Podmieneného prístupu politiky** sú zamerané na požadovanej skupiny používateľov.</span><span class="sxs-lookup"><span data-stu-id="e2432-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="e2432-109">To môže vyžadovať vytvorenie konkrétnym skupinám používateľov Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="e2432-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="e2432-110">Prečítajte si viac:</span><span class="sxs-lookup"><span data-stu-id="e2432-110">Read more:</span></span>
  
- [<span data-ttu-id="e2432-111">Podmieneného prístupu osvedčených postupov</span><span class="sxs-lookup"><span data-stu-id="e2432-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="e2432-112">Začíname s podmieneným prístupom</span><span class="sxs-lookup"><span data-stu-id="e2432-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    


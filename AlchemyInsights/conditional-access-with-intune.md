---
title: Podmienený prístup pomocou Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706036"
---
# <a name="conditional-access-with-intune"></a><span data-ttu-id="c1d2a-102">Podmienený prístup pomocou Intune</span><span class="sxs-lookup"><span data-stu-id="c1d2a-102">Conditional Access with Intune</span></span>

<span data-ttu-id="c1d2a-103">Použitie **podmieneného prístupu** s Intune vyžaduje 3 kroky:</span><span class="sxs-lookup"><span data-stu-id="c1d2a-103">Using **Conditional Access** with Intune requires 3 steps:</span></span> 
  
- <span data-ttu-id="c1d2a-104">Vytvorte **politiku podmieneného prístupu** , ktorá definuje, aké prostriedky sú chránené, a aké podmienky je potrebné splniť na prístup k týmto prostriedkom.</span><span class="sxs-lookup"><span data-stu-id="c1d2a-104">Create a **Conditional Access Policy** that defines what resources are being protected, and what conditions need to be met to access those resources.</span></span> <span data-ttu-id="c1d2a-105">Zariadenie musí byť napríklad kompatibilné pred prístupom do podnikového e-mailu.</span><span class="sxs-lookup"><span data-stu-id="c1d2a-105">For example, a device must be compliant before accessing corporate email.</span></span> 
    
- <span data-ttu-id="c1d2a-106">Vytvorenie **politiky súladu** na definovanie nastavení, ktoré musia byť splnené pred tým, ako sa zariadenie považuje za vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="c1d2a-106">Create a **Compliance Policy** to define settings that must be met before the device is considered compliant.</span></span> <span data-ttu-id="c1d2a-107">Zariadenie musí mať napríklad PIN aspoň 6 číslic predtým, ako sa považuje za vyhovujúce.</span><span class="sxs-lookup"><span data-stu-id="c1d2a-107">For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span> 
    
- <span data-ttu-id="c1d2a-108">Zabezpečenie **politík súladu** a **politiky podmieneného prístupu** sú zacielené na želané skupiny používateľov.</span><span class="sxs-lookup"><span data-stu-id="c1d2a-108">Ensuring both **Compliance Policies** and **Conditional Access Policies** are targeted to the desired groups of users.</span></span> <span data-ttu-id="c1d2a-109">To môže vyžadovať vytvorenie konkrétnych skupín používateľov v Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c1d2a-109">This may require creating specific groups of users in Azure Active Directory.</span></span> 
    
<span data-ttu-id="c1d2a-110">Čítajte viac:</span><span class="sxs-lookup"><span data-stu-id="c1d2a-110">Read more:</span></span>
  
- [<span data-ttu-id="c1d2a-111">Osvedčené postupy podmieneného prístupu</span><span class="sxs-lookup"><span data-stu-id="c1d2a-111">Conditional Access best practices</span></span>](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [<span data-ttu-id="c1d2a-112">Začíname s podmieneným prístupom</span><span class="sxs-lookup"><span data-stu-id="c1d2a-112">Getting started with Conditional Access </span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    


---
title: Zmena názvových serverov
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706770"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="e250e-102">Aktualizácia názvových serverov domény, aby smerovali na Microsoft</span><span class="sxs-lookup"><span data-stu-id="e250e-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="e250e-103">Poznámka: Rozšírenie zmien názvových serverov môže trvať až 48 hodín.</span><span class="sxs-lookup"><span data-stu-id="e250e-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="e250e-104">Ak chcete nastaviť doménu v službách Microsoft 365, názvové servery u vášho registrátora musia byť aktualizované.</span><span class="sxs-lookup"><span data-stu-id="e250e-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="e250e-105">Vytvorte alebo upravte záznamy názvového servera u registrátora domén.</span><span class="sxs-lookup"><span data-stu-id="e250e-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="e250e-106">Prejdite na webovú lokalitu registrátora domén a vyhľadajte miesto, kde môžete upraviť názvové servery.</span><span class="sxs-lookup"><span data-stu-id="e250e-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="e250e-107">Vytvorte alebo upravte dva záznamy názvového servera, ktoré sa zhodujú s týmito hodnotami:</span><span class="sxs-lookup"><span data-stu-id="e250e-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="e250e-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e250e-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="e250e-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="e250e-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="e250e-110">Uložte zmeny.</span><span class="sxs-lookup"><span data-stu-id="e250e-110">Save changes.</span></span>

<span data-ttu-id="e250e-111">Podrobné pokyny nájdete aj v tomto článku: [Zmena názvových serverov s ľubovoľným registrátorom domén](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="e250e-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  
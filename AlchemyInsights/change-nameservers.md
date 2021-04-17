---
title: Zmena názvových serverov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 67680a6fa514d31ccb88cc8691a199cd1f58a402
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818627"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="57711-102">Aktualizácia názvových serverov domény, aby smerovali na Microsoft</span><span class="sxs-lookup"><span data-stu-id="57711-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="57711-103">Poznámka: Rozšírenie zmien názvových serverov môže trvať až 48 hodín.</span><span class="sxs-lookup"><span data-stu-id="57711-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="57711-104">Ak chcete nastaviť doménu v službách Microsoft 365, názvové servery u vášho registrátora musia byť aktualizované.</span><span class="sxs-lookup"><span data-stu-id="57711-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="57711-105">Vytvorte alebo upravte záznamy názvového servera u registrátora domén.</span><span class="sxs-lookup"><span data-stu-id="57711-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="57711-106">Prejdite na webovú lokalitu registrátora domén a vyhľadajte miesto, kde môžete upraviť názvové servery.</span><span class="sxs-lookup"><span data-stu-id="57711-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="57711-107">Vytvorte alebo upravte dva záznamy názvového servera, ktoré sa zhodujú s týmito hodnotami:</span><span class="sxs-lookup"><span data-stu-id="57711-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="57711-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="57711-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="57711-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="57711-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="57711-110">Uložte zmeny.</span><span class="sxs-lookup"><span data-stu-id="57711-110">Save changes.</span></span>

<span data-ttu-id="57711-111">Podrobné pokyny nájdete aj v tomto článku: [Zmena názvových serverov s ľubovoľným registrátorom domén](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="57711-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  
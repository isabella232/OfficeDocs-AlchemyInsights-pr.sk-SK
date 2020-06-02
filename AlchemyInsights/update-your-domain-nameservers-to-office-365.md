---
title: Aktualizácia názvových serverov domény, aby smerovali na Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 9dd52c60b2d15d66c1c3f2a96c9db08ea2a010c6
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510299"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="ca71a-102">Aktualizácia názvových serverov domény, aby smerovali na Microsoft</span><span class="sxs-lookup"><span data-stu-id="ca71a-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="ca71a-103">Poznámka: Rozšírenie zmien názvových serverov môže trvať až 48 hodín.</span><span class="sxs-lookup"><span data-stu-id="ca71a-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="ca71a-104">Ak chcete nastaviť doménu so spoločnosťou Microsoft, je potrebné aktualizovať názvové servery registrátora.</span><span class="sxs-lookup"><span data-stu-id="ca71a-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="ca71a-105">Vytvorte alebo upravte záznamy názvového servera u registrátora domén.</span><span class="sxs-lookup"><span data-stu-id="ca71a-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="ca71a-106">Prejdite na webovú lokalitu registrátora domén a vyhľadajte miesto, kde môžete upraviť názvové servery.</span><span class="sxs-lookup"><span data-stu-id="ca71a-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="ca71a-107">Vytvorte alebo upravte dva záznamy názvového servera, ktoré sa zhodujú s týmito hodnotami:</span><span class="sxs-lookup"><span data-stu-id="ca71a-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="ca71a-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ca71a-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="ca71a-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ca71a-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="ca71a-110">Uložte zmeny.</span><span class="sxs-lookup"><span data-stu-id="ca71a-110">Save changes.</span></span>

<span data-ttu-id="ca71a-111">Podrobné pokyny nájdete aj v tomto článku: [Zmena názvových serverov na nastavenie programu Microsoft 365 s ľubovoľným registrátorom domény](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="ca71a-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  
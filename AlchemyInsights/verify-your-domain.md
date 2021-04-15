---
title: Overenie domény
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771006"
---
# <a name="verify-your-domain"></a><span data-ttu-id="3f90b-102">Overenie domény</span><span class="sxs-lookup"><span data-stu-id="3f90b-102">Verify your domain</span></span>

 <span data-ttu-id="3f90b-103">**Záznam pravdepodobne nebol aktualizovaný na internete.**</span><span class="sxs-lookup"><span data-stu-id="3f90b-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="3f90b-104">Zvyčajne trvá len niekoľko minút, kým sa nám zobrazí nový záznam, ale niekedy to môže trvať aj niekoľko hodín.</span><span class="sxs-lookup"><span data-stu-id="3f90b-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="3f90b-105">Ak ste tak dlho počkali, overte, či ste skopírovali a prilepení presnej hodnoty do overovacieho TXT záznamu u svojho hostiteľa DNS.</span><span class="sxs-lookup"><span data-stu-id="3f90b-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="3f90b-106">Jeden bežný problém je nezahrnienie časti "MS=" záznamu.</span><span class="sxs-lookup"><span data-stu-id="3f90b-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="3f90b-107">Potrebujeme aj tú.</span><span class="sxs-lookup"><span data-stu-id="3f90b-107">We need that too!</span></span>

- <span data-ttu-id="3f90b-108">U niektorých hostiteľov DNS musíte urobiť krok navyše a uložiť súbor zóny (kde je uložený DNS záznam) tak, aby sa aktual nachádzal na internete.</span><span class="sxs-lookup"><span data-stu-id="3f90b-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="3f90b-109">Uistite sa, že ste uložili zmeny, aby Microsoft mohol záznam zobraziť a overiť.</span><span class="sxs-lookup"><span data-stu-id="3f90b-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>

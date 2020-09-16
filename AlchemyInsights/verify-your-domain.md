---
title: Overenie domény
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734321"
---
# <a name="verify-your-domain"></a><span data-ttu-id="a8a08-102">Overenie domény</span><span class="sxs-lookup"><span data-stu-id="a8a08-102">Verify your domain</span></span>

 <span data-ttu-id="a8a08-103">**Záznam sa pravdepodobne neaktualizoval cez internet.**</span><span class="sxs-lookup"><span data-stu-id="a8a08-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="a8a08-104">Je to zvyčajne len pár minút, aby sme mohli vidieť nový záznam, ale občas to môže trvať aj niekoľko hodín.</span><span class="sxs-lookup"><span data-stu-id="a8a08-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="a8a08-105">Ak ste už dlho čakali, dvakrát skontrolujte, či ste skopírovali a prilepili presnú hodnotu do záznamu na overenie TXT u svojho hostiteľa DNS.</span><span class="sxs-lookup"><span data-stu-id="a8a08-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="a8a08-106">Jedným z bežných problémov nie je zahrnutie časti "MS =" záznamu.</span><span class="sxs-lookup"><span data-stu-id="a8a08-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="a8a08-107">Potrebujeme to taky!</span><span class="sxs-lookup"><span data-stu-id="a8a08-107">We need that too!</span></span>

- <span data-ttu-id="a8a08-108">Na niektorých hostiteľoch DNS musíte vykonať ďalší krok na uloženie súboru zóny (v ktorom je uložený DNS záznam), aby sa aktualizoval cez internet.</span><span class="sxs-lookup"><span data-stu-id="a8a08-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="a8a08-109">Presvedčte sa, že ste uložili zmeny tak, aby Microsoft mohol Zobraziť a overiť záznam.</span><span class="sxs-lookup"><span data-stu-id="a8a08-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>

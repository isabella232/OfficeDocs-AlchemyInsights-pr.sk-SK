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
# <a name="verify-your-domain"></a>Overenie domény

 **Záznam pravdepodobne nebol aktualizovaný na internete.**
  
Zvyčajne trvá len niekoľko minút, kým sa nám zobrazí nový záznam, ale niekedy to môže trvať aj niekoľko hodín. 
  
- Ak ste tak dlho počkali, overte, či ste skopírovali a prilepení presnej hodnoty do overovacieho TXT záznamu u svojho hostiteľa DNS. Jeden bežný problém je nezahrnienie časti "MS=" záznamu. Potrebujeme aj tú.

- U niektorých hostiteľov DNS musíte urobiť krok navyše a uložiť súbor zóny (kde je uložený DNS záznam) tak, aby sa aktual nachádzal na internete. Uistite sa, že ste uložili zmeny, aby Microsoft mohol záznam zobraziť a overiť.

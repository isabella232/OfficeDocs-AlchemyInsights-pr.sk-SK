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
ms.openlocfilehash: 9e258cfc70c57fe787830d659dc52f4696768bea164d3be9ce7bcb9e7123c5a9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971030"
---
# <a name="verify-your-domain"></a>Overenie domény

 **Záznam pravdepodobne nebol aktualizovaný na internete.**
  
Zvyčajne trvá len niekoľko minút, kým sa nám zobrazí nový záznam, ale niekedy to môže trvať aj niekoľko hodín. 
  
- Ak ste tak dlho počkali, overte, či ste skopírovali a prilepení presnej hodnoty do overovacieho TXT záznamu u svojho hostiteľa DNS. Jeden bežný problém je nezahrnienie časti "MS=" záznamu. Potrebujeme aj tú.

- U niektorých hostiteľov DNS musíte urobiť krok navyše a uložiť súbor zóny (kde je uložený DNS záznam) tak, aby sa aktual nachádzal na internete. Uistite sa, že ste uložili zmeny, aby Microsoft mohol záznam zobraziť a overiť.

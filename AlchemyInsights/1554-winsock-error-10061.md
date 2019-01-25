---
title: Chyba rozhrania Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29488897"
---
# <a name="winsock-error-10061"></a>Chyba rozhrania Winsock 10061

Tento kód chyby znamená, že Office 365 nemohol vytvoriť soket TCP (pripojenie) s cieľového hostiteľa. Najpravdepodobnejšou príčinou vzniku tejto chyby je problém s konfiguráciou brány firewall. Ak chcete vyriešiť tento problém, skontrolujte tieto nastavenia:
  
- Overte konfiguráciu brány firewall s informáciami v [Office 365 URL a IP rozsahu adries](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- Ak chyba je špecifická pre Exchange Online Protection (EOP), ste mali predtým oznámili zmenu na [Exchange Online Protection IP adries](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- Overiť, že váš Internet Service Provider (ISP) nie je blokovanie portov.
    
- Overenie smart hostiteľským a cieľovým server nastavenia vo vašom konektory.
    
Všimnite si, že Office 365 nemá blokovať *prichádzajúce* pripojenia týmto spôsobom. 
  


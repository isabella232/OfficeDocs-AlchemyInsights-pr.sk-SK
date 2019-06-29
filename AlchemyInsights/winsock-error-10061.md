---
title: Chyba rozhrania Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e82e90b670235848105636fb2039ed60d3b93c67
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364928"
---
# <a name="winsock-error-10061"></a>Chyba rozhrania Winsock 10061

Tento kód chyby znamená, že Office 365 nemohol vytvoriť soket TCP (pripojenie) s cieľového hostiteľa. Najpravdepodobnejšou príčinou vzniku tejto chyby je problém s konfiguráciou brány firewall. Ak chcete vyriešiť tento problém, skontrolujte tieto nastavenia:

- Overte konfiguráciu brány firewall s informáciami v [Office 365 URL a IP rozsahu adries](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ak chyba je špecifická pre Exchange Online Protection (EOP), ste mali predtým oznámili zmenu na [Exchange Online Protection IP adries](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Overiť, že váš Internet Service Provider (ISP) nie je blokovanie portov.

- Overenie smart hostiteľským a cieľovým server nastavenia vo vašom konektory.

Všimnite si, že Office 365 nemá blokovať *prichádzajúce* pripojenia týmto spôsobom.

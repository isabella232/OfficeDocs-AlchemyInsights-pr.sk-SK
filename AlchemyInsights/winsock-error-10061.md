---
title: 1554 chyba rozhrania Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766184"
---
# <a name="winsock-error-10061"></a>Chyba rozhrania Winsock 10061

Tento kód chyby znamená, že spoločnosť Microsoft nemohla vytvoriť soket TCP (pripojenie) s cieľovým hostiteľom. Najpravdepodobnejšou príčinou tejto chyby je problém s konfiguráciou brány firewall. Ak chcete problém vyriešiť, skontrolujte tieto nastavenia:

- Overte konfiguráciu brány firewall s informáciami v [Microsoft 365 URL a rozsahy adries IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ak je chyba špecifická pre Exchange Online Protection (EOP), mali by ste boli predtým upozornení na zmenu [Exchange Online Protection IP adresy](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Overte, či poskytovateľ internetových služieb (ISP) neblokuje port.

- Skontrolujte nastavenia inteligentných hostiteľov a cieľového servera v konektoroch.

Všimnite si, že Microsoft 365 neblokuje *prichádzajúce* pripojenia týmto spôsobom.

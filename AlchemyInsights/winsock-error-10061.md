---
title: Chyba 1554 Vlašove 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083245"
---
# <a name="winsock-error-10061"></a>Chyba Vlašook 10061

Tento kód chyby znamená, že spoločnosti Microsoft sa nepodarilo vytvoriť TCP socket (pripojenie) s cieľovým hostiteľom. Najpravdepodobnou príčinou tejto chyby je problém s konfiguráciou brány firewall. Ak chcete problém vyriešiť, skontrolujte tieto nastavenia:

- Overenie konfigurácie brány firewall pomocou informácií z [Microsoft 365 URL adries a rozsahov IP adries](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ak je chyba špecifická pre Exchange Online Protection (EOP), mali by ste byť predtým upozornení na [zmenu Exchange Online Protection IP adries.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Overte, či váš poskytovateľ internetových služieb (ISP) neblokuje port.

- Overte nastavenia servera smart host a target server v konektoroch.

Pamätajte, Microsoft 365 spôsob neblokuje *prichádzajúce* pripojenia.

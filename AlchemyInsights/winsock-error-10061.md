---
title: 1554 Winsock error 10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698877"
---
# <a name="winsock-error-10061"></a>Chyba rozhrania Winsock 10061

Tento kód chyby znamená, že spoločnosť Microsoft nedokáže vytvoriť zásuvku TCP (pripojenie) s cieľovým hostiteľom. Najpravdepodobnejšou príčinou tejto chyby je problém s konfiguráciou brány firewall. Ak chcete problém vyriešiť, skontrolujte tieto nastavenia:

- Overenie konfigurácie brány firewall s informáciami v [rozsahu URL adries a rozsahov IP adries v Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ak je chyba špecifická pre Exchange Online Protection (EOP), mali by ste byť predtým upozornení na zmenu [IP adries ochrany v službe Exchange Online](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Overte, či poskytovateľ internetových služieb (ISP) neblokuje port.

- Overte nastavenia inteligentného hostiteľa a cieľového servera v konektoroch.

Všimnite si, že Microsoft 365 neblokuje *prichádzajúce* pripojenia týmto spôsobom.

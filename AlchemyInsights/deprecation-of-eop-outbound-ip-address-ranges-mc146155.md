---
title: 1065 zamietnutá IP adresa odchádzajúce rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806810"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Odmietanie rozsahov IP adries pre odchádzajúce prenosy EOP

Zistili sme potenciálny problém s vašou organizáciou, ktorý (ak nie je opravený do 26. októbra 2018) môže zlomiť tok pošty do lokálnych alebo externých destinácií. Na zjednodušenie spravovania rozsahu IP adries ako predtým oznámených sa konsolidujú rozsahy IP adries pre Exchange Online Protection (EOP), ktoré sa používajú na odosielanie a prijímanie e-mailov mimo služby Microsoft 365. Naša analýza označuje, že jeden alebo viaceré externé e-mailové zdroje alebo cieľové umiestnenia, ktoré ste nakonfigurovali v konektoroch toku pošty, neprijímajú pripojenia z rozsahov IP adries, ktoré sú [tu](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)zobrazené.

Konať pred 26. októbra, aby sa zabezpečilo, že tieto zdroje a ciele budú prijímať spojenia zo všetkých [publikovaných IP adries a zo všetkých publikovaných IP adries](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Ďalšie informácie o tejto zmene nájdete v centre správ príspevky [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)alebo [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Poznámka**: Ak ste predtým použili IP alebo URL publikovanie prostredníctvom HTML, XML a informačného kanála RSS pre aktualizácie koncových bodov, mali by ste tiež migrovať na nové webové služby na automatizáciu týchto typov aktualizácií. Ďalšie informácie nájdete v téme [kategórie koncových bodov v službe microsoft 365 a adresa IP a webová služba spoločnosti microsoft 365](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).

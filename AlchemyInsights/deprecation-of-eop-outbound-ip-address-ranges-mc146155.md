---
title: 1065 deaktivácia EOP odchádzajúce IP adresa rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704612"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecácia rozsahov IP odchádzajúcich adries EOP

Zistili sme potenciálny problém s vašou organizáciou, že (ak nie je opravené 26. októbra, 2018) môže zlomiť tok pošty do lokálnych alebo externých destinácií. Ako už bolo oznámené, zjednodušiť riadenie rozsahu adries IP, sme konsolidácia Exchange Online Protection (EOP) IP adries rozsahy, ktoré sa používajú na odosielanie a prijímanie e-mailov mimo Microsoft 365. Z našej analýzy vyplýva, že jeden alebo viac externých e-mailových zdrojov alebo cieľových miest, ktoré ste nakonfigurovali v konektoroch toku pošty, neprijímajú pripojenia z rozsahov adries IP, ktoré sú [tu](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)zobrazené.

Zákon pred 26. října na zabezpečenie týchto zdrojov a destinácií bude akceptovať pripojenie k a zo všetkých [publikovaných EOP IP adresy](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Ďalšie informácie o tejto zmene nájdete centrum správ príspevky [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)alebo [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Poznámka**: Ak ste predtým používali IP alebo URL publikovanie prostredníctvom HTML, XML a RSS pre Endpoint aktualizácie, mali by ste tiež migrovať na nové webové služby pre automatizáciu týchto typov aktualizácií. Ďalšie informácie nájdete v téme [microsoft 365 koncový bod kategórie a microsoft 365 adresu IP a URL webovej služby](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).

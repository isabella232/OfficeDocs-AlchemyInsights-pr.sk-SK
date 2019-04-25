---
title: 1065 odsudzovanie EOP odchádzajúce IP adresa rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404836"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Odmietanie EOP odchádzajúce rozsahy adries IP

Zistili sme potenciálny problém s vašou organizáciou (ak nie je opravené 26 októbra 2018) by mohol zlomiť tok pošty lokálne alebo externé ciele. Ako predtým oznámené, zjednodušiť spravovanie rozsah IP adries, sme sa konsolidácia rozsahy adries IP Exchange Online Protection (EOP), ktoré sa používajú na odosielať a prijímať e-maily mimo Office 365. Naša analýza naznačuje, že jeden alebo viac zdrojov externých e-mailov alebo ciele, ktoré ste nakonfigurovali v pošty tok konektory nie sú prijímať pripojenia z IP adresy rozsahy uvedené [tu](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Konať pred 26.októbra na zabezpečenie týchto zdrojov a destinácií bude akceptovať spojenie na všetky [uverejnené EOP IP adresy](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

Ďalšie informácie o tejto zmene nájdete Message Center príspevky [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)alebo [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).

**Poznámka**: Ak ste predtým používali IP alebo adresu URL publikovanie cez HTML, XML a RSS aktualizácií endpoint, tiež by mali migrovať na nové webové služby pre automatizáciu týchto typov aktualizácií. Ďalšie informácie nájdete v [kategórií koncový bod Office 365 a Office 365 IP adresa a adresa URL webovej služby](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).

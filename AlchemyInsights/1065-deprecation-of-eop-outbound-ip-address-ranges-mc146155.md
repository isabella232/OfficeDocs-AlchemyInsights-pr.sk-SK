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
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 2b4b2e2341f45e2d37713d72a2e0d34fa1a9a7cc
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934899"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Odmietanie EOP odchádzajúce rozsahy adries IP

Zistili sme potenciálny problém s vašou organizáciou (ak nie je opravené 26 októbra 2018) by mohol zlomiť tok pošty lokálne alebo externé ciele. Ako predtým oznámené, zjednodušiť spravovanie rozsah IP adries, sme sa konsolidácia rozsahy adries IP Exchange Online Protection (EOP), ktoré sa používajú na odosielať a prijímať e-maily mimo Office 365. Naša analýza naznačuje, že jeden alebo viac zdrojov externých e-mailov alebo ciele, ktoré ste nakonfigurovali v pošty tok konektory nie sú prijímať pripojenia z IP adresy rozsahy uvedené [tu](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Konať pred 26.októbra na zabezpečenie týchto zdrojov a destinácií bude akceptovať spojenie na všetky [uverejnené EOP IP adresy](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
  
Ďalšie informácie o tejto zmene nájdete Message Center príspevky [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)alebo [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).
  
 **Poznámka**: Ak ste predtým používali IP alebo adresu URL publikovanie cez HTML, XML a RSS aktualizácií endpoint, tiež by mali migrovať na nové webové služby pre automatizáciu týchto typov aktualizácií. Ďalšie informácie nájdete v [kategórií koncový bod Office 365 a Office 365 IP adresa a adresa URL webovej služby](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).
  


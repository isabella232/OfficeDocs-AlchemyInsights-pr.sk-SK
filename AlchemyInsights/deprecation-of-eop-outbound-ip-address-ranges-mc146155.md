---
title: 1065 – Deprecation of EOP out IP address rangesMC146155
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
ms.openlocfilehash: 214abc57a99c70a02a7d159441713e007f6ad980f67e373780d4ca297f69f764
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031277"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>Deprecation of EOP outbound IP address ranges

Zistili sme potenciálny problém s vašou organizáciou, ktorý (ak nie je opravený do 26. októbra 2018) môže prerušiť tok pošty do vašich lokálnych alebo externých cieľových miest. Ako sa predtým komunikovali a zjednodušili správu rozsahu IP adries, zjednocujeme rozsahy IP adries pre Exchange Online Protection (EOP), ktoré sa používajú na odosielanie a prijímanie e-mailov mimo Microsoft 365. Z našej analýzy vyplýva, že jeden alebo viacero externých zdrojov e-mailov alebo cieľových miest, ktoré ste nakonfigurovali v konektoroch toku pošty, neprijímajú pripojenia z rozsahov IP adries zobrazených [tu.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Konať pred 26. októbra s cieľom zabezpečiť, aby tieto zdroje a ciele prijímali pripojenia do a zo všetkých [publikovaných IP adries služby EOP.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

Ďalšie informácie o tejto zmene nájdete v téme Príspevky v Centre správ [MC146155,](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155) [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)alebo [MC149274.](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)

**Poznámka:** Ak ste predtým používali publikovanie IP adresy alebo URL adresy cez HTML, XML a RSS pre aktualizácie koncových bodov, mali by ste tiež vykonať migráciu do nových webových služieb s cieľom automatizácie týchto typov aktualizácií. Ďalšie informácie nájdete v Microsoft 365 [kategórií koncových bodov a Microsoft 365 IP adresy a webovej služby URL.](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)

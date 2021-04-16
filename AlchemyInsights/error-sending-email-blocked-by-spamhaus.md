---
title: Chyba pri odosielaní e-mailov zablokovaných zo strany súboru SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813739"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Chyba pri odosielaní e-mailu: Hostiteľ klienta zablokovaný pomocou lokality Spamhaus

IP adresa, z ktorých bola správa odoslaná, je v zozname blokovaných položiek vo vlastníctve lokality [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Dôvodom zablokovania zo strany lokality Spamhaus môže byť zneužiné kontá, zneužiné počítače so zdieľaním verejnej IP adresy a zásady poskytovateľa internetových služieb (ISP). Možné opravy:
  
- Pri blokovaných prichádzajúcich správach, ktoré určujú zdrojový e-mailový server, je nutné určiť príčinu a odstrániť blokovanie z webovej lokality Spamhaus.

- V prípade blokovaných prichádzajúcich správ, pri ktorých patrí zdrojová IP adresa inému vlastníkovi, musí blokovanie z webovej lokality Spamhaus odstrániť vlastník adresy. Ak sa IP adresa nachádza v zozname blokovaných politík (PBL), vlastník môže priradiť inú statickú IP adresu alebo odstrániť adresu zo zoznamu PBL.

- V prípade blokovaných odchádzajúcich správ z domény pripojenej k spoločnosti Microsoft sa môže táto chyba zobraziť, ak sú správy smerované cez službu tretej strany. Vlastníka blokovanú IP adresu môžete vyhľadať pomocou vyhľadávacieho nástroja WHOIS.

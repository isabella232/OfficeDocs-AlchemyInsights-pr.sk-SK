---
title: Chyba pri odosielaní e-mailov zablokovaných SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783818"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Chyba pri odosielaní e-mailu: hostiteľ klienta je blokovaný pomocou spamhaus

IP adresa, ktorá odoslala správu, je v zozname blokovaných vo vlastníctve [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Dôvody, prečo zablokoval spamhaus, zahŕňajú ohrozené kontá, ohrozené počítače, ktoré zdieľajú verejnú IP adresu, a politiky poskytovateľa internetových služieb (ISP). Možné opravy:
  
- V prípade blokovaných prichádzajúcich správ, na ktorých môžete ovládať zdrojový e-mailový server, je potrebné určiť príčinu a odstrániť blok z webovej lokality spamhaus.

- V prípade blokovaných prichádzajúcich správ, v ktorých je zdrojová IP adresa členom inej osoby, musí vlastník adresy odstrániť blok z webovej lokality spamhaus. Ak sa IP adresa nachádza v zozname blok politiky (PBL), vlastník môže priradiť inú statickú IP adresu alebo odstrániť adresu z poľa PBL.

- V prípade blokovaných odchádzajúcich správ z vašej domény pripojenej k spoločnosti Microsoft sa môže táto chyba Zobraziť, ak sú správy smerované prostredníctvom služby tretích strán. Pomocou nástroja vyhľadávania WHOIS môžete nájsť blokovaných vlastníkov IP adries.

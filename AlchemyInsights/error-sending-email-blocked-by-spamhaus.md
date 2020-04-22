---
title: Chyba pri odosielaní e-mailov zablokovaných SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714273"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Chyba pri odosielaní e-mailu: klient hostiteľa blokovaný pomocou spamhaus

Adresa IP, ktorá odoslala správu, sa nachádza na zozname blokovaných položiek, ktorý vlastní [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Dôvody pre blokovanie spamhaus zahŕňajú kompromitovaných účtov, ohrozená stroje zdieľanie verejnej IP adresu a Internet Service Provider (ISP) politiky. Možné opravy sú:
  
- Pre blokované prichádzajúce správy, kde ovládate zdrojový e-mailový server, musíte určiť príčinu a odstrániť blok z webovej stránky spamhaus.

- Pre blokované prichádzajúce správy, kde zdrojová adresa IP patrí niekomu inému, vlastník adresy musí odstrániť blok z webovej stránky spamhaus. Ak je adresa IP v zozname blokovaných politík (PBL), vlastník môže priradiť inú statickú adresu IP alebo odstrániť adresu z PBL.

- Pre blokované odchádzajúce správy z domény pripojenej k spoločnosti Microsoft, môžete získať túto chybu, ak správy sú smerované prostredníctvom 3rd party služby. Na vyhľadanie zablokovaného vlastníka adresy IP môžete použiť vyhľadávací nástroj WHOIS.

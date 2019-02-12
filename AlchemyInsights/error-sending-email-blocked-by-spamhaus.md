---
title: Chyba pri odosielaní e-mailu blokovaný SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912363"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Chyba pri odosielaní e-mailu: klienta hostiteľa blokovaný pomocou Spamhaus

IP adresu, ktorá správu odoslala sa na zoznam zablokovaných vlastníctve [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Príčiny pre blokovaný Spamhaus prelomených účtov, ohrozená stroje zdieľanie verejnú IP adresu, a podmienky Internet Service Provider (ISP). Možné opravy sú:
  
- Pre blokované prichádzajúce správy do služieb Office 365, kde ovládate zdroj e-mailový server, musíte určiť príčinu a odstrániť blok z internetovej Spamhaus.
    
- Blokované prichádzajúce správy do služby Office 365 kde zdrojová adresa IP patrí niekomu inému, adresa vlastníka treba odstrániť blok z internetovej Spamhaus. Ak je adresa IP na politiku blokovať zoznamu (PBL), vlastník môžete priradiť rôzne statickú IP adresu alebo odstráňte adresu zo PBL.
    
- Blokované odchádzajúce správy z vašej domény Office 365, môžete dostať túto chybu, ak správy sú smerované prostredníctvom 3rd party servis. WHOIS lookup nástroj môžete použiť na vyhľadanie blokovaných IP adresa vlastníka.
    


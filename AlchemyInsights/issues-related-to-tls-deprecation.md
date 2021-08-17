---
title: Z dôvodu zakázania PROTOKOLU TLS 1.0 a TLS 1.1 nie je možné odosielať a prijímať e-maily do alebo z programu Office 365
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054921"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Z dôvodu zakázania PROTOKOLU TLS 1.0 a TLS 1.1 nie je možné odosielať a prijímať e-maily do alebo z programu Office 365

Ako bolo potvrdené v centre správ po príspevku MC229914, po prepustení protokolov TLS 1.0 a TLS 1.1 sa začalo vyvolanie koncových bodov Exchange Online toku pošty. Čoskoro Office 365 pripojenia k e-mailovým pripojeniam z externých zdrojov už nebudú akceptovať protokoly TLS 1.0 a TLS 1.1. Okrem Exchange Online na odosielanie odchádzajúcich e-mailov nikdy nebude používať protokol TLS 1.0 ani 1.1. Ak sa vyskytnú problémy z dôvodu zakázania protokolu TLS 1.0 alebo 1.1, môže sa vyskytnúť jedna z nasledujúcich chýb:

- Odosielateľovi sa vráti e-mail o nedoručení späť – pripojenie 421 4.4.2 sa vynechá z dôvodu chyby SocketError
- Chyba v zobrazovači frontu lokálneho servera, ktorý odosiela e-maily na adresu Officer 365- '421 4.4.2 Connection vynechá pre SocketError'
- Chyba v denníku protokolu [Odoslať konektor](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) na serveri, ktorý odosiela e-maily do programu Office 365 - zlyhanie pri vychýlení protokolu TLS s chybou SocketError
- Chyba v denníku protokolu konektora Odosielanie alebo prijímanie – "451 5.7.3 najskôr musí vydať príkaz STARTTLS"

Ak sa vyskytne niektorá z vyššie uvedených chýb, skontrolujte, či má server, ktorý odosiela alebo prijíma e-mail, zapnutú možnosť TLS 1.2. Skontrolujte tieto kľúče databázy Registry–

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Klient] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Ak urobíte zmeny v uvedených kľúčoch databázy Registry na povolenie protokolu TLS 1.2, reštartujte server, aby sa zmeny mohli prejaviť. Skontrolujte tiež, či máte nainštalované Windows a Exchange aktualizácie.

Ďalšie informácie nájdete v téme:

- [Exchange Server Pokyny pre protokol TLS, časť 1: Príprava na TLS 1.2 – komunita Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server Pokyny pre protokol TLS Časť 2: Povolenie protokolu TLS 1.2 a identifikácia klientov, ktorí ho nepoužíva – komunita technikov spoločnosti Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Vysvetlenie scenárov e-mailu, ak nie je možné rozumieť verziám TLS s Exchange Online – komunitou Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)

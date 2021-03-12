---
title: Nie je možné odosielať alebo odosielať e-maily do služieb Office 365 z dôvodu vypnutia TLS 1,0 a TLS 1,1
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747117"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nie je možné odosielať alebo odosielať e-maily do služieb Office 365 z dôvodu vypnutia TLS 1,0 a TLS 1,1

Ako bolo potvrdené v centre správ post MC229914, TLS 1,0 a TLS 1,1 zastaranie začalo vynucovanie pre koncové body toku pošty Exchange Online. Čoskoro Office 365 už nebude prijímať e-mailové pripojenia TLS 1,0 a TLS 1,1 z externých zdrojov. Exchange Online už nikdy nepoužíva protokol TLS 1,0 alebo 1,1 na odosielanie odchádzajúcich e-mailov. Ak sa stretávate s problémami z dôvodu vypnutia TLS 1,0 alebo 1,1, môže sa vyskytnúť niektorá z týchto chýb:

- Odosielateľ sa stáva oznámením o nedoručení sa vráti späť-' 421 4.4.2 spojenie klesol z dôvodu SocketError '
- Chyba v zobrazovači frontu lokálneho servera, ktorý odosiela e-maily dôstojníkovi 365 – 421 4.4.2 pripojenie klesol z dôvodu SocketError
- Pri odosielaní e-mailov do služieb Office 365 – zlyhanie vyjednávania [protokolov](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) TLS na serveri s chybou SocketError sa vyskytla chyba
- Chyba pri odosielaní alebo prijímaní protokolu spojnice protokolu-' 451 5.7.3 musí vydať príkaz STARTTLS prvý '

Ak sa vyskytnú niektoré z vyššie uvedených chýb, uistite sa, že server, ktorý odosiela alebo prijíma e-maily, má TLS 1,2 povolené kontrolou nasledujúcich kľúčov databázy Registry –

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ client] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**

Ak vo vyššie uvedených kľúčoch databázy Registry vykonáte zmeny, ktoré umožnia TLS 1,2, reštartujte server, aby sa zmeny prejavili. Skontrolujte tiež, či máte nainštalované najnovšie aktualizácie pre Windows a Exchange.

Ďalšie informácie nájdete v téme:

- [Usmernenie pre Exchange Server TLS, časť 1: Príprava na 1,2 TLS – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Usmernenie pre Exchange Server TLS časť 2: povolenie TLS 1,2 a identifikácia klientov, ktorí ho nepoužívajú – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Informácie o scenároch e-mailu v prípade, že nie je možné dohodnúť verzie TLS so službou Exchange Online – komunita Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)

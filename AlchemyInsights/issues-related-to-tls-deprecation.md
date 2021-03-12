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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="cd5d0-102">Nie je možné odosielať alebo odosielať e-maily do služieb Office 365 z dôvodu vypnutia TLS 1,0 a TLS 1,1</span><span class="sxs-lookup"><span data-stu-id="cd5d0-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="cd5d0-103">Ako bolo potvrdené v centre správ post MC229914, TLS 1,0 a TLS 1,1 zastaranie začalo vynucovanie pre koncové body toku pošty Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="cd5d0-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="cd5d0-104">Čoskoro Office 365 už nebude prijímať e-mailové pripojenia TLS 1,0 a TLS 1,1 z externých zdrojov.</span><span class="sxs-lookup"><span data-stu-id="cd5d0-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="cd5d0-105">Exchange Online už nikdy nepoužíva protokol TLS 1,0 alebo 1,1 na odosielanie odchádzajúcich e-mailov.</span><span class="sxs-lookup"><span data-stu-id="cd5d0-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="cd5d0-106">Ak sa stretávate s problémami z dôvodu vypnutia TLS 1,0 alebo 1,1, môže sa vyskytnúť niektorá z týchto chýb:</span><span class="sxs-lookup"><span data-stu-id="cd5d0-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="cd5d0-107">Odosielateľ sa stáva oznámením o nedoručení sa vráti späť-' 421 4.4.2 spojenie klesol z dôvodu SocketError '</span><span class="sxs-lookup"><span data-stu-id="cd5d0-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="cd5d0-108">Chyba v zobrazovači frontu lokálneho servera, ktorý odosiela e-maily dôstojníkovi 365 – 421 4.4.2 pripojenie klesol z dôvodu SocketError</span><span class="sxs-lookup"><span data-stu-id="cd5d0-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="cd5d0-109">Pri odosielaní e-mailov do služieb Office 365 – zlyhanie vyjednávania [protokolov](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) TLS na serveri s chybou SocketError sa vyskytla chyba</span><span class="sxs-lookup"><span data-stu-id="cd5d0-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="cd5d0-110">Chyba pri odosielaní alebo prijímaní protokolu spojnice protokolu-' 451 5.7.3 musí vydať príkaz STARTTLS prvý '</span><span class="sxs-lookup"><span data-stu-id="cd5d0-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="cd5d0-111">Ak sa vyskytnú niektoré z vyššie uvedených chýb, uistite sa, že server, ktorý odosiela alebo prijíma e-maily, má TLS 1,2 povolené kontrolou nasledujúcich kľúčov databázy Registry –</span><span class="sxs-lookup"><span data-stu-id="cd5d0-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="cd5d0-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ client] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="cd5d0-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="cd5d0-113">Ak vo vyššie uvedených kľúčoch databázy Registry vykonáte zmeny, ktoré umožnia TLS 1,2, reštartujte server, aby sa zmeny prejavili.</span><span class="sxs-lookup"><span data-stu-id="cd5d0-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="cd5d0-114">Skontrolujte tiež, či máte nainštalované najnovšie aktualizácie pre Windows a Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd5d0-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="cd5d0-115">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="cd5d0-115">For more information, see:</span></span>

- [<span data-ttu-id="cd5d0-116">Usmernenie pre Exchange Server TLS, časť 1: Príprava na 1,2 TLS – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="cd5d0-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="cd5d0-117">Usmernenie pre Exchange Server TLS časť 2: povolenie TLS 1,2 a identifikácia klientov, ktorí ho nepoužívajú – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="cd5d0-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="cd5d0-118">Informácie o scenároch e-mailu v prípade, že nie je možné dohodnúť verzie TLS so službou Exchange Online – komunita Microsoft</span><span class="sxs-lookup"><span data-stu-id="cd5d0-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)

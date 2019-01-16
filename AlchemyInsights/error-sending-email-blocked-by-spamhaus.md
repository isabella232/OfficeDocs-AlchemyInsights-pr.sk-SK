---
title: Chyba pri odosielaní e-mailu blokovaný SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311440"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="1b1c5-102">Chyba pri odosielaní e-mailu: klienta hostiteľa blokovaný pomocou Spamhaus</span><span class="sxs-lookup"><span data-stu-id="1b1c5-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="1b1c5-p101">IP adresu, ktorá správu odoslala sa na zoznam zablokovaných vlastníctve [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Príčiny pre blokovaný Spamhaus prelomených účtov, ohrozená stroje zdieľanie verejnú IP adresu, a podmienky Internet Service Provider (ISP). Možné opravy sú:</span><span class="sxs-lookup"><span data-stu-id="1b1c5-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="1b1c5-106">Pre blokované prichádzajúce správy do služieb Office 365, kde ovládate zdroj e-mailový server, musíte určiť príčinu a odstrániť blok z internetovej Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="1b1c5-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="1b1c5-p102">Blokované prichádzajúce správy do služby Office 365 kde zdrojová adresa IP patrí niekomu inému, adresa vlastníka treba odstrániť blok z internetovej Spamhaus. Ak je adresa IP na politiku blokovať zoznamu (PBL), vlastník môžete priradiť rôzne statickú IP adresu alebo odstráňte adresu zo PBL.</span><span class="sxs-lookup"><span data-stu-id="1b1c5-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="1b1c5-p103">Blokované odchádzajúce správy z vašej domény Office 365, môžete dostať túto chybu, ak správy sú smerované prostredníctvom 3rd party servis. WHOIS lookup nástroj môžete použiť na vyhľadanie blokovaných IP adresa vlastníka.</span><span class="sxs-lookup"><span data-stu-id="1b1c5-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    


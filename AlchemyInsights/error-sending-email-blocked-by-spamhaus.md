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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="7c2d6-102">Chyba pri odosielaní e-mailu: Hostiteľ klienta zablokovaný pomocou lokality Spamhaus</span><span class="sxs-lookup"><span data-stu-id="7c2d6-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="7c2d6-103">IP adresa, z ktorých bola správa odoslaná, je v zozname blokovaných položiek vo vlastníctve lokality [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="7c2d6-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="7c2d6-104">Dôvodom zablokovania zo strany lokality Spamhaus môže byť zneužiné kontá, zneužiné počítače so zdieľaním verejnej IP adresy a zásady poskytovateľa internetových služieb (ISP).</span><span class="sxs-lookup"><span data-stu-id="7c2d6-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="7c2d6-105">Možné opravy:</span><span class="sxs-lookup"><span data-stu-id="7c2d6-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="7c2d6-106">Pri blokovaných prichádzajúcich správach, ktoré určujú zdrojový e-mailový server, je nutné určiť príčinu a odstrániť blokovanie z webovej lokality Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="7c2d6-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="7c2d6-107">V prípade blokovaných prichádzajúcich správ, pri ktorých patrí zdrojová IP adresa inému vlastníkovi, musí blokovanie z webovej lokality Spamhaus odstrániť vlastník adresy.</span><span class="sxs-lookup"><span data-stu-id="7c2d6-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="7c2d6-108">Ak sa IP adresa nachádza v zozname blokovaných politík (PBL), vlastník môže priradiť inú statickú IP adresu alebo odstrániť adresu zo zoznamu PBL.</span><span class="sxs-lookup"><span data-stu-id="7c2d6-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="7c2d6-109">V prípade blokovaných odchádzajúcich správ z domény pripojenej k spoločnosti Microsoft sa môže táto chyba zobraziť, ak sú správy smerované cez službu tretej strany.</span><span class="sxs-lookup"><span data-stu-id="7c2d6-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="7c2d6-110">Vlastníka blokovanú IP adresu môžete vyhľadať pomocou vyhľadávacieho nástroja WHOIS.</span><span class="sxs-lookup"><span data-stu-id="7c2d6-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>

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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="3e3d1-102">Chyba pri odosielaní e-mailu: hostiteľ klienta je blokovaný pomocou spamhaus</span><span class="sxs-lookup"><span data-stu-id="3e3d1-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="3e3d1-103">IP adresa, ktorá odoslala správu, je v zozname blokovaných vo vlastníctve [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="3e3d1-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="3e3d1-104">Dôvody, prečo zablokoval spamhaus, zahŕňajú ohrozené kontá, ohrozené počítače, ktoré zdieľajú verejnú IP adresu, a politiky poskytovateľa internetových služieb (ISP).</span><span class="sxs-lookup"><span data-stu-id="3e3d1-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="3e3d1-105">Možné opravy:</span><span class="sxs-lookup"><span data-stu-id="3e3d1-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="3e3d1-106">V prípade blokovaných prichádzajúcich správ, na ktorých môžete ovládať zdrojový e-mailový server, je potrebné určiť príčinu a odstrániť blok z webovej lokality spamhaus.</span><span class="sxs-lookup"><span data-stu-id="3e3d1-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="3e3d1-107">V prípade blokovaných prichádzajúcich správ, v ktorých je zdrojová IP adresa členom inej osoby, musí vlastník adresy odstrániť blok z webovej lokality spamhaus.</span><span class="sxs-lookup"><span data-stu-id="3e3d1-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="3e3d1-108">Ak sa IP adresa nachádza v zozname blok politiky (PBL), vlastník môže priradiť inú statickú IP adresu alebo odstrániť adresu z poľa PBL.</span><span class="sxs-lookup"><span data-stu-id="3e3d1-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="3e3d1-109">V prípade blokovaných odchádzajúcich správ z vašej domény pripojenej k spoločnosti Microsoft sa môže táto chyba Zobraziť, ak sú správy smerované prostredníctvom služby tretích strán.</span><span class="sxs-lookup"><span data-stu-id="3e3d1-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="3e3d1-110">Pomocou nástroja vyhľadávania WHOIS môžete nájsť blokovaných vlastníkov IP adries.</span><span class="sxs-lookup"><span data-stu-id="3e3d1-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>

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
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/22/2019
ms.locfileid: "30761648"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="23430-102">Chyba pri odosielaní e-mailu: klienta hostiteľa blokovaný pomocou Spamhaus</span><span class="sxs-lookup"><span data-stu-id="23430-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="23430-103">IP adresu, ktorá správu odoslala sa na zoznam zablokovaných vlastníctve [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="23430-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="23430-104">Príčiny pre blokovaný Spamhaus prelomených účtov, ohrozená stroje zdieľanie verejnú IP adresu, a podmienky Internet Service Provider (ISP).</span><span class="sxs-lookup"><span data-stu-id="23430-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="23430-105">Možné opravy sú:</span><span class="sxs-lookup"><span data-stu-id="23430-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="23430-106">Pre blokované prichádzajúce správy do služieb Office 365, kde ovládate zdroj e-mailový server, musíte určiť príčinu a odstrániť blok z internetovej Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="23430-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="23430-107">Blokované prichádzajúce správy do služby Office 365 kde zdrojová adresa IP patrí niekomu inému, adresa vlastníka treba odstrániť blok z internetovej Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="23430-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="23430-108">Ak je adresa IP na politiku blokovať zoznamu (PBL), vlastník môžete priradiť rôzne statickú IP adresu alebo odstráňte adresu zo PBL.</span><span class="sxs-lookup"><span data-stu-id="23430-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="23430-109">Blokované odchádzajúce správy z vašej domény Office 365, môžete dostať túto chybu, ak správy sú smerované prostredníctvom 3rd party servis.</span><span class="sxs-lookup"><span data-stu-id="23430-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="23430-110">WHOIS lookup nástroj môžete použiť na vyhľadanie blokovaných IP adresa vlastníka.</span><span class="sxs-lookup"><span data-stu-id="23430-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    


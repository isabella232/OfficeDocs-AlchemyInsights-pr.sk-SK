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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="a4bef-102">Chyba pri odosielaní e-mailu: klient hostiteľa blokovaný pomocou spamhaus</span><span class="sxs-lookup"><span data-stu-id="a4bef-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="a4bef-103">Adresa IP, ktorá odoslala správu, sa nachádza na zozname blokovaných položiek, ktorý vlastní [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="a4bef-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="a4bef-104">Dôvody pre blokovanie spamhaus zahŕňajú kompromitovaných účtov, ohrozená stroje zdieľanie verejnej IP adresu a Internet Service Provider (ISP) politiky.</span><span class="sxs-lookup"><span data-stu-id="a4bef-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="a4bef-105">Možné opravy sú:</span><span class="sxs-lookup"><span data-stu-id="a4bef-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="a4bef-106">Pre blokované prichádzajúce správy, kde ovládate zdrojový e-mailový server, musíte určiť príčinu a odstrániť blok z webovej stránky spamhaus.</span><span class="sxs-lookup"><span data-stu-id="a4bef-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="a4bef-107">Pre blokované prichádzajúce správy, kde zdrojová adresa IP patrí niekomu inému, vlastník adresy musí odstrániť blok z webovej stránky spamhaus.</span><span class="sxs-lookup"><span data-stu-id="a4bef-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="a4bef-108">Ak je adresa IP v zozname blokovaných politík (PBL), vlastník môže priradiť inú statickú adresu IP alebo odstrániť adresu z PBL.</span><span class="sxs-lookup"><span data-stu-id="a4bef-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="a4bef-109">Pre blokované odchádzajúce správy z domény pripojenej k spoločnosti Microsoft, môžete získať túto chybu, ak správy sú smerované prostredníctvom 3rd party služby.</span><span class="sxs-lookup"><span data-stu-id="a4bef-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="a4bef-110">Na vyhľadanie zablokovaného vlastníka adresy IP môžete použiť vyhľadávací nástroj WHOIS.</span><span class="sxs-lookup"><span data-stu-id="a4bef-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>

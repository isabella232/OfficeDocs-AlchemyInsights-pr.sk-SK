---
title: Ochrana pred útokom nevyžiadané
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037178"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="05ecf-102">Ochrana pred útokom nevyžiadané</span><span class="sxs-lookup"><span data-stu-id="05ecf-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="05ecf-103">Nevyžiadané je hlásenie o nedoručení (známe aj ako oznámenia o nedoručení alebo odraziť správy), ktoré ste prijali pre správy, ktoré ste neodoslali.</span><span class="sxs-lookup"><span data-stu-id="05ecf-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="05ecf-104">Spameri Forge (spoof) **z:** adresa svojich správ a často používajú skutočné e-mailové adresy na zaručenie dôveryhodnosti svojich správ.</span><span class="sxs-lookup"><span data-stu-id="05ecf-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="05ecf-105">Ak však spameri nevyhnutne odosielajú správy neexistujúcim príjemcom, cieľový e-mailový server je v podstate podriadený vráteniu nedoručiteľnej správy v oznámení o nedoručení sfalšovanému odosielateľovi v adrese **od:** .</span><span class="sxs-lookup"><span data-stu-id="05ecf-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="05ecf-106">Ďalšie informácie nájdete v [nevyžiadané v službe EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span><span class="sxs-lookup"><span data-stu-id="05ecf-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="05ecf-107">**Povolenie ochrany nevyžiadané**</span><span class="sxs-lookup"><span data-stu-id="05ecf-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="05ecf-108">Ak chcete zapnúť ochranu nevyžiadané, postupujte podľa nižšie uvedenej cesty.</span><span class="sxs-lookup"><span data-stu-id="05ecf-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="05ecf-109">**protection.office.com > > politiky > antispam > vyberte politiku filtrovania nevyžiadanej pošty a upravte politiku > vlastnosti nevyžiadanej pošty > označiť ako nevyžiadanú poštu > NDR nevyžiadané > nastavte na možnosť zapnuté.**</span><span class="sxs-lookup"><span data-stu-id="05ecf-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="05ecf-110">Ak sa domnievate, že konto bolo zneužité, pozrite si tieto témy:</span><span class="sxs-lookup"><span data-stu-id="05ecf-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="05ecf-111">Odpovedanie na kompromisné e-mailové konto</span><span class="sxs-lookup"><span data-stu-id="05ecf-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="05ecf-112">Odstránenie blokovaných používateľov z portálu s obmedzenými používateľmi v Office 365</span><span class="sxs-lookup"><span data-stu-id="05ecf-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)




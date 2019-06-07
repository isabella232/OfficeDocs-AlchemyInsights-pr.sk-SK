---
title: 1332 OWA - doručenej pošty pravidiel sa nevykonáva pre poštovú schránku
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 28b03183552e00dd2522fff51b061cc27d5032ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762238"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="c1eee-102">Pravidlo pre doručenú poštu nefunguje podľa očakávania</span><span class="sxs-lookup"><span data-stu-id="c1eee-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="c1eee-103">Skontrolujte nasledujúce nastavenia:</span><span class="sxs-lookup"><span data-stu-id="c1eee-103">Verify the following settings:</span></span>

- <span data-ttu-id="c1eee-104">Môžu byť presmerované správy poslanej ďalej alebo v odpovediach na automaticky na základe pravidiel pre doručenú poštu iba raz.</span><span class="sxs-lookup"><span data-stu-id="c1eee-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="c1eee-105">Presmerovanie pravidlo (pravidlo priečinka doručenej pošty alebo pošty tok pravidlo, tiež známy ako pravidlo prenosu) môžete pridať maximálne desať presmerovanie príjemcov správy.</span><span class="sxs-lookup"><span data-stu-id="c1eee-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="c1eee-106">Ďalšie informácie, Zobraziť [Denník, dopravy, a Doručená pošta pravidlo obmedzuje](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="c1eee-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="c1eee-107">Pravidlá pre doručenú poštu nefungujú na alternatívne journaling schránku.</span><span class="sxs-lookup"><span data-stu-id="c1eee-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="c1eee-108">Ďalšie informácie o alternatívny journaling schránky, pozri [alternatívne journaling schránku](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="c1eee-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="c1eee-109">Ak chcete vyriešiť tieto problémy, pozri [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="c1eee-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="c1eee-110">Ak predchádzajúcich vydaniach neuplatníte, spustiť diagnostická zostava pravidlo priečinka doručenej pošty, pred eskalovat vydanie Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="c1eee-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="c1eee-111">Otvorte poštovú schránku v Outlooku na webe, a kliknite na položku **Nastavenie** \> **Možnosti** \> **Usporiadať e-mail** \> **pravidlá pre doručenú poštu**.</span><span class="sxs-lookup"><span data-stu-id="c1eee-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="c1eee-112">V spodnej časti stránky, kliknite na tlačidlo **Ak vaše pravidlá nefungujú kliknite tu pre generovanie diagnostickej zostavy**.</span><span class="sxs-lookup"><span data-stu-id="c1eee-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>

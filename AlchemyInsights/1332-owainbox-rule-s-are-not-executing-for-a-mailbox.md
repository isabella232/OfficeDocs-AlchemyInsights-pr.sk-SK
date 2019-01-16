---
title: 1332 OWA - doručenej pošty pravidiel sa nevykonáva pre poštovú schránku
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2019
ms.locfileid: "28311542"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="d4a58-102">Pravidlo pre doručenú poštu nefunguje podľa očakávania</span><span class="sxs-lookup"><span data-stu-id="d4a58-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="d4a58-103">Skontrolujte nasledujúce nastavenia:</span><span class="sxs-lookup"><span data-stu-id="d4a58-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="d4a58-p101">Môžu byť presmerované správy poslanej ďalej alebo v odpovediach na automaticky na základe pravidiel pre doručenú poštu iba raz. Presmerovanie pravidlo (pravidlo priečinka doručenej pošty alebo pošty tok pravidlo, tiež známy ako pravidlo prenosu) môžete pridať maximálne desať presmerovanie príjemcov správy. Ďalšie informácie, Zobraziť [Denník, dopravy, a Doručená pošta pravidlo obmedzuje](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span><span class="sxs-lookup"><span data-stu-id="d4a58-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="d4a58-p102">Pravidlá pre doručenú poštu nefungujú na alternatívne journaling schránku. Ďalšie informácie o alternatívny journaling schránky, pozri [alternatívne journaling schránku](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span><span class="sxs-lookup"><span data-stu-id="d4a58-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="d4a58-109">Ak chcete vyriešiť tieto problémy, pozri [KB 2829319](https://support.microsoft.com/kb/2829319).</span><span class="sxs-lookup"><span data-stu-id="d4a58-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="d4a58-110">Ak predchádzajúcich vydaniach neuplatníte, spustiť diagnostická zostava pravidlo priečinka doručenej pošty, pred eskalovat vydanie Microsoft Support:</span><span class="sxs-lookup"><span data-stu-id="d4a58-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="d4a58-111">Otvorte poštovú schránku v Outlooku na webe, a kliknite na položku **Nastavenie** \> **Možnosti** \> **Usporiadať e-mail** \> **pravidlá pre doručenú poštu**.</span><span class="sxs-lookup"><span data-stu-id="d4a58-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="d4a58-112">V spodnej časti stránky, kliknite na tlačidlo **Ak vaše pravidlá nefungujú kliknite tu pre generovanie diagnostickej zostavy**.</span><span class="sxs-lookup"><span data-stu-id="d4a58-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    


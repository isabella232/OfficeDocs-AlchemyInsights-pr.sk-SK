---
title: Riešenie problémov s overním SMTP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826430"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="c299b-102">Riešenie problémov s overním SMTP</span><span class="sxs-lookup"><span data-stu-id="c299b-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="c299b-103">Ak sa pri pokuse o odoslanie e-mailu SMTP a overenie pomocou klienta alebo aplikácie zobrazí chyba 5.7.57 alebo 5.7.3, mali by ste skontrolovať niekoľko vecí:</span><span class="sxs-lookup"><span data-stu-id="c299b-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="c299b-104">Overené odosielanie SMTP servera môže byť v nájomníkovi vypnuté alebo v poštovej schránke, ktorú sa pokúšate použiť (skontrolujte obe nastavenia).</span><span class="sxs-lookup"><span data-stu-id="c299b-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="c299b-105">Ďalšie informácie nájdete v téme [Zapnutie alebo vypnutie odoslaného overeného klienta SMTP.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="c299b-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="c299b-106">Skontrolujte, [či sú pre vášho nájomníka](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) povolené predvolené nastavenia zabezpečenia služby Azure. ak je povolené, overenie SMTP pomocou základného overovania (známe aj ako staršie verzie), ktoré použije meno používateľa a heslo, zlyhá.</span><span class="sxs-lookup"><span data-stu-id="c299b-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>

---
title: Fond prenosu odchádzajúcich prenosov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381862"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="12b7c-102">Fond prenosu odchádzajúcich prenosov</span><span class="sxs-lookup"><span data-stu-id="12b7c-102">Outbound relay pool</span></span>

<span data-ttu-id="12b7c-103">Spoločnosť Microsoft v konfigurácii robí určité zmeny týkajúce sa prenosu alebo preposielania e-mailov prostredníctvom Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="12b7c-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="12b7c-104">Správy sa v určitých situáciách preposielajú alebo prenášajú Microsoft 365 prostredníctvom špeciálneho fondu prenosov.</span><span class="sxs-lookup"><span data-stu-id="12b7c-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="12b7c-105">Správy odoslané pomocou fondu prenosu údajov môžu skončiť v priečinku nevyžiadanej pošty príjemcu.</span><span class="sxs-lookup"><span data-stu-id="12b7c-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="12b7c-106">Ďalšie informácie nájdete v téme [Výstupné fondy doručovania](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="12b7c-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="12b7c-107">Ak sa chcete vyhnúť scenáru používania fondu prenosov, uistite sa, že preposlané alebo presmerované správy spĺňajú jedno z nasledujúcich kritérií:</span><span class="sxs-lookup"><span data-stu-id="12b7c-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="12b7c-108">Výstupný odosielateľ je akceptovaná doména nájomníka.</span><span class="sxs-lookup"><span data-stu-id="12b7c-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="12b7c-109">SPF (Sender Policy Framework) prejde v čase, keď sa správa Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="12b7c-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="12b7c-110">DomainKeys Identified Mail (DKIM) v doméne odosielateľa P2 prejde, keď sa správa Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="12b7c-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="12b7c-111">Správy, ktoré spĺňajú vyššie uvedené kritériá, nie sú prenášané prostredníctvom fondu prenosov.</span><span class="sxs-lookup"><span data-stu-id="12b7c-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="12b7c-112">Ak je MX záznam pre vašu doménu určený pre tretí alebo lokálny server, použite rozšírené filtrovanie, aby ste sa uistili, že pre prichádzajúce e-maily je správne overenie SPF, a vyhnete sa odosielaniu e-mailov prostredníctvom fondu prenosov.</span><span class="sxs-lookup"><span data-stu-id="12b7c-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="12b7c-113">**Ako zistiť, či je na nás vplyv fond prenosu?**</span><span class="sxs-lookup"><span data-stu-id="12b7c-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="12b7c-114">Ak preposlané alebo presmerované e-maily používajú jedno z vyššie uvedených kritérií, správy sa nebudú prenášať prostredníctvom fondu prenosov.</span><span class="sxs-lookup"><span data-stu-id="12b7c-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="12b7c-115">Ak sa však správa odošle prostredníctvom fondu prenosu, IP server odchádzajúcej pošty je v rozsahu 40.95.0.0/16 a názov servera odchádzajúcej pošty obsahuje v názov **rly.**</span><span class="sxs-lookup"><span data-stu-id="12b7c-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>


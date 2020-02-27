---
title: Vytvoriť email chytiť všetky
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286306"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="e7862-102">Vytvoriť email chytiť všetky</span><span class="sxs-lookup"><span data-stu-id="e7862-102">Create an email catch all</span></span>

<span data-ttu-id="e7862-103">Použitie úlovku všetko je silne odradiť.</span><span class="sxs-lookup"><span data-stu-id="e7862-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="e7862-104">Je lepšie poskytnúť odskočiť späť odosielateľovi nájmu odosielateľom vedieť, že ich správa nemohla byť doručená, ako je určené, aby mohli podniknúť kroky.</span><span class="sxs-lookup"><span data-stu-id="e7862-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="e7862-105">Môžete tiež obmedziť sledované poštovej schránky len chytiť predtým platné e-mailové adresy.</span><span class="sxs-lookup"><span data-stu-id="e7862-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="e7862-106">Akékoľvek chytiť všetky schránky dostane veľa spamu a môže nakoniec vyplniť, ak nie pozorne sledovať.</span><span class="sxs-lookup"><span data-stu-id="e7862-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="e7862-107">(Tam sú prijímacie limity.)</span><span class="sxs-lookup"><span data-stu-id="e7862-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="e7862-108">Ak sa rozhodnete pokračovať, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="e7862-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="e7862-109">Vytvorte dynamickú distribučnú skupinu & zahrnúť "všetky typy príjemcov."</span><span class="sxs-lookup"><span data-stu-id="e7862-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="e7862-110">Vytvoriť vyhradenú poštovú schránku zachytiť e-maily, napríklad catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="e7862-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="e7862-111">Pre konkrétnu doménu, nastavte DomainType "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="e7862-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="e7862-112">Ak neskôr odstránite úlovok všetky, uistite sa, že nastaviť doménu späť na autoritatívne.</span><span class="sxs-lookup"><span data-stu-id="e7862-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="e7862-113">Vytvoriť pravidlo prenosu Mailflow takto:</span><span class="sxs-lookup"><span data-stu-id="e7862-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="e7862-114">Ak je odosielateľ "mimo organizácie"</span><span class="sxs-lookup"><span data-stu-id="e7862-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="e7862-115">Presmerovanie správy na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="e7862-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="e7862-116">Okrem prípadov, keď je príjemca členom allusers@domain.com (distribučná skupina obsahuje všetkých členov)</span><span class="sxs-lookup"><span data-stu-id="e7862-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="e7862-117">Overte, či sa nové poštové schránky pridajú do dynamickej distribučnej skupiny</span><span class="sxs-lookup"><span data-stu-id="e7862-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>

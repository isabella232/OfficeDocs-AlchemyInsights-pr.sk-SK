---
title: Vytvorenie e-mailu na zachytenie všetkých
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816215"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="42d63-102">Vytvorenie e-mailu na zachytenie všetkých</span><span class="sxs-lookup"><span data-stu-id="42d63-102">Create an email catch all</span></span>

<span data-ttu-id="42d63-103">Použitie všetkých záchytných údajov sa dôrazne neodporúča.</span><span class="sxs-lookup"><span data-stu-id="42d63-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="42d63-104">Je lepšie vrátiť sa odosielateľovi, ktorý odosielateľovi dá vedieť, že sa ich správa nemôže doručiť ako adresa, aby mohol prijať opatrenia.</span><span class="sxs-lookup"><span data-stu-id="42d63-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="42d63-105">Monitorovanú poštovú schránku môžete obmedziť iba na predtým platné e-mailové adresy.</span><span class="sxs-lookup"><span data-stu-id="42d63-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="42d63-106">Každý úchylovok všetkých poštových schránok dostane veľa nevyžiadanej pošty a nakoniec sa môže vyplniť, ak nie je podrobne monitorovaný.</span><span class="sxs-lookup"><span data-stu-id="42d63-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="42d63-107">(Prijímacie limity.)</span><span class="sxs-lookup"><span data-stu-id="42d63-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="42d63-108">Ak sa rozhodnete pokračovať, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="42d63-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="42d63-109">Vytvorte dynamickú distribučnú skupinu& obsahuje položku Všetky typy príjemcov.</span><span class="sxs-lookup"><span data-stu-id="42d63-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="42d63-110">Vytvorte vyhradenú poštovú schránku na zachytenie e-mailov, napríklad catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="42d63-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="42d63-111">Pre konkrétnu doménu nastavte položku DomainType na možnosť InternalRelay.</span><span class="sxs-lookup"><span data-stu-id="42d63-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="42d63-112">Ak neskôr odstránite všetky, uistite sa, že ste doménu nastavili späť na možnosť Autoritatívny.</span><span class="sxs-lookup"><span data-stu-id="42d63-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="42d63-113">Pravidlo prenosu mailflow je možné vytvoriť takto:</span><span class="sxs-lookup"><span data-stu-id="42d63-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="42d63-114">Ak je odosielateľ "Mimo organizácie"</span><span class="sxs-lookup"><span data-stu-id="42d63-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="42d63-115">Presmerovať správu na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="42d63-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="42d63-116">Okrem prípadov, keď je príjemca členom člena allusers@domain.com (distribučná skupina obsahuje všetkých členov)</span><span class="sxs-lookup"><span data-stu-id="42d63-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="42d63-117">Overenie pridania nových poštových schránok do dynamickej distribučnej skupiny</span><span class="sxs-lookup"><span data-stu-id="42d63-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>

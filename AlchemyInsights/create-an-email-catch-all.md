---
title: Vytvorenie e-mailového úlovku všetkých
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713001"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="a828f-102">Vytvorenie e-mailového úlovku všetkých</span><span class="sxs-lookup"><span data-stu-id="a828f-102">Create an email catch all</span></span>

<span data-ttu-id="a828f-103">Používanie všetkých úlovkov je silne odradzované.</span><span class="sxs-lookup"><span data-stu-id="a828f-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="a828f-104">Je lepšie poskytnúť odskočiť späť odosielateľovi, ktorí odosielajú odosielateľovi, že ich správa sa nedá dodať ako adresovaná, aby mohli konať.</span><span class="sxs-lookup"><span data-stu-id="a828f-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="a828f-105">Môžete tiež obmedziť sledovanú poštovú schránku, aby sa len chytiť predtým platné e-mailové adresy.</span><span class="sxs-lookup"><span data-stu-id="a828f-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="a828f-106">Akýkoľvek úlovok všetky poštovej schránky dostane veľa nevyžiadanej pošty a môže nakoniec vyplniť, ak nie pozorne sledovať.</span><span class="sxs-lookup"><span data-stu-id="a828f-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="a828f-107">(Dostávajú sa limity.)</span><span class="sxs-lookup"><span data-stu-id="a828f-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="a828f-108">Ak sa rozhodnete pokračovať, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="a828f-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="a828f-109">Vytvorenie dynamickej distribučnej skupiny & zahrnúť všetky typy príjemcov.</span><span class="sxs-lookup"><span data-stu-id="a828f-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="a828f-110">Vytvorte vyhradenú poštovú schránku na zachytenie e-mailov, napríklad catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="a828f-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="a828f-111">Pre konkrétnu doménu nastavte DomainType na "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="a828f-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="a828f-112">Ak neskôr odstránite všetky úlovky, nezabudnite nastaviť doménu späť na autoritatívne.</span><span class="sxs-lookup"><span data-stu-id="a828f-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="a828f-113">Vytvorte pravidlo prenosu Poštyhttps://Configure.Office.com/scenario.aspx?sid=12 takto:</span><span class="sxs-lookup"><span data-stu-id="a828f-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="a828f-114">Ak sa odosielateľ nachádza mimo organizácie</span><span class="sxs-lookup"><span data-stu-id="a828f-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="a828f-115">Presmerovať správu na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="a828f-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="a828f-116">Okrem prípadov, keď je príjemca členom allusers@domain.com (distribučná skupina obsahuje všetkých členov)</span><span class="sxs-lookup"><span data-stu-id="a828f-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="a828f-117">Overenie pridávania nových poštových schránok do dynamickej distribučnej skupiny</span><span class="sxs-lookup"><span data-stu-id="a828f-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>

---
title: Odchod do dôchodku Legacy eDiscovery nástroje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157708"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="6e71f-102">Odchod do dôchodku Legacy eDiscovery nástroje</span><span class="sxs-lookup"><span data-stu-id="6e71f-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="6e71f-103">V dôsledku nových a vylepšených funkcií eDiscovery v Microsoft 365 Compliance Center, nasledujúce staršie eDiscovery nástroje a commandlets bude dôchodku v najbližších mesiacoch:</span><span class="sxs-lookup"><span data-stu-id="6e71f-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="6e71f-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) a [in-miesto drží](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v Exchange Admin Center.</span><span class="sxs-lookup"><span data-stu-id="6e71f-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="6e71f-105">Rutiny cmdlet prostredia Exchange Online PowerShell, ktoré podporujú in-Place eDiscovery a na mieste drží.</span><span class="sxs-lookup"><span data-stu-id="6e71f-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="6e71f-106">(Tieto rutiny cmdlet sú súhrnne identifikované ako \*-MailboxSearch rutiny cmdlet.) To zahŕňa nasledujúce rutiny cmdlet:</span><span class="sxs-lookup"><span data-stu-id="6e71f-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="6e71f-107">Nové-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="6e71f-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="6e71f-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="6e71f-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="6e71f-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="6e71f-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="6e71f-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="6e71f-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="6e71f-111">Rutiny cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v prostredí Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6e71f-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="6e71f-112">Nasledujúce operácie v rozhraní API webových služieb Exchange:</span><span class="sxs-lookup"><span data-stu-id="6e71f-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="6e71f-113">Getsearchablepoštové schránky</span><span class="sxs-lookup"><span data-stu-id="6e71f-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="6e71f-114">Setholdonpoštové schránky</span><span class="sxs-lookup"><span data-stu-id="6e71f-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="6e71f-115">Getholdonpoštové schránky</span><span class="sxs-lookup"><span data-stu-id="6e71f-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="6e71f-116">Office 365 Advanced eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="6e71f-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="6e71f-117">**Časová os pre odchod do dôchodku**:</span><span class="sxs-lookup"><span data-stu-id="6e71f-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="6e71f-118">1. apríla, 2020: nebudete môcť vytvárať nové vyhľadávania a zadržania, ale stále môžete spúšťať, upravovať a odstraňovať existujúce vyhľadávania na vlastné riziko.</span><span class="sxs-lookup"><span data-stu-id="6e71f-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="6e71f-119">Microsoft Support už nebude podporovať in-Place eDiscovery & drží v EAC.</span><span class="sxs-lookup"><span data-stu-id="6e71f-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="6e71f-120">1. júl 2020: in-Place eDiscovery & drží funkčnosť v EAC budú umiestnené v Read-Only režime.</span><span class="sxs-lookup"><span data-stu-id="6e71f-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="6e71f-121">To znamená, že budete môcť odstrániť len existujúce vyhľadávania a ich podržaní.</span><span class="sxs-lookup"><span data-stu-id="6e71f-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="6e71f-122">**Ďalšie informácie nájdete v téme**:</span><span class="sxs-lookup"><span data-stu-id="6e71f-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="6e71f-123">Migrovať staršie eDiscovery vyhľadávania a drží na Microsoft 365 Compliance Center</span><span class="sxs-lookup"><span data-stu-id="6e71f-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="6e71f-124">Odchod do dôchodku Legacy eDiscovery nástroje</span><span class="sxs-lookup"><span data-stu-id="6e71f-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="6e71f-125">Najčastejšie otázky o in-Place eDiscovery a in-Place drží</span><span class="sxs-lookup"><span data-stu-id="6e71f-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




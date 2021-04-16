---
title: Vyradenie starších nástrojov vyhľadávania eDiscovery
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798564"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="899b5-102">Vyradenie starších nástrojov vyhľadávania eDiscovery</span><span class="sxs-lookup"><span data-stu-id="899b5-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="899b5-103">V dôsledku novej a vylepšenej funkcie eDiscovery v centre dodržiavania súladu pre Microsoft 365 sa v nadchádzajúcich mesiacoch tieto staršie nástroje a commandlety služby eDiscovery prepustia:</span><span class="sxs-lookup"><span data-stu-id="899b5-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="899b5-104">[Miestne blokovanie eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [a miestne blokovanie blokovania](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v Centre spravovania pre Exchange.</span><span class="sxs-lookup"><span data-stu-id="899b5-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="899b5-105">Rutiny typu cmdlet prostredia PowerShell služby Exchange Online, ktoré In-Place eDiscovery a blokovania In-Place blokovania údajov.</span><span class="sxs-lookup"><span data-stu-id="899b5-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="899b5-106">(Tieto rutiny typu cmdlet sa spolu identifikujú ako rutiny typu cmdlet \*-MailboxSearch.) Patria sem nasledujúce rutiny cmdlet:</span><span class="sxs-lookup"><span data-stu-id="899b5-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="899b5-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="899b5-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="899b5-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="899b5-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="899b5-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="899b5-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="899b5-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="899b5-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="899b5-111">Rutina typu cmdlet [search-mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v prostredí Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="899b5-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="899b5-112">Nasledujúce operácie v rozhraní API webových služieb Exchange:</span><span class="sxs-lookup"><span data-stu-id="899b5-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="899b5-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="899b5-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="899b5-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="899b5-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="899b5-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="899b5-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="899b5-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="899b5-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="899b5-117">**Časová os na vyradenie:**</span><span class="sxs-lookup"><span data-stu-id="899b5-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="899b5-118">**1. júla 2020** Už nemôžete vytvárať nové vyhľadávania a zadržanie, ale môžete spustiť, upraviť a odstrániť existujúce vyhľadávania na vlastné riziko.</span><span class="sxs-lookup"><span data-stu-id="899b5-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="899b5-119">Podpora spoločnosti Microsoft už nepodporuje In-Place eDiscovery & blokovania blokovania uchová v EAC.</span><span class="sxs-lookup"><span data-stu-id="899b5-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="899b5-120">Funkcie In-Place eDiscovery & Holds v EAC z **1. októbra 2020** sa umiestnia do režimu iba na čítanie, takže môžete odstrániť iba existujúce vyhľadávania a blokovania.</span><span class="sxs-lookup"><span data-stu-id="899b5-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="899b5-121">**Ďalšie informácie nájdete v téme:**</span><span class="sxs-lookup"><span data-stu-id="899b5-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="899b5-122">Migrácia starších vyhľadávaní eDiscovery a blokovania ich zadržania do Centra dodržiavania súladu pre Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="899b5-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="899b5-123">Vyradenie starších nástrojov vyhľadávania eDiscovery</span><span class="sxs-lookup"><span data-stu-id="899b5-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="899b5-124">Najčastejšie otázky o In-Place eDiscovery a In-Place blokovania elektronického vyhľadávania</span><span class="sxs-lookup"><span data-stu-id="899b5-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




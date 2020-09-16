---
title: Odchod starších nástrojov elektronického vyhľadávania
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
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727798"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="24190-102">Odchod starších nástrojov elektronického vyhľadávania</span><span class="sxs-lookup"><span data-stu-id="24190-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="24190-103">V dôsledku novej a vylepšenej funkcie elektronického vyhľadávania v centre dodržiavania súladu pre Microsoft 365 sa v nasledujúcich mesiacoch vyplatí nasledujúci starší nástroj eDiscovery a príkazové aplety:</span><span class="sxs-lookup"><span data-stu-id="24190-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="24190-104">[Miestne elektronické vyhľadávanie](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) a [miestne priestory](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) v centre spravovania pre Exchange.</span><span class="sxs-lookup"><span data-stu-id="24190-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="24190-105">Rutiny cmdlet prostredia PowerShell služby Exchange Online, ktoré podporujú miestne elektronické vyhľadávanie a miestne zadržania.</span><span class="sxs-lookup"><span data-stu-id="24190-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="24190-106">(Tieto rutiny typu cmdlet sa spoločne identifikujú ako rutiny cmdlet \*-MailboxSearch.) Zahŕňa tieto rutiny typu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="24190-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="24190-107">Nové – MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="24190-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="24190-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="24190-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="24190-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="24190-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="24190-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="24190-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="24190-111">Rutina cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) v prostredí Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="24190-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="24190-112">Nasledujúce operácie v rozhraní API webových služieb Exchange Web Services:</span><span class="sxs-lookup"><span data-stu-id="24190-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="24190-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="24190-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="24190-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="24190-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="24190-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="24190-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="24190-116">Rozšírené elektronické vyhľadávanie v 1.0</span><span class="sxs-lookup"><span data-stu-id="24190-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="24190-117">**Časová os na odchod do dôchodku**:</span><span class="sxs-lookup"><span data-stu-id="24190-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="24190-118">**1. júl 2020** Už nie je možné vytvárať nové vyhľadávania a zadržania, ale môžete spustiť, upraviť a odstrániť existujúce vyhľadávania na vlastné riziko.</span><span class="sxs-lookup"><span data-stu-id="24190-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="24190-119">Podpora spoločnosti Microsoft už nepodporuje miestne elektronické vyhľadávanie & v systéme EAC.</span><span class="sxs-lookup"><span data-stu-id="24190-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="24190-120">**1. október 2020** Miestne elektronické vyhľadávanie & zachová funkčnosť v systéme EAC sa umiestni do režimu iba na čítanie, takže môžete odstrániť iba existujúce vyhľadávania a zadržania.</span><span class="sxs-lookup"><span data-stu-id="24190-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="24190-121">**Ďalšie informácie nájdete v témach**:</span><span class="sxs-lookup"><span data-stu-id="24190-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="24190-122">Migrácia starších vyhľadávaní vyhľadávania eDiscovery a zadržania v centre zabezpečenia dodržiavania súladu pre Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="24190-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="24190-123">Odchod starších nástrojov elektronického vyhľadávania</span><span class="sxs-lookup"><span data-stu-id="24190-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="24190-124">Najčastejšie otázky týkajúce sa miestneho elektronického vyhľadávania a lokálnych zadržaní</span><span class="sxs-lookup"><span data-stu-id="24190-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)




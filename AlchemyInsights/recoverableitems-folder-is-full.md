---
title: 1336 RecoverableItems priečinok je plný
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: fb10b792981040bdcf4661b8aff30733c2438212
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720267"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="fe02c-102">Priečinok Obnoviteľné položky je plný</span><span class="sxs-lookup"><span data-stu-id="fe02c-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="fe02c-103">Pre poštové schránky Exchange Online je predvolený limit ukladacieho priestoru pre priečinok Obnoviteľné položky 30 GB.</span><span class="sxs-lookup"><span data-stu-id="fe02c-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="fe02c-104">Limit ukladacieho priestoru pre priečinok Obnoviteľné položky sa automaticky zvýši na 100 GB, ak poštová schránka je umiestnená v zadržanie, eDiscovery hold alebo je priradená politika uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="fe02c-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="fe02c-105">Keď priečinok Obnoviteľné položky dosiahne limit ukladacieho priestoru, funkčnosť poštovej schránky je ovplyvnená nasledujúcimi spôsobmi:</span><span class="sxs-lookup"><span data-stu-id="fe02c-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="fe02c-106">Používateľ nemôže odstrániť položky z poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="fe02c-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="fe02c-107">Asistent pre spravované priečinky nemôže odstrániť položky založené na značke uchovávania údajov alebo v nastaveniach spravovaných priečinkov.</span><span class="sxs-lookup"><span data-stu-id="fe02c-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="fe02c-108">V prípade poštových schránok, ktoré majú povolené obnovenie jednej položky alebo sú umiestnené na podržanie, proces ochrany stránky kopírovania na zápis nemôže zachovať verzie položiek upravených používateľom.</span><span class="sxs-lookup"><span data-stu-id="fe02c-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="fe02c-109">Pre poštové schránky, ktoré majú schránky auditu zapisovania do denníka zapnutá, žiadne položky denníka auditu poštovej schránky môžu byť uložené v podpriečinku audity v priečinku Obnoviteľné položky.</span><span class="sxs-lookup"><span data-stu-id="fe02c-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="fe02c-110">V prípade poštových schránok, ktoré nie sú podržaných, `Search-Mailbox -SearchDumpsterOnly -DeleteContent` môžu správcovia použiť príkaz v službe Exchange Online PowerShell na odstránenie položiek v priečinku Obnoviteľné položky.</span><span class="sxs-lookup"><span data-stu-id="fe02c-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="fe02c-111">Ďalšie informácie sa nachádzajú v týchto témach:</span><span class="sxs-lookup"><span data-stu-id="fe02c-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="fe02c-112">Vyhľadávanie a odstraňovanie správ</span><span class="sxs-lookup"><span data-stu-id="fe02c-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="fe02c-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="fe02c-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="fe02c-114">V prípade poštových schránok, ktoré sú podržaný, Správcovia musia odstrániť držanie pred odstránením položiek z priečinka Obnoviteľné položky.</span><span class="sxs-lookup"><span data-stu-id="fe02c-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="fe02c-115">Ďalšie informácie nájdete v téme [Odstránenie položiek v priečinku Obnoviteľné položky v poštových schránkach typu cloud na podržanie](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="fe02c-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="fe02c-116">Ak chcete zabrániť úplnému obnoveniu priečinka Obnoviteľné položky, správcovia môžu zvýšiť limit ukladacieho priestoru priečinka Obnoviteľné položky pre poštové schránky zadržaných a nastaviť politiku uchovávania poštových schránok, ktorá presunie položky z priečinka Obnoviteľné položky do archívnej poštovej schránky používateľa.</span><span class="sxs-lookup"><span data-stu-id="fe02c-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="fe02c-117">Pozrite si [zvýšenie kvóty pre obnoviteľné položky pre poštové schránky podržaných](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="fe02c-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>

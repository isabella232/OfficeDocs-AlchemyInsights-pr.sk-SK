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
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510767"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="858ff-102">Priečinok Obnoviteľné položky je plný</span><span class="sxs-lookup"><span data-stu-id="858ff-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="858ff-103">Pre poštové schránky služby Exchange Online je predvolený limit ukladacieho priestoru pre priečinok Obnoviteľné položky 30 GB.</span><span class="sxs-lookup"><span data-stu-id="858ff-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="858ff-104">Limit ukladacieho priestoru pre priečinok Obnoviteľné položky sa automaticky zvýši na 100 GB, ak je poštová schránka umiestnená v zadržaní v dôsledku súdneho sporu, zadržaní elektronického vyhľadávania alebo priradená k politike uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="858ff-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="858ff-105">Keď priečinok Obnoviteľné položky dosiahne limit ukladacieho priestoru, funkcie poštovej schránky je ovplyvnená nasledujúcimi spôsobmi:</span><span class="sxs-lookup"><span data-stu-id="858ff-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="858ff-106">Používateľ nemôže odstrániť položky z poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="858ff-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="858ff-107">Asistent pre spravované priečinky nemôže odstrániť položky na základe značky uchovávania údajov alebo nastavenia spravovaného priečinka.</span><span class="sxs-lookup"><span data-stu-id="858ff-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="858ff-108">Pre poštové schránky, ktoré majú jeden bod obnovenia zapnuté alebo sú umiestnené pouložené, proces ochrany stránky copy-on-write nemôže zachovať verzie položiek upravovaných používateľom.</span><span class="sxs-lookup"><span data-stu-id="858ff-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="858ff-109">Pre poštové schránky, ktoré majú poštovej schránky auditu zapisovania do denníka zapnuté, žiadne položky denníka auditu poštovej schránky môžu byť uložené v podpriečinku Audity v priečinku Obnoviteľné položky.</span><span class="sxs-lookup"><span data-stu-id="858ff-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="858ff-110">Pre poštové schránky, ktoré nie sú zadržané, správcovia môžu použiť `Search-Mailbox -SearchDumpsterOnly -DeleteContent` príkaz v prostredí Exchange Online PowerShell na odstránenie položiek v priečinku Obnoviteľné položky.</span><span class="sxs-lookup"><span data-stu-id="858ff-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="858ff-111">Ďalšie informácie sa nachádzajú v týchto témach:</span><span class="sxs-lookup"><span data-stu-id="858ff-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="858ff-112">Vyhľadávanie a odstraňovanie správ</span><span class="sxs-lookup"><span data-stu-id="858ff-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="858ff-113">Poštová schránka vyhľadávania</span><span class="sxs-lookup"><span data-stu-id="858ff-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="858ff-114">V prípade poštových schránok, ktoré sú zadržané, správcovia musia odstrániť zadržanie pred odstránením položiek z priečinka Obnoviteľné položky.</span><span class="sxs-lookup"><span data-stu-id="858ff-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="858ff-115">Ďalšie informácie sa nachádzajú v téme [Odstránenie položiek v priečinku Obnoviteľné položky poštových schránok typu cloud v zadržaných poštových schránkach typu cloud](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="858ff-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="858ff-116">S cieľom zabrániť tomu, aby sa priečinok Obnoviteľné položky nestal plným, správcovia môžu zvýšiť limit ukladacieho priestoru priečinka Obnoviteľné položky pre poštové schránky zadržané a nastaviť politiku uchovávania údajov poštovej schránky, ktorá presunie položky z priečinka Obnoviteľné položky do archívnej poštovej schránky používateľa.</span><span class="sxs-lookup"><span data-stu-id="858ff-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="858ff-117">Ďalšie informácie nájdete v téme [Zvýšenie kvóty Obnoviteľné položky pre poštové schránky v zadržaných poštových schránkach](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="858ff-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>

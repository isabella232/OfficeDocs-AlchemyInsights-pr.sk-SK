---
title: 1336 RecoverableItems priečinok je plný
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741282"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="f640e-102">Priečinok s využiteľnými položkami je plný</span><span class="sxs-lookup"><span data-stu-id="f640e-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="f640e-103">V prípade poštových schránok v službe Exchange Online je predvolený limit ukladacieho priestoru pre priečinok s využiteľnými položkami 30 GB.</span><span class="sxs-lookup"><span data-stu-id="f640e-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="f640e-104">Limit ukladacieho priestoru pre priečinok s využiteľnými položkami sa automaticky zvýši na 100 GB, ak je poštová schránka umiestnená v zadržaní zadržania, eDiscovery alebo je priradená k politike uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="f640e-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="f640e-105">Keď priečinok uhraditeľné položky dosiahne limit ukladacieho priestoru, funkčnosť poštovej schránky sa ovplyvní týmito spôsobmi:</span><span class="sxs-lookup"><span data-stu-id="f640e-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="f640e-106">Používateľ nemôže odstrániť položky z poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="f640e-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="f640e-107">Asistent pre spravované priečinky nedokáže odstrániť položky na základe značiek uchovávania údajov alebo spravovaného priečinka.</span><span class="sxs-lookup"><span data-stu-id="f640e-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="f640e-108">V prípade poštových schránok s možnosťou obnovenia jednej položky, ktoré sú povolené alebo sú podržané, proces ochrany stránky kopírovania a zápisu nemôže zachovať verzie položiek upravovaných používateľom.</span><span class="sxs-lookup"><span data-stu-id="f640e-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="f640e-109">V prípade poštových schránok, ktoré majú zapnuté zapisovanie do denníka auditu poštovej schránky, nie je možné uložiť žiadne položky denníka auditu poštovej schránky do podpriečinka auditov v priečinku uhraditeľné položky.</span><span class="sxs-lookup"><span data-stu-id="f640e-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="f640e-110">V prípade poštových schránok, ktoré nie sú zadržané, môžu správcovia použiť `Search-Mailbox -SearchDumpsterOnly -DeleteContent` príkaz v prostredí Exchange Online PowerShell na odstránenie položiek v priečinku uhraditeľné položky.</span><span class="sxs-lookup"><span data-stu-id="f640e-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="f640e-111">Ďalšie informácie sa nachádzajú v týchto témach:</span><span class="sxs-lookup"><span data-stu-id="f640e-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="f640e-112">Vyhľadanie a odstránenie správ</span><span class="sxs-lookup"><span data-stu-id="f640e-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="f640e-113">Vyhľadávanie – poštová schránka</span><span class="sxs-lookup"><span data-stu-id="f640e-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="f640e-114">V prípade poštových schránok, ktoré sú zadržané, musia správcovia pred odstránením položiek z priečinka s využiteľnými položkami odstrániť zadržanie.</span><span class="sxs-lookup"><span data-stu-id="f640e-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="f640e-115">Ďalšie informácie nájdete v téme [Odstránenie položiek v priečinku uhraditeľné položky v poštových schránkach v cloude zadržaných](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="f640e-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="f640e-116">Ak chcete zabrániť tomu, aby sa priečinok uhraditeľné položky stal úplným, správcovia môžu zvýšiť limit ukladacieho priestoru pre priečinok s využiteľnými položkami pre poštové schránky a nastaviť politiku uchovávania poštovej schránky, ktorá premiestni položky z priečinka využiteľné položky do archívnej poštovej schránky používateľa.</span><span class="sxs-lookup"><span data-stu-id="f640e-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="f640e-117">Pozrite si tému [zvýšenie kvóty uhraditeľných položiek pre poštové schránky v podržaní](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="f640e-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>

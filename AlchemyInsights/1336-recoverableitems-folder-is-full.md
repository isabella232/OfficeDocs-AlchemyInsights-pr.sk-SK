---
title: 1336 RecoverableItems priečinok je plný.
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: dbf4930c34e4175a14b77fab4eafc953bb37cc02
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29909303"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="9383d-102">Priečinok Obnoviteľné položky je plný</span><span class="sxs-lookup"><span data-stu-id="9383d-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="9383d-p101">Schránky Exchange Online v Office 365, predvolené ukladacieho priečinka Obnoviteľné položky je 30 GB. Ukladacieho priečinka Obnoviteľné položky sa automaticky zvýši na 100 GB, ak poštová schránka je umiestnený na zadržanie, podržte eDiscovery, alebo je priradená k politike uchovávania údajov služby Office 365.</span><span class="sxs-lookup"><span data-stu-id="9383d-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="9383d-105">Keď priečinka Obnoviteľné položky dosiahne limit ukladacieho priestoru, schránky funkčnosť je ovplyvnený nasledovnými spôsobmi:</span><span class="sxs-lookup"><span data-stu-id="9383d-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="9383d-106">Používateľa nemôžete odstrániť položky z poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="9383d-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="9383d-107">Asistent pre spravované priečinky nemožno odstrániť položky založené na značku uchovávania údajov alebo spravovaných priečinkov nastavenia.</span><span class="sxs-lookup"><span data-stu-id="9383d-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="9383d-108">Pre poštové schránky, ktoré majú jediný obnovenie položky zapnuté alebo sa odloží, procese ochrany kópiu na zápis stránky nemôže zachovať verzie položiek upravil používateľ.</span><span class="sxs-lookup"><span data-stu-id="9383d-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="9383d-109">Pre poštové schránky, ktoré majú zapnuté zapisovanie auditu poštovej schránky, žiadne položky denníka auditu poštovej schránky môžu byť uložené v podpriečinku auditov v priečinku Obnoviteľné položky.</span><span class="sxs-lookup"><span data-stu-id="9383d-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="9383d-p102">Pre poštové schránky, ktoré nie sú zadržané, správcovia môžu použiť `Search-Mailbox -SearchDumpsterOnly -DeleteContent` príkaz Exchange Online PowerShell odstrániť položky v priečinku Obnoviteľné položky. Ďalšie informácie nájdete v nasledujúcich témach:</span><span class="sxs-lookup"><span data-stu-id="9383d-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="9383d-112">Vyhľadanie a odstránenie správ</span><span class="sxs-lookup"><span data-stu-id="9383d-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="9383d-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="9383d-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="9383d-p103">Pre poštové schránky, ktoré sú podržané, správcovia majú odstrániť hold, ako budú môcť odstránené položky z priečinka Obnoviteľné položky. Ďalšie informácie nájdete v téme [odstrániť položky Obnoviteľné položky priečinka poštovými schránkami na držať](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="9383d-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="9383d-p104">Zabrániť stáva plne priečinka Obnoviteľné položky, správcovia môžu zvýšiť limit pre skladovanie Obnoviteľné položky priečinka poštové schránky na držať a nastaviť politiku uchovávania údajov poštovej schránky, ktoré premiestni položky z priečinka Obnoviteľné položky používateľa Archív Poštová schránka. Vidieť [zvýšenie Obnoviteľné položky kvóty poštových schránok na hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="9383d-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  


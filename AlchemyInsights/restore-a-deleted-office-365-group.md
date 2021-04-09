---
title: Obnovenie odstránenej skupiny Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645146"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="a3a5d-102">Obnovenie odstránenej skupiny Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a3a5d-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="a3a5d-103">Odstránenú skupinu v Microsoft 365 alebo aplikáciu Microsoft Teams môžete obnoviť do 30 dní od odstránenia.</span><span class="sxs-lookup"><span data-stu-id="a3a5d-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="a3a5d-104">Prejdite do [Centra spravovania služby Microsoft 365](https://aka.ms/RestoreDeletedGroup) a prihláste sa do zoznamu odstránených skupín a tímov.</span><span class="sxs-lookup"><span data-stu-id="a3a5d-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="a3a5d-105">**Poznámka:** Prihláste sa pomocou konta, ktoré je priradené správcovi nájomníkovi alebo k role správcu skupín.</span><span class="sxs-lookup"><span data-stu-id="a3a5d-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="a3a5d-106">Vyberte odstránenú skupinu alebo aplikáciu Microsoft 365/Teams, ktorá sa má obnoviť, a kliknite na **položku Obnoviť skupinu**.</span><span class="sxs-lookup"><span data-stu-id="a3a5d-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="a3a5d-107">Ak skupinu nemožno obnoviť z dôvodu konfliktnej adresy SMTP, pomocou nasledujúceho príkazu vyhľadajte objekt, ktorý je príčinou konfliktu, a odstráňte adresu SMTP:</span><span class="sxs-lookup"><span data-stu-id="a3a5d-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="a3a5d-108">**Poznámka:** V niektorých prípadoch môže trvať až 24 hodín, kým sa skupina a všetky jej údaje obnovia.</span><span class="sxs-lookup"><span data-stu-id="a3a5d-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="a3a5d-109">Ďalšie informácie alebo informácie o obnovení skupín pomocou prostredia PowerShell nájdete v téme Obnovenie [odstránenej skupiny v službe Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="a3a5d-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>
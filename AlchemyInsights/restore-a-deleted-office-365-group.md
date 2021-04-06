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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597458"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="e18c3-102">Obnovenie odstránenej skupiny Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e18c3-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="e18c3-103">Odstránenú skupinu v Microsoft 365 alebo aplikáciu Microsoft Teams môžete obnoviť do 30 dní od odstránenia.</span><span class="sxs-lookup"><span data-stu-id="e18c3-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="e18c3-104">Prejdite do Centra [spravovania služby Microsoft 365 a](https://aka.ms/RestoreDeletedGroup) prihláste sa do zoznamu odstránených skupín a tímov.</span><span class="sxs-lookup"><span data-stu-id="e18c3-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="e18c3-105">**Poznámka:** Prihláste sa pomocou konta, ktoré je priradené správcovi nájomníkovi alebo k role správcu skupín.</span><span class="sxs-lookup"><span data-stu-id="e18c3-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="e18c3-106">Vyberte odstránenú skupinu alebo aplikáciu Microsoft 365/Teams, ktorá sa má obnoviť, a kliknite na **položku Obnoviť skupinu**.</span><span class="sxs-lookup"><span data-stu-id="e18c3-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="e18c3-107">Ak skupinu nemožno obnoviť z dôvodu konfliktnej adresy SMTP, pomocou nasledujúceho príkazu vyhľadajte objekt, ktorý je príčinou konfliktu, a odstráňte adresu SMTP:</span><span class="sxs-lookup"><span data-stu-id="e18c3-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="e18c3-108">**Poznámka:** V niektorých prípadoch môže trvať až 24 hodín, kým sa skupina a všetky jej údaje obnovia.</span><span class="sxs-lookup"><span data-stu-id="e18c3-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="e18c3-109">Ďalšie informácie alebo informácie o obnovení skupín pomocou prostredia PowerShell nájdete v téme Obnovenie [odstránenej skupiny v službe Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="e18c3-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>
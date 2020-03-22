---
title: Nie je možné získať prístup k verejným priečinkom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891764"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="8c682-102">Program Outlook sa nemôže pripojiť k verejným priečinkom</span><span class="sxs-lookup"><span data-stu-id="8c682-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="8c682-103">Ak prístup k verejnému priečinku nefunguje niektorým používateľom, vyskúšajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="8c682-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="8c682-104">Pripojiť k EXO PowerShell a nakonfigurovať parameter DefaultPublicFolderMailbox na problémové používateľské konto, aby zodpovedali parametra na pracovné používateľské konto.</span><span class="sxs-lookup"><span data-stu-id="8c682-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="8c682-105">Príklad:</span><span class="sxs-lookup"><span data-stu-id="8c682-105">Example:</span></span>

<span data-ttu-id="8c682-106">Get-poštová schránka WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="8c682-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="8c682-107">Súbor schránky ProblemUser-DefaultPublicFolderMailbox \<hodnota z predchádzajúceho príkazu></span><span class="sxs-lookup"><span data-stu-id="8c682-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="8c682-108">Počkajte aspoň jednu hodinu, kým sa zmena prejaví.</span><span class="sxs-lookup"><span data-stu-id="8c682-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="8c682-109">Ak problém pretrváva, postupujte podľa [tohto postupu](https://aka.ms/pfcte) a Vyriešte problémy s prístupom k verejným priečinkom pomocou programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="8c682-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
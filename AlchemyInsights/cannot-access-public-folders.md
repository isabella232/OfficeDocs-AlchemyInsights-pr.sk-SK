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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959509"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="d9b66-102">Program Outlook sa nemôže pripojiť k verejným priečinkom</span><span class="sxs-lookup"><span data-stu-id="d9b66-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="d9b66-103">Ak prístup k verejnému priečinku nefunguje pre niekoľko používateľov, vyskúšajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="d9b66-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="d9b66-104">Pripojiť k EXO PowerShell a nakonfigurovať DefaultPublicFolderMailbox na problémové používateľské konto, aby zodpovedali jeden na pracovné používateľské konto.</span><span class="sxs-lookup"><span data-stu-id="d9b66-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="d9b66-105">Príklad:</span><span class="sxs-lookup"><span data-stu-id="d9b66-105">Example:</span></span>

<span data-ttu-id="d9b66-106">Get-poštová schránka WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="d9b66-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="d9b66-107">Súbor schránky ProblemUser-DefaultPublicFolderMailbox \<hodnota z predchádzajúceho príkazu></span><span class="sxs-lookup"><span data-stu-id="d9b66-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="d9b66-108">Počkajte aspoň jednu hodinu, kým sa zmena prejaví.</span><span class="sxs-lookup"><span data-stu-id="d9b66-108">Wait at least one hour for the change to take effect.</span></span>
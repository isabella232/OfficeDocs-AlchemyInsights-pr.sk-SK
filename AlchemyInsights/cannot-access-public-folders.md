---
title: Nie je možné získať prístup k verejným priečinkom
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819527"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="166b9-102">Outlook sa nemôže pripojiť k verejným priečinkom</span><span class="sxs-lookup"><span data-stu-id="166b9-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="166b9-103">Ak prístup do verejného priečinka nefunguje pre niektorých používateľov, vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="166b9-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="166b9-104">Pripojte sa k exo PowerShell a nakonfigurujte parameter DefaultPublicFolderMailbox v problémovom používateľskom konte tak, aby zodpovedal parametru v pracovnom používateľskom konte.</span><span class="sxs-lookup"><span data-stu-id="166b9-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="166b9-105">Príklad:</span><span class="sxs-lookup"><span data-stu-id="166b9-105">Example:</span></span>

<span data-ttu-id="166b9-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="166b9-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="166b9-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="166b9-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="166b9-108">Počkajte aspoň jednu hodinu, kým sa zmena prejaví.</span><span class="sxs-lookup"><span data-stu-id="166b9-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="166b9-109">Ak problém pretrváva, postupujte podľa tohto [postupu na riešenie problémov](https://aka.ms/pfcte) s prístupom do verejného priečinka pomocou Outlooku.</span><span class="sxs-lookup"><span data-stu-id="166b9-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="166b9-110">**Riadenie prístupu používateľov k verejným priečinkom pomocou Outlooku:**</span><span class="sxs-lookup"><span data-stu-id="166b9-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="166b9-111">Použitie Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true alebo $false</span><span class="sxs-lookup"><span data-stu-id="166b9-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="166b9-112">$true: Povolenie prístupu používateľov k verejným priečinkom v Outlooku</span><span class="sxs-lookup"><span data-stu-id="166b9-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="166b9-113">$false: Zabránenie prístupu používateľov k verejným priečinkom v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="166b9-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="166b9-114">Táto hodnota je predvolená.</span><span class="sxs-lookup"><span data-stu-id="166b9-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="166b9-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="166b9-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="166b9-116">**Poznámka** Týmto postupom môžete ovládať pripojenia iba k počítačovej aplikácii Outlook pre klientov s Windowsom.</span><span class="sxs-lookup"><span data-stu-id="166b9-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="166b9-117">Používateľ môže aj naďalej pristupovať k verejným priečinkom pomocou aplikácie OWA alebo Outlooku pre Mac.</span><span class="sxs-lookup"><span data-stu-id="166b9-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="166b9-118">Ďalšie informácie nájdete v téme [Oznámenie podpory kontrolovaných pripojení k verejným priečinkom v Outlooku.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="166b9-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>
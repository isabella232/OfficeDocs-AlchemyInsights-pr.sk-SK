---
title: Nie je možné získať prístup k verejným priečinkom
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812562"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="fbfba-102">Outlook sa nemôže pripojiť k verejným priečinkom</span><span class="sxs-lookup"><span data-stu-id="fbfba-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="fbfba-103">Ak prístup k verejným priečinkom nefunguje pre niektorých používateľov, vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="fbfba-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="fbfba-104">Pripojte sa k EXO PowerShell a nakonfigurujte parameter DefaultPublicFolderMailbox v používateľskom konte problém tak, aby zodpovedal parametru v pracovnom používateľskom konte.</span><span class="sxs-lookup"><span data-stu-id="fbfba-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="fbfba-105">Napríklad</span><span class="sxs-lookup"><span data-stu-id="fbfba-105">Example:</span></span>

<span data-ttu-id="fbfba-106">Prístup k poštovej schránke WorkingUser | ft DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="fbfba-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="fbfba-107">Nastavenie poštovej schránky ProblemUser – DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="fbfba-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="fbfba-108">Počkajte aspoň jednu hodinu, kým sa zmena prejaví.</span><span class="sxs-lookup"><span data-stu-id="fbfba-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="fbfba-109">Ak problém pretrváva, použite [Tento postup](https://aka.ms/pfcte) na riešenie problémov s prístupom k verejným priečinkom pomocou Outlooku.</span><span class="sxs-lookup"><span data-stu-id="fbfba-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="fbfba-110">**Ak chcete určiť, ktorí používatelia majú prístup k verejným priečinkom pomocou Outlooku**:</span><span class="sxs-lookup"><span data-stu-id="fbfba-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="fbfba-111">Použitie súpravy Set-CASMailbox <mailboxname> -PublicFolderClientAccess $True alebo $FALSE</span><span class="sxs-lookup"><span data-stu-id="fbfba-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="fbfba-112">$true: povolenie prístupu používateľov k verejným priečinkom v Outlooku</span><span class="sxs-lookup"><span data-stu-id="fbfba-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="fbfba-113">$false: zabránenie prístupu používateľov k verejným priečinkom v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="fbfba-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="fbfba-114">Táto hodnota je predvolená.</span><span class="sxs-lookup"><span data-stu-id="fbfba-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="fbfba-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="fbfba-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="fbfba-116">**Poznámka:** Tento postup umožňuje ovládať pripojenia iba pomocou počítačovej aplikácie Outlook pre klientov Windowsu.</span><span class="sxs-lookup"><span data-stu-id="fbfba-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="fbfba-117">Používateľ môže pokračovať v prístupe k verejným priečinkom pomocou aplikácie OWA alebo Outlooku pre Mac.</span><span class="sxs-lookup"><span data-stu-id="fbfba-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="fbfba-118">Ďalšie informácie nájdete v téme [oznámenie podpory spravovaných pripojení k verejným priečinkom v Outlooku](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="fbfba-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>
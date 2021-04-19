---
title: Riadenie prístupu k verejným priečinkom pomocou Outlooku
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816755"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="87475-102">Riadenie prístupu k verejným priečinkom pomocou Outlooku</span><span class="sxs-lookup"><span data-stu-id="87475-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="87475-103">Riadenie prístupu používateľov k verejným priečinkom pomocou Outlooku:</span><span class="sxs-lookup"><span data-stu-id="87475-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="87475-104">Použite `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="87475-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="87475-105">$true: Povolenie prístupu používateľov k verejným priečinkom v Outlooku</span><span class="sxs-lookup"><span data-stu-id="87475-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="87475-106">$false: Zabránenie prístupu používateľov k verejným priečinkom v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="87475-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="87475-107">Táto hodnota je predvolená.</span><span class="sxs-lookup"><span data-stu-id="87475-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="87475-108">Poznámka: Tento postup dokáže ovládať iba pripojenia k počítačovej aplikácii Outlook pre klientov s Windowsom.</span><span class="sxs-lookup"><span data-stu-id="87475-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="87475-109">Používatelia môžu aj naďalej pristupovať k verejným priečinkom pomocou aplikácie OWA alebo Outlooku pre Mac.</span><span class="sxs-lookup"><span data-stu-id="87475-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="87475-110">Ďalšie informácie nájdete v téme [Riadené pripojenia k verejným priečinkom v Outlooku.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="87475-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>

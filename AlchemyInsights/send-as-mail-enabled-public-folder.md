---
title: Verejný priečinok Odoslať ako E-mail v EXO
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
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/13/2020
ms.locfileid: "48462071"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="2501e-102">Verejný priečinok SendAs pošta</span><span class="sxs-lookup"><span data-stu-id="2501e-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="2501e-103">V nasledujúcom príklade sa priraďujú povolenia Odoslať ako pre verejný priečinok s podporou e-mailov pre NewPF1 používateľa Jason.</span><span class="sxs-lookup"><span data-stu-id="2501e-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="2501e-104">Add-RecipientPermission-identita ' NewPF1 '-správca "Jason"-AccessRights ' SendAs '</span><span class="sxs-lookup"><span data-stu-id="2501e-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="2501e-105">Podrobné informácie o syntaxi a parametroch nájdete v téme [Priradenie povolení Odoslať ako alebo Odoslať v mene pre verejné priečinky s podporou e-mailu](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="2501e-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>


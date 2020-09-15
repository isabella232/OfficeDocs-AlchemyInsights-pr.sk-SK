---
title: Zmena povolení pre verejný priečinok
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: a2a902e8fdfd8628772364c173979c633d25a169
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714262"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="b9c00-102">Zmena povolení pre verejný priečinok</span><span class="sxs-lookup"><span data-stu-id="b9c00-102">Changing public folder permissions</span></span>

<span data-ttu-id="b9c00-103">Povolenia pre verejný priečinok môžu meniť používatelia a správcovia v Outlooku.</span><span class="sxs-lookup"><span data-stu-id="b9c00-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="b9c00-104">Správcovia môžu tiež riadiť povolenia z centra spravovania pre Exchange (EAC) vykonaním týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="b9c00-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="b9c00-105">V centre spravovania služby Microsoft 365 prejdite na **Exchange centra spravovania** \> **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b9c00-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="b9c00-106">Vyberte položku **verejné priečinky**.</span><span class="sxs-lookup"><span data-stu-id="b9c00-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="b9c00-107">Odtiaľ môžete zmeniť povolenia pre jednotlivé verejné priečinky priradením skupín zabezpečenia k povoleniam.</span><span class="sxs-lookup"><span data-stu-id="b9c00-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="b9c00-108">Ak chcete, aby koncový používateľ zmenil povolenia verejného priečinka, používateľ musí mať v priečinku práva vlastníka.</span><span class="sxs-lookup"><span data-stu-id="b9c00-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="b9c00-109">Postupujte podľa postupu popísaného v [téme diagnostikovanie a oprava problémov s povolením verejného priečinka](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) na riešenie problémov s povolením verejného priečinka.</span><span class="sxs-lookup"><span data-stu-id="b9c00-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="b9c00-110">**Poznámka**: Existuje niekoľko známych problémov, ktoré sa môžu vyskytnúť pri pokuse o zmenu povolení pre verejné priečinky.</span><span class="sxs-lookup"><span data-stu-id="b9c00-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="b9c00-111">Ďalšie informácie nájdete v nasledujúcich článkoch.</span><span class="sxs-lookup"><span data-stu-id="b9c00-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="b9c00-112">Nie je možné použiť povolenia pre podpriečinky verejného priečinka v EAC</span><span class="sxs-lookup"><span data-stu-id="b9c00-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="b9c00-113">Pri prístupe k verejným priečinkom sa zobrazí chyba poštová schránka sa nenašla v lokálnom doménovom lese</span><span class="sxs-lookup"><span data-stu-id="b9c00-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)

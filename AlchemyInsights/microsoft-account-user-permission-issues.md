---
title: Riešenie problému – používateľ sa nenašiel v adresári
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725422"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="276c4-102">Riešenie problému – používateľ sa nenašiel v adresári</span><span class="sxs-lookup"><span data-stu-id="276c4-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="276c4-103">Ak sa používateľovi zobrazí chybové hlásenie "používateľ sa nenašiel" v adresári, skúste to znova, kde typ problému nie je používateľ v adresári.</span><span class="sxs-lookup"><span data-stu-id="276c4-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="276c4-104">Na vyriešenie problému je možné vykonať nasledujúce kroky.</span><span class="sxs-lookup"><span data-stu-id="276c4-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="276c4-105">Uistite sa, že konto, ktoré prijalo e-mailovú pozvánku, je rovnaké ako konto, ktoré sa používa na prihlásenie neskôr.</span><span class="sxs-lookup"><span data-stu-id="276c4-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="276c4-106">Uistite sa, že používateľ používa rovnaké konto na prijatie pozvania a prihlásenia na lokalitu.</span><span class="sxs-lookup"><span data-stu-id="276c4-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="276c4-107">Ďalšie informácie nájdete v téme [spravovanie aliasov konta Microsoft </a> na spravovanie prihlásenia do služby Microsoft 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="276c4-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="276c4-108">Prejdite na všetky lokality, v ktorých sa používateľovi zobrazuje chyba.</span><span class="sxs-lookup"><span data-stu-id="276c4-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="276c4-109">Pridajte text "/_layouts/15/People.aspx/MembershipGroupId = 0" (v rámci dvojitých úvodzoviek) na koniec URL adresy lokality.</span><span class="sxs-lookup"><span data-stu-id="276c4-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="276c4-110">Príklad: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="276c4-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="276c4-111">Vyberte používateľa v zozname.</span><span class="sxs-lookup"><span data-stu-id="276c4-111">Select the user from the list.</span></span>

- <span data-ttu-id="276c4-112">Na páse s nástrojmi kliknite na položku **odstrániť povolenia používateľa** .</span><span class="sxs-lookup"><span data-stu-id="276c4-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="276c4-113">Pridajte späť používateľa a znova odošlite pozvánku používateľovi.</span><span class="sxs-lookup"><span data-stu-id="276c4-113">Add back the User and Resend the invite to the user.</span></span>


---
title: Riešenie problému-používateľ sa nenašiel v adresári
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754207"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="c3810-102">Riešenie problému-používateľ sa nenašiel v adresári</span><span class="sxs-lookup"><span data-stu-id="c3810-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="c3810-103">Ak používatelia dostávajú chybové hlásenie "používateľ sa nenašiel" v adresári.</span><span class="sxs-lookup"><span data-stu-id="c3810-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="c3810-104">Skúste to znova, ak je typ problému používateľ nie je v adresári.</span><span class="sxs-lookup"><span data-stu-id="c3810-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="c3810-105">Nasledujúce kroky môžu byť dokončené na vyriešenie problému.</span><span class="sxs-lookup"><span data-stu-id="c3810-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="c3810-106">Uistite sa, že účet, ktorý prijal e-mailovú pozvánku je rovnaký účet, ktorý sa používa na prihlásenie neskôr.</span><span class="sxs-lookup"><span data-stu-id="c3810-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="c3810-107">Uistite sa, že používateľ používa rovnaký účet prijať pozvanie a prihláste sa na lokalitu.</span><span class="sxs-lookup"><span data-stu-id="c3810-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="c3810-108">Ďalšie informácie nájdete v téme [spravovanie aliasov konta</a> Microsoft na spravovanie prihlásenia na Office 365](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="c3810-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="c3810-109">Prejdite na každú lokalitu, v ktorej používateľ dostane chybu.</span><span class="sxs-lookup"><span data-stu-id="c3810-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="c3810-110">Pridať "/_layouts/15/People.aspx/MembershipGroupId = 0" (v úvodzovkách) na koniec adresy URL lokality.</span><span class="sxs-lookup"><span data-stu-id="c3810-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="c3810-111">Príklad: https://_ lt_ "contoso">. SharePoint. com/_layouts/15/People. aspx/membershipGroupId = 0.</span><span class="sxs-lookup"><span data-stu-id="c3810-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="c3810-112">Vyberte používateľa zo zoznamu.</span><span class="sxs-lookup"><span data-stu-id="c3810-112">Select the user from the list.</span></span>

- <span data-ttu-id="c3810-113">Kliknite na položku **odstrániť povolenia používateľa** z pása s nástrojmi.</span><span class="sxs-lookup"><span data-stu-id="c3810-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="c3810-114">Pridajte späť používateľa a odošlite pozvánku používateľovi.</span><span class="sxs-lookup"><span data-stu-id="c3810-114">Add back the User and Resend the invite to the user.</span></span>


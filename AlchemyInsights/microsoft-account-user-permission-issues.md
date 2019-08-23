---
title: Vyriešiť problém - používateľ nenašiel v adresári
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544878"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="92aa9-102">Vyriešiť problém - používateľ nenašiel v adresári</span><span class="sxs-lookup"><span data-stu-id="92aa9-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="92aa9-103">Používateľom sa zobrazuje chybové hlásenie "používateľa sa nenašla" v adresári.</span><span class="sxs-lookup"><span data-stu-id="92aa9-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="92aa9-104">Prosím, skúste znova kde typ problému používateľ nie je v adresári.</span><span class="sxs-lookup"><span data-stu-id="92aa9-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="92aa9-105">Tieto kroky môže byť dokončená na vyriešenie problému.</span><span class="sxs-lookup"><span data-stu-id="92aa9-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="92aa9-106">Zabezpečiť konto, e-mailovú pozvánku prijme rovnaké konto, ktoré používa prihlásiť neskôr.</span><span class="sxs-lookup"><span data-stu-id="92aa9-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="92aa9-107">Uistite sa, že používateľ používa rovnaké konto prijmite pozvanie a prihláste sa do site.</span><span class="sxs-lookup"><span data-stu-id="92aa9-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="92aa9-108">Ďalšie informácie nájdete v téme [Správa aliasov konta Microsoft</a> spravovať Office 365 prihlásenie](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="92aa9-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="92aa9-109">Vyhľadajte každý lokalít, v ktorých používateľ dostáva chyba.</span><span class="sxs-lookup"><span data-stu-id="92aa9-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="92aa9-110">Pridať "/ _layouts/15/people.aspx/membershipgroupid=0" (do úvodzoviek) na koniec URL stránky.</span><span class="sxs-lookup"><span data-stu-id="92aa9-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="92aa9-111">Príklad: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="92aa9-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="92aa9-112">Vyberte používateľa v zozname.</span><span class="sxs-lookup"><span data-stu-id="92aa9-112">Select the user from the list.</span></span>

- <span data-ttu-id="92aa9-113">Kliknite na položku **odstrániť povolenia používateľov** z pása s nástrojmi.</span><span class="sxs-lookup"><span data-stu-id="92aa9-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="92aa9-114">Pridať späť používateľa a odoslať pozvánku používateľovi.</span><span class="sxs-lookup"><span data-stu-id="92aa9-114">Add back the User and Resend the invite to the user.</span></span>


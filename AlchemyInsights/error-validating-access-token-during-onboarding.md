---
title: Počas nastupovania do funkcie Desktop Analytics sa vyskytla chyba s overujúca chyba prístupového tokenu
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813703"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="7d79c-102">Počas za panelovania funkcie Desktop Analytics sa vyskytla chyba overovania prístupového tokenu</span><span class="sxs-lookup"><span data-stu-id="7d79c-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="7d79c-103">Táto chyba sa zvyčajne vyskytuje po uplynutí platnosti tokenu overenia.</span><span class="sxs-lookup"><span data-stu-id="7d79c-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="7d79c-104">Obnovením stránky sa zvyčajne obnoví token.</span><span class="sxs-lookup"><span data-stu-id="7d79c-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="7d79c-105">Tento problém však môže pretrvávať, ak sa v konte používanom na počítačovú analýzu na palube používajú nejaké politiky podmieneného prístupu.</span><span class="sxs-lookup"><span data-stu-id="7d79c-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="7d79c-106">Môžete si pozrieť denníky prihlásenia do služby Azure AD na portáli Azure a zistiť, či sa pre konto používaná pre onboardovanie funkcie Desktop Analytics nejaké zlyhanie prihlásenia.</span><span class="sxs-lookup"><span data-stu-id="7d79c-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="7d79c-107">Ďalšie informácie o podmienenom prístupe nájdete v článku [Plánovanie nasadenia podmieneného prístupu.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="7d79c-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>
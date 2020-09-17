---
title: Pri overovaní chyby tokenu prístupu počas analýzy počítača sa vyskytla chyba.
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783566"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="7e43a-102">Chyba pri overovaní accessového tokenu sa vyskytla chyba počas integrovaného nástroja na analýzu pracovnej plochy</span><span class="sxs-lookup"><span data-stu-id="7e43a-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="7e43a-103">Táto chyba sa zvyčajne sleduje po uplynutí platnosti overovacieho tokenu.</span><span class="sxs-lookup"><span data-stu-id="7e43a-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="7e43a-104">Obnovenie stránky zvyčajne obnoví token.</span><span class="sxs-lookup"><span data-stu-id="7e43a-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="7e43a-105">Tento problém však môže pretrvávať, ak sa uplatňujú politiky podmieneného prístupu použité na konto, ktoré sa používa na analýzu na palube počítača.</span><span class="sxs-lookup"><span data-stu-id="7e43a-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="7e43a-106">Ak chcete zistiť, či existujú nejaké zlyhanie prihlásenia pre konto, ktoré sa používa na zabudovanie počítačovej analýzy, môžete si pozrieť Denníky prihlásenia Azure AD na portáli Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="7e43a-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="7e43a-107">Ďalšie informácie o podmienenom prístupe nájdete v téme [Plánovanie nasadenia podmieneného prístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="7e43a-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>
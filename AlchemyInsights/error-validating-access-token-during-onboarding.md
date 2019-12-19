---
title: Vyskytla sa chyba pri overovaní prístupu token chyba počas Desktop Analytics na stravovanie
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741268"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="ab5b0-102">"Došlo k chybe overenie prístupového tokenu" chyba počas Desktop Analytics registrácia</span><span class="sxs-lookup"><span data-stu-id="ab5b0-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="ab5b0-103">Táto chyba sa zvyčajne pozoruje pri uplynutí tokenu overenia.</span><span class="sxs-lookup"><span data-stu-id="ab5b0-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="ab5b0-104">Zvyčajne obnovuje stránku obnoví token.</span><span class="sxs-lookup"><span data-stu-id="ab5b0-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="ab5b0-105">Tento problém však môže pretrvávať, ak existujú nejaké politiky podmieneného prístupu použité na konto sa používa na palube Desktop Analytics.</span><span class="sxs-lookup"><span data-stu-id="ab5b0-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="ab5b0-106">Môžete skontrolovať Azure AD prihlásiť denníky na portáli Azure zistiť, či existujú nejaké zlyhanie prihlásenia pre konto sa používa pre Desktop Analytics Onboarding.</span><span class="sxs-lookup"><span data-stu-id="ab5b0-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="ab5b0-107">Ďalšie informácie o podmienenom prístupe nájdete [v téme Plánovanie nasadenia podmieneného prístupu](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="ab5b0-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>
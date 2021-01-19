---
title: Problémy s udelením súhlasu správcu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901511"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="de0f1-102">Problémy s udelením súhlasu správcu</span><span class="sxs-lookup"><span data-stu-id="de0f1-102">Admin consent issues</span></span>

1. <span data-ttu-id="de0f1-103">Povoľte [pracovný postup súhlasu správcu](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , aby používatelia mohli požiadať o schválenie správcu priamo z obrazovky súhlasu.</span><span class="sxs-lookup"><span data-stu-id="de0f1-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="de0f1-104">Ak sa počas procesu udelenia súhlasu zobrazili neočakávané chyby, v tomto článku nájdete postup na riešenie problémov: [neočakávaná chyba pri vykonávaní súhlasu s aplikáciou](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="de0f1-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="de0f1-105">Ďalšie informácie o [súhlase správcu na platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), o tom, ako funguje [výzva na udelenie súhlasu](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) , a ako [vyhodnotiť žiadosť o súhlas správcu pre celú nájomníka](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="de0f1-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="de0f1-106">Aplikácie, ktoré sú integrované s platformou Microsoft identity, sledujú autorizačný model, ktorý umožňuje používateľom a správcom kontrolovať spôsob prístupu k údajom.</span><span class="sxs-lookup"><span data-stu-id="de0f1-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="de0f1-107">Implementácia modelu autorizácie bola aktualizovaná na koncovom bode Microsoft Identity Platform a mení sa, ako musí aplikácia pracovať s platformou Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="de0f1-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="de0f1-108">Pozrite si tému [povolenia a súhlas v koncovom bode platformy Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) pre prehľad tohto modelu autorizácie vrátane rozsahov, povolení a súhlasu.</span><span class="sxs-lookup"><span data-stu-id="de0f1-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>
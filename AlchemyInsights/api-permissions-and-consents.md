---
title: Povolenia a súhlas rozhrania API
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974993"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="7ee2a-102">Povolenia a súhlas rozhrania API</span><span class="sxs-lookup"><span data-stu-id="7ee2a-102">API permissions and consent</span></span>

<span data-ttu-id="7ee2a-103">Aplikácie, ktoré sú integrované s platformou Microsoft identity, sledujú autorizačný model, ktorý umožňuje používateľom a správcom kontrolovať spôsob prístupu k údajom.</span><span class="sxs-lookup"><span data-stu-id="7ee2a-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="7ee2a-104">Implementácia modelu autorizácie bola aktualizovaná na koncovom bode platformy Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="7ee2a-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="7ee2a-105">Zmení sa, ako aplikácia musí pracovať s platformou Microsoft Identity.</span><span class="sxs-lookup"><span data-stu-id="7ee2a-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="7ee2a-106">[Povolenia a súhlas v koncovom bode platformy Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) sa vzťahujú na základné pojmy tohto modelu autorizácie vrátane rozsahov, povolení a súhlasu.</span><span class="sxs-lookup"><span data-stu-id="7ee2a-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="7ee2a-107">[Rámec súhlasu služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) zjednodušuje tvorbu webových a natívnych klientskych aplikácií viacerých nájomníkov.</span><span class="sxs-lookup"><span data-stu-id="7ee2a-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="7ee2a-108">Tieto aplikácie povoľujú prihlásenie pomocou používateľských kont z nájomníka služby Azure AD, ktorý sa líši od toho, v ktorom je aplikácia zaregistrovaná.</span><span class="sxs-lookup"><span data-stu-id="7ee2a-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="7ee2a-109">Okrem vlastných webových rozhraní API môžu tiež potrebovať prístup k webovým rozhraniam API, ako je napríklad rozhranie Microsoft Graph API (na prístup k službe Azure AD, Intune a službám v Microsoft 365) a v iných rozhraniach API služieb spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="7ee2a-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>


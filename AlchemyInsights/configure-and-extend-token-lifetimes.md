---
title: Konfigurovanie a predĺženie životnosti tokenov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917011"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="35bb6-102">Konfigurovanie a predĺženie životnosti tokenov</span><span class="sxs-lookup"><span data-stu-id="35bb6-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="35bb6-103">Môžete zadať životnosť tokenu Accessu, SAML alebo ID vydaného spoločnosťou Microsoft Identity Platform.</span><span class="sxs-lookup"><span data-stu-id="35bb6-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="35bb6-104">Môžete nastaviť životnosť tokenov pre všetky aplikácie vo vašej organizácii, pre aplikáciu viacerých nájomníkov (multi-Organization) alebo pre konkrétnu službu v organizácii.</span><span class="sxs-lookup"><span data-stu-id="35bb6-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="35bb6-105">Ďalšie informácie nájdete v téme [konfigurovateľné tokeny životnosti](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="35bb6-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="35bb6-106">Príklady si môžete prečítať v [téme ako nakonfigurovať životnosť tokenov](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span><span class="sxs-lookup"><span data-stu-id="35bb6-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="35bb6-107">Ak chcete zistiť, ako nakonfigurovať životnosť a kompatibilitu tokenu v službe Azure Active Directory B2C (Azure AD B2C), pozrite si tému [Konfigurácia tokenov v službe Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span><span class="sxs-lookup"><span data-stu-id="35bb6-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="35bb6-108">Článok [Konfigurácia správania relácie v službe Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) popisuje metódy jediného prihlásenia (SSO), ktoré sa používajú v službe Azure AD B2C, a pomáha vám pri konfigurácii politiky použiť NAJVHODNEJŠÍ spôsob SSO.</span><span class="sxs-lookup"><span data-stu-id="35bb6-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="35bb6-109">**Ako dlho trvajú tokeny? Ako dlho platia?**</span><span class="sxs-lookup"><span data-stu-id="35bb6-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="35bb6-110">Životnosť tokenov je 1 hodina a životnosť relácie je 24 hodín.</span><span class="sxs-lookup"><span data-stu-id="35bb6-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="35bb6-111">To znamená, že ak sa nevykonajú žiadne žiadosti v priebehu 24 hodín, pred vyžiadaním nového tokenu sa budete musieť znova prihlásiť.</span><span class="sxs-lookup"><span data-stu-id="35bb6-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="35bb6-112">Po 30. mája 2020 bude mať žiadny nový nájomník možnosť použiť konfigurovateľné tokeny Lifetime Policy na konfiguráciu relácií a obnovenia tokenov.</span><span class="sxs-lookup"><span data-stu-id="35bb6-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="35bb6-113">Nezhoda sa stane v priebehu niekoľkých mesiacov po tom, čo znamená, že zastavíme rešpektovanie existujúcich relácií a obnovenia tokenov polície.</span><span class="sxs-lookup"><span data-stu-id="35bb6-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="35bb6-114">Životnosť tokenov prístupu môžete nakonfigurovať aj po uplynutí platnosti.</span><span class="sxs-lookup"><span data-stu-id="35bb6-114">You can still configure access token lifetimes after the deprecation.</span></span>







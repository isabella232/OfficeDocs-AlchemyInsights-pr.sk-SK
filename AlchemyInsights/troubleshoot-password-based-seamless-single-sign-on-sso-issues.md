---
title: Riešenie problémov s bezproblémovým jediným prihlásením (SSO) založeného na hesle
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714886"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="fcea0-102">Riešenie problémov s bezproblémovým jediným prihlásením (SSO) založeného na hesle</span><span class="sxs-lookup"><span data-stu-id="fcea0-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="fcea0-103">Ak sa chcete dozvedieť základy SSO na základe hesla, pozrite si tému [overovanie na základe hesla so službou Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span><span class="sxs-lookup"><span data-stu-id="fcea0-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="fcea0-104">**Konfigurovanie SSO na základe hesla**</span><span class="sxs-lookup"><span data-stu-id="fcea0-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="fcea0-105">[Konfigurácia jediného prihlásenia založeného na hesle – v](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) tomto článku nájdete podrobnejšie informácie o možnosti SSO na základe hesla.</span><span class="sxs-lookup"><span data-stu-id="fcea0-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="fcea0-106">Ak pridávaná aplikácia vyžaduje vlastnú konfiguráciu a potrebujete použiť SSO na základe hesla, tento článok je určený vám.</span><span class="sxs-lookup"><span data-stu-id="fcea0-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="fcea0-107">[Konfigurácia jediného prihlásenia založeného na hesle pre aplikácie v službe Prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – server proxy aplikácie podporuje viaceré režimy jediného prihlásenia.</span><span class="sxs-lookup"><span data-stu-id="fcea0-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="fcea0-108">Prihlásenie na základe hesla je určené pre aplikácie, ktoré používajú kombináciu používateľského mena a hesla na overenie.</span><span class="sxs-lookup"><span data-stu-id="fcea0-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="fcea0-109">Pri konfigurácii prihlásenia na základe hesla pre svoju aplikáciu sa používatelia musia prihlásiť do lokálnej aplikácie raz.</span><span class="sxs-lookup"><span data-stu-id="fcea0-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="fcea0-110">Za to, Azure Active Directory ukladá prihlasovacie údaje a automaticky ju poskytne aplikácii, keď používatelia prístup na diaľku.</span><span class="sxs-lookup"><span data-stu-id="fcea0-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="fcea0-111">Aplikáciu by ste už mali publikovať a otestovať pomocou servera proxy aplikácie.</span><span class="sxs-lookup"><span data-stu-id="fcea0-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="fcea0-112">Ak nie, postupujte podľa krokov v téme [publikovanie aplikácií pomocou servera proxy aplikácie Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) a potom pokračujte v konfigurácii SSO na základe hesla pre aplikácie v službe Prem.</span><span class="sxs-lookup"><span data-stu-id="fcea0-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="fcea0-113">Riešenie problémov s SSO na základe hesla nájdete [v téme Riešenie problémov s jediným prihlásením založeným na hesle v službe Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="fcea0-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>

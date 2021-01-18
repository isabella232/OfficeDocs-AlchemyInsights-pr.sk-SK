---
title: Konfigurácia servera proxy aplikácie
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885527"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="3ad0d-102">Konfigurácia servera proxy aplikácie</span><span class="sxs-lookup"><span data-stu-id="3ad0d-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="3ad0d-103">Informácie o konfigurácii aplikácie proxy aplikácie v službe Azure AD na vystavenie lokálnych aplikácií do cloudu nájdete v téme Konfigurácia aplikácie [proxy aplikácie](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="3ad0d-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="3ad0d-104">Jediné prihlásenie (SSO) umožňuje používateľom prístup k aplikácii bez overenia viackrát.</span><span class="sxs-lookup"><span data-stu-id="3ad0d-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="3ad0d-105">Umožňuje vykonávať jednoduché overovanie v cloude v porovnaní so službou Azure Active Directory a umožňuje službe alebo spojnici zosobniť používateľa, aby dokončil akékoľvek ďalšie problémy s overovaním z aplikácie.</span><span class="sxs-lookup"><span data-stu-id="3ad0d-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="3ad0d-106">Ďalšie informácie nájdete v téme [Konfigurácia jediného prihlásenia do aplikácie proxy aplikácie](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="3ad0d-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="3ad0d-107">[Tento článok](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) sa používa na riešenie bežných problémov, ktorým ľudia čelia pri vytváraní novej aplikácie proxy aplikácie.</span><span class="sxs-lookup"><span data-stu-id="3ad0d-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="3ad0d-108">Ak máte problém s nastavením záložnej autentifikácie v aplikácii, budete musieť riešiť problémy s [obmedzením delegovania delegovania Kerberos pre aplikačný Server](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) alebo sledovať pokyny týkajúce sa [konfigurácie aplikácie s PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) .</span><span class="sxs-lookup"><span data-stu-id="3ad0d-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>

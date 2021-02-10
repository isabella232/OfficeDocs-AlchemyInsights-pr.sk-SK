---
title: Nasadenie služby AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177717"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="640f9-102">Nasadenie služby AD FS</span><span class="sxs-lookup"><span data-stu-id="640f9-102">Deploy AD FS</span></span>

<span data-ttu-id="640f9-103">Nasadenie služby Active Directory Federation Services (ADFS) (AD FS) používa lokálnu infraštruktúru na overenie používateľov služieb Office 365.</span><span class="sxs-lookup"><span data-stu-id="640f9-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="640f9-104">S externým prihlásením môžete povoliť používateľom prihlásiť sa do služieb a softvéru balíka Office 365 ako služby (SAAS), ktoré sú integrované so službou Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="640f9-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="640f9-105">Externý podpis overí používateľov v lokálnej službe Active Directory prostredníctvom služby AD FS.</span><span class="sxs-lookup"><span data-stu-id="640f9-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="640f9-106">Aj keď sa v podnikovej sieti používatelia nebudú musieť znova zadať svoje heslá.</span><span class="sxs-lookup"><span data-stu-id="640f9-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="640f9-107">[Poradca pre nasadenie AD FS](https://go.microsoft.com/fwlink/?linkid=2071178) vám poskytuje podrobné pokyny na nasadenie lokálnej infraštruktúry AD FS, ktorá overuje používateľov služieb Microsoft 365 a služieb Office 365.</span><span class="sxs-lookup"><span data-stu-id="640f9-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="640f9-108">V tejto príručke môže vaša organizácia skontrolovať súčasti a požiadavky služby AD FS, získať a nainštalovať Certifikáty SSL, ktoré sú potrebné na nasadenie, a nainštalovať požadovanú proxy server webovej aplikácie.</span><span class="sxs-lookup"><span data-stu-id="640f9-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>

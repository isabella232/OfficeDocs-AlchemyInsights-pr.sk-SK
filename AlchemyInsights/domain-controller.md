---
title: Radič domény
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901313"
---
# <a name="domain-controller"></a><span data-ttu-id="bc93e-102">Radič domény</span><span class="sxs-lookup"><span data-stu-id="bc93e-102">Domain controller</span></span>

<span data-ttu-id="bc93e-103">**Nie je možné povoliť AAD-DS alebo nasadenie zlyháva**</span><span class="sxs-lookup"><span data-stu-id="bc93e-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="bc93e-104">Ak chcete vyriešiť problém služby Azure AD Domain (AAD-DS), ktorý nie je povolený alebo nie je možné nasadiť, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="bc93e-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="bc93e-105">Ak používate už existujúcu virtuálnu sieť, pozrite si NSG pravidlá, ktoré blokujú porty potrebné na synchronizáciu v rámci AAD-DS na portáli https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="bc93e-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="bc93e-106">Skontrolujte, či sa v tejto príručke na riešenie problémov, ktorá je k dispozícii, zobrazí chybové hlásenie  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="bc93e-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="bc93e-107">Skúste nasadiť služby Azure AD Domain Services v novej virtuálnej sieti.</span><span class="sxs-lookup"><span data-stu-id="bc93e-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="bc93e-108">Postupujte podľa pokynov Začíname s nasadením AAD-DS, ktoré je k dispozícii na lokalite [tutorial na vytvorenie služieb Azure AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="bc93e-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="bc93e-109">Ak máte problémy s nasadením služieb Azure AD Domain, prečítajte si tému [Riešenie problémov s doménou služby Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) na vyriešenie bežných chýb, ktoré vám pomôžu pri opätovnom práci.</span><span class="sxs-lookup"><span data-stu-id="bc93e-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="bc93e-110">**AAD-DS sa nedá vypnúť**</span><span class="sxs-lookup"><span data-stu-id="bc93e-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="bc93e-111">AAD-DS nie je možné pozastaviť.</span><span class="sxs-lookup"><span data-stu-id="bc93e-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="bc93e-112">Ak chcete prestať používať spravovanú doménu, musí byť odstránená.</span><span class="sxs-lookup"><span data-stu-id="bc93e-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="bc93e-113">Ak sa vyskytnú problémy, riešenie bežných chybových hlásení a súvisiace kroky na riešenie problémov, ktoré vám pomôžu znova začať pracovať, pozrite si tému [Riešenie problémov s doménovou službou Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="bc93e-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>

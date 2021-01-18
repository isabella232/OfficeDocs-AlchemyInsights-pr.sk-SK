---
title: Konfigurácia služby Domain
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885688"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="eea28-102">Nie je možné povoliť AAD-DS alebo nasadenie zlyháva</span><span class="sxs-lookup"><span data-stu-id="eea28-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="eea28-103">Ak chcete vyriešiť problém služby Azure AD Domain (AAD-DS), ktorý nie je povolený alebo nie je možné nasadiť, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="eea28-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="eea28-104">Ak používate už existujúcu virtuálnu sieť, pozrite si NSG pravidlá, ktoré blokujú porty potrebné na synchronizáciu v rámci AAD-DS na portáli https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="eea28-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="eea28-105">Skontrolujte, či sa v tejto príručke na riešenie problémov, ktorá je k dispozícii, zobrazí chybové hlásenie  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="eea28-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="eea28-106">Skúste nasadiť služby Azure AD Domain Services v novej virtuálnej sieti.</span><span class="sxs-lookup"><span data-stu-id="eea28-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="eea28-107">Postupujte podľa pokynov Začíname s nasadením AAD – DS: [Vytvorenie a konfigurácia služieb domény AAD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="eea28-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="eea28-108">Ak máte problémy s nasadením služieb Azure AD Domain, prečítajte si tému [Riešenie problémov s doménou služby Azure AD](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) na vyriešenie bežných chýb, ktoré vám pomôžu pri opätovnom práci.</span><span class="sxs-lookup"><span data-stu-id="eea28-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="eea28-109">**AAD-DS sa nedá vypnúť**</span><span class="sxs-lookup"><span data-stu-id="eea28-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="eea28-110">AAD-DS nie je možné pozastaviť.</span><span class="sxs-lookup"><span data-stu-id="eea28-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="eea28-111">Ak chcete prestať používať spravovanú doménu, musí byť odstránená.</span><span class="sxs-lookup"><span data-stu-id="eea28-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="eea28-112">Ak chcete odstrániť spravovanú doménu, pozrite si tému [Odstránenie domény služby AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="eea28-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>




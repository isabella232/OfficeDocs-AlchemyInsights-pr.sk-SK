---
title: Nastavenie DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: d23a816d4eef065f800eaee60829d57dc1e7177f
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/21/2020
ms.locfileid: "43645687"
---
# <a name="setup-dkim"></a><span data-ttu-id="9c609-102">Nastavenie DKIM</span><span class="sxs-lookup"><span data-stu-id="9c609-102">Setup DKIM</span></span>

<span data-ttu-id="9c609-103">Kompletné pokyny pre konfiguráciu DKIM pre vlastné domény v Microsoft 365 sú [tu](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="9c609-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="9c609-104">Pre **každú** vlastnú doménu, musíte vytvoriť **dva** dkim CNAME záznamy v doméne DNS hostingové služby (typicky, Registrátor domén).</span><span class="sxs-lookup"><span data-stu-id="9c609-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="9c609-105">Napríklad contoso.com a fourthcoffee.com vyžadujú štyri záznamy DKIM CNAME: dve pre contoso.com a dve pre fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="9c609-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="9c609-106">Záznamy CNAME DKIM pre **každú** vlastnú doménu používajú nasledujúce formáty:</span><span class="sxs-lookup"><span data-stu-id="9c609-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="9c609-107">**Názov hostiteľa**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9c609-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9c609-108">**Body na adresu alebo hodnotu**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9c609-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9c609-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9c609-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="9c609-110">**Názov hostiteľa**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="9c609-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="9c609-111">**Body na adresu alebo hodnotu**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="9c609-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="9c609-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="9c609-112">**TTL**: 3600</span></span>

   <span data-ttu-id="9c609-113">\<DomainGUID\> je text naľavo `.mail.protection.outlook.com` v prispôsobenom zázname MX pre vlastnú doménu (napríklad `contoso-com` pre doménu contoso.com).</span><span class="sxs-lookup"><span data-stu-id="9c609-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="9c609-114">\<InitialDomain\> je doména, ktorú ste použili pri prihlásení do spoločnosti Microsoft 365 (napríklad contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="9c609-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="9c609-115">Po vytvorení záznamov CNAME pre vlastné domény postupujte podľa nasledujúcich pokynov:</span><span class="sxs-lookup"><span data-stu-id="9c609-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="9c609-116">A.</span><span class="sxs-lookup"><span data-stu-id="9c609-116">a.</span></span> <span data-ttu-id="9c609-117">[Prihláste sa do Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) so svojím pracovným alebo školským kontom.</span><span class="sxs-lookup"><span data-stu-id="9c609-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="9c609-118">B.</span><span class="sxs-lookup"><span data-stu-id="9c609-118">b.</span></span> <span data-ttu-id="9c609-119">V ľavom hornom rohu vyberte ikonu spúšťača aplikácií a vyberte možnosť **správca**.</span><span class="sxs-lookup"><span data-stu-id="9c609-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="9c609-120">C.</span><span class="sxs-lookup"><span data-stu-id="9c609-120">c.</span></span> <span data-ttu-id="9c609-121">V ľavom dolnom navigáciu, rozbaľte **admin** a vyberte **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="9c609-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="9c609-122">D.</span><span class="sxs-lookup"><span data-stu-id="9c609-122">d.</span></span> <span data-ttu-id="9c609-123">Prejdite na **ochranu** > **dkim**.</span><span class="sxs-lookup"><span data-stu-id="9c609-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="9c609-124">E.</span><span class="sxs-lookup"><span data-stu-id="9c609-124">e.</span></span> <span data-ttu-id="9c609-125">Vyberte doménu a potom vyberte **Povoliť** pre **podpísať správy pre túto doménu s dkim podpisy**.</span><span class="sxs-lookup"><span data-stu-id="9c609-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="9c609-126">Zopakujte tento krok pre každú vlastnú doménu.</span><span class="sxs-lookup"><span data-stu-id="9c609-126">Repeat this step for each custom domain.</span></span>

---
title: Nastavenie DKIM v balíku Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: dd908db6a4bc1739b3c1cff059387034d67e093d
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666279"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="e59ba-102">Nastavenie DKIM v balíku Office 365</span><span class="sxs-lookup"><span data-stu-id="e59ba-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="e59ba-103">Úplné pokyny na konfigurovanie DKIM vlastnej domény v Office 365 sú [tu](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="e59ba-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="e59ba-104">Pre **každú** vlastnú doménu, musíte vytvoriť **dva** záznamy DKIM CNAME hostiteľskej služby servera DNS vašej domény (zvyčajne Registrátor domén).</span><span class="sxs-lookup"><span data-stu-id="e59ba-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="e59ba-105">Napríklad contoso.com a fourthcoffee.com vyžadujú štyri DKIM CNAME záznamov: dva pre contoso.com a dva pre fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="e59ba-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="e59ba-106">DKIM CNAME záznamov pre **každú** vlastnú doménu, použite nasledujúce formáty:</span><span class="sxs-lookup"><span data-stu-id="e59ba-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="e59ba-107">**Názov hostiteľa**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e59ba-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e59ba-108">**Body na adresu alebo hodnotu**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e59ba-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e59ba-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="e59ba-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="e59ba-110">**Názov hostiteľa**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="e59ba-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="e59ba-111">**Body na adresu alebo hodnotu**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="e59ba-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="e59ba-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="e59ba-112">**TTL**: 3600</span></span>

   <span data-ttu-id="e59ba-113">\<DomainGUID\> je text naľavo od `.mail.protection.outlook.com` v prispôsobených záznam MX pre domény (napríklad `contoso-com` domény contoso.com).</span><span class="sxs-lookup"><span data-stu-id="e59ba-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="e59ba-114">\<InitialDomain\> je doména, ktorú ste použili pri registrácii do služby Office 365 (doménu napríklad contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="e59ba-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="e59ba-115">Po vytvorení záznamy CNAME pre svoje vlastné domény, použite nasledujúce pokyny:</span><span class="sxs-lookup"><span data-stu-id="e59ba-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="e59ba-116">a.</span><span class="sxs-lookup"><span data-stu-id="e59ba-116">a.</span></span> <span data-ttu-id="e59ba-117">[Prihlásenie do služby Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocou konta práca alebo škola.</span><span class="sxs-lookup"><span data-stu-id="e59ba-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="e59ba-118">b.</span><span class="sxs-lookup"><span data-stu-id="e59ba-118">b.</span></span> <span data-ttu-id="e59ba-119">Vyberte ikonu launcher aplikácie v ľavom hornom a **Admin**.</span><span class="sxs-lookup"><span data-stu-id="e59ba-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="e59ba-120">c.</span><span class="sxs-lookup"><span data-stu-id="e59ba-120">c.</span></span> <span data-ttu-id="e59ba-121">V ľavom dolnom navigácia, rozbaľte **Admin** a vyberte **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="e59ba-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="e59ba-122">d.</span><span class="sxs-lookup"><span data-stu-id="e59ba-122">d.</span></span> <span data-ttu-id="e59ba-123">Prejdite na **ochranu** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="e59ba-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="e59ba-124">e.</span><span class="sxs-lookup"><span data-stu-id="e59ba-124">e.</span></span> <span data-ttu-id="e59ba-125">Vyberte doménu, a potom vyberte **Povoliť** pre **znak správy pre túto doménu s podpismi DKIM**.</span><span class="sxs-lookup"><span data-stu-id="e59ba-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="e59ba-126">Zopakujte tento krok pre každú vlastnú doménu.</span><span class="sxs-lookup"><span data-stu-id="e59ba-126">Repeat this step for each custom domain.</span></span>

---
title: Nastavenie DKIM v balíku Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765407"
---
# <a name="setup-dkim-in-office-365"></a><span data-ttu-id="4563f-102">Nastavenie DKIM v balíku Office 365</span><span class="sxs-lookup"><span data-stu-id="4563f-102">Setup DKIM in Office 365</span></span>

<span data-ttu-id="4563f-103">Úplné pokyny na konfigurovanie DKIM vlastnej domény v Office 365 sú [tu](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4563f-103">The complete instructions for configuring DKIM for custom domains in Office 365 are [here](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

1. <span data-ttu-id="4563f-104">Pre **každú** vlastnú doménu, musíte vytvoriť **dva** záznamy DKIM CNAME hostiteľskej služby servera DNS vašej domény (zvyčajne Registrátor domén).</span><span class="sxs-lookup"><span data-stu-id="4563f-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="4563f-105">Napríklad contoso.com a fourthcoffee.com vyžadujú štyri DKIM CNAME záznamov: dva pre contoso.com a dva pre fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="4563f-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="4563f-106">DKIM CNAME záznamov pre **každú** vlastnú doménu, použite nasledujúce formáty:</span><span class="sxs-lookup"><span data-stu-id="4563f-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="4563f-107">**Názov hostiteľa**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4563f-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4563f-108">**Body na adresu alebo hodnotu**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4563f-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4563f-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4563f-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="4563f-110">**Názov hostiteľa**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4563f-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4563f-111">**Body na adresu alebo hodnotu**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4563f-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4563f-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4563f-112">**TTL**: 3600</span></span>

   <span data-ttu-id="4563f-113">\<DomainGUID\> je text naľavo od `.mail.protection.outlook.com` v prispôsobených záznam MX pre domény (napríklad `contoso-com` domény contoso.com).</span><span class="sxs-lookup"><span data-stu-id="4563f-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="4563f-114">\<InitialDomain\> je doména, ktorú ste použili pri registrácii do služby Office 365 (doménu napríklad contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="4563f-114">\<InitialDomain\> is the domain you used when you signed up for Office 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="4563f-115">Po vytvorení záznamy CNAME pre svoje vlastné domény, použite nasledujúce pokyny:</span><span class="sxs-lookup"><span data-stu-id="4563f-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="4563f-116">a.</span><span class="sxs-lookup"><span data-stu-id="4563f-116">a.</span></span> <span data-ttu-id="4563f-117">[Prihlásenie do služby Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocou konta práca alebo škola.</span><span class="sxs-lookup"><span data-stu-id="4563f-117">[Sign in to Office 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="4563f-118">b.</span><span class="sxs-lookup"><span data-stu-id="4563f-118">b.</span></span> <span data-ttu-id="4563f-119">Vyberte ikonu launcher aplikácie v ľavom hornom a **Admin**.</span><span class="sxs-lookup"><span data-stu-id="4563f-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="4563f-120">c.</span><span class="sxs-lookup"><span data-stu-id="4563f-120">c.</span></span> <span data-ttu-id="4563f-121">V ľavom dolnom navigácia, rozbaľte **Admin** a vyberte **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4563f-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="4563f-122">d.</span><span class="sxs-lookup"><span data-stu-id="4563f-122">d.</span></span> <span data-ttu-id="4563f-123">Prejdite na **ochranu** > **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="4563f-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="4563f-124">e.</span><span class="sxs-lookup"><span data-stu-id="4563f-124">e.</span></span> <span data-ttu-id="4563f-125">Vyberte doménu, a potom vyberte **Povoliť** pre **znak správy pre túto doménu s podpismi DKIM**.</span><span class="sxs-lookup"><span data-stu-id="4563f-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="4563f-126">Zopakujte tento krok pre každú vlastnú doménu.</span><span class="sxs-lookup"><span data-stu-id="4563f-126">Repeat this step for each custom domain.</span></span>

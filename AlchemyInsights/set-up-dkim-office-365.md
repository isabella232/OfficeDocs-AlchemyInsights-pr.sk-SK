---
title: Nastavenie DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808722"
---
# <a name="setup-dkim"></a><span data-ttu-id="96208-102">Nastavenie DKIM</span><span class="sxs-lookup"><span data-stu-id="96208-102">Setup DKIM</span></span>

<span data-ttu-id="96208-103">Všetky pokyny na konfiguráciu DKIM pre vlastné domény v Microsoft 365 sú [tu](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="96208-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="96208-104">Pre **každú** vlastnú doménu je potrebné vytvoriť **dva** CNAME záznamy CNAME na hostiteľskej službe DNS vašej domény (zvyčajne registrátora domén).</span><span class="sxs-lookup"><span data-stu-id="96208-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="96208-105">Napríklad contoso.com a fourthcoffee.com vyžadujú štyri CNAME záznamy CNAME: dva pre contoso.com a dve pre fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="96208-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="96208-106">CNAME CNAME záznamy pre **každú** vlastnú doménu používajú tieto formáty:</span><span class="sxs-lookup"><span data-stu-id="96208-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="96208-107">**Názov hostiteľa**: `selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="96208-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="96208-108">**Odkazuje na adresu alebo hodnotu**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="96208-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="96208-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="96208-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="96208-110">**Názov hostiteľa**: `selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="96208-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="96208-111">**Odkazuje na adresu alebo hodnotu**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="96208-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="96208-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="96208-112">**TTL**: 3600</span></span>

   <span data-ttu-id="96208-113">\<DomainGUID\> je text naľavo od `.mail.protection.outlook.com` prispôsobeného MX záznamu pre vlastnú doménu (napríklad `contoso-com` pre doménu contoso.com).</span><span class="sxs-lookup"><span data-stu-id="96208-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="96208-114">\<InitialDomain\> je doména, ktorú ste použili, keď ste sa zaregistrovali v službe Microsoft 365 (napríklad contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="96208-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="96208-115">Po vytvorení CNAME záznamov pre svoje vlastné domény postupujte podľa nasledujúcich pokynov:</span><span class="sxs-lookup"><span data-stu-id="96208-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="96208-116">a.</span><span class="sxs-lookup"><span data-stu-id="96208-116">a.</span></span> <span data-ttu-id="96208-117">[Prihláste sa do služby Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocou svojho pracovného alebo školského konta.</span><span class="sxs-lookup"><span data-stu-id="96208-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="96208-118">b.</span><span class="sxs-lookup"><span data-stu-id="96208-118">b.</span></span> <span data-ttu-id="96208-119">V ľavom hornom rohu vyberte ikonu spúšťača aplikácií a vyberte položku **správca**.</span><span class="sxs-lookup"><span data-stu-id="96208-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="96208-120">c.</span><span class="sxs-lookup"><span data-stu-id="96208-120">c.</span></span> <span data-ttu-id="96208-121">V navigácii v ľavom dolnom rohu rozbaľte položku **správca** a vyberte položku **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="96208-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="96208-122">d.</span><span class="sxs-lookup"><span data-stu-id="96208-122">d.</span></span> <span data-ttu-id="96208-123">Prejdite na **ochranu**  >  **dkim**.</span><span class="sxs-lookup"><span data-stu-id="96208-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="96208-124">e.</span><span class="sxs-lookup"><span data-stu-id="96208-124">e.</span></span> <span data-ttu-id="96208-125">Vyberte doménu a potom vyberte položku **Povoliť** pre **podpísanie správ pre túto doménu pomocou podpisov dkim**.</span><span class="sxs-lookup"><span data-stu-id="96208-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="96208-126">Zopakujte tento krok pre každú vlastnú doménu.</span><span class="sxs-lookup"><span data-stu-id="96208-126">Repeat this step for each custom domain.</span></span>

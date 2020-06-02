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
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509399"
---
# <a name="setup-dkim"></a><span data-ttu-id="4347d-102">Nastavenie DKIM</span><span class="sxs-lookup"><span data-stu-id="4347d-102">Setup DKIM</span></span>

<span data-ttu-id="4347d-103">Kompletné pokyny pre konfiguráciu DKIM pre vlastné domény v Microsoft 365 sú [tu](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="4347d-103">The complete instructions for configuring DKIM for custom domains in Microsoft 365 are [here](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

1. <span data-ttu-id="4347d-104">Pre **každú vlastnú** doménu je potrebné vytvoriť **dva** záznamy DKIM CNAME v hostiteľskej službe DNS vašej domény (zvyčajne registrátordomény).</span><span class="sxs-lookup"><span data-stu-id="4347d-104">For **each** custom domain, you need to create **two** DKIM CNAME records at your domain's DNS hosting service (typically, the domain registrar).</span></span> <span data-ttu-id="4347d-105">Napríklad contoso.com a fourthcoffee.com vyžadujú štyri záznamy DKIM CNAME: dva pre contoso.com a dva pre fourthcoffee.com.</span><span class="sxs-lookup"><span data-stu-id="4347d-105">For example, contoso.com and fourthcoffee.com require four DKIM CNAME records: two for contoso.com and two for fourthcoffee.com.</span></span>

   <span data-ttu-id="4347d-106">Záznamy DKIM CNAME pre **každú** vlastnú doménu používajú nasledujúce formáty:</span><span class="sxs-lookup"><span data-stu-id="4347d-106">The DKIM CNAME records for **each** custom domain use the following formats:</span></span>

   - <span data-ttu-id="4347d-107">**Názov hostiteľa**:`selector1._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4347d-107">**Host name**: `selector1._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4347d-108">**Počet bodov na adresu alebo hodnotu:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4347d-108">**Points to address or value**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4347d-109">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4347d-109">**TTL**: 3600</span></span>

   - <span data-ttu-id="4347d-110">**Názov hostiteľa**:`selector2._domainkey.<CustomDomain>`</span><span class="sxs-lookup"><span data-stu-id="4347d-110">**Host name**: `selector2._domainkey.<CustomDomain>`</span></span>

     <span data-ttu-id="4347d-111">**Počet bodov na adresu alebo hodnotu:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`</span><span class="sxs-lookup"><span data-stu-id="4347d-111">**Points to address or value**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`</span></span>

     <span data-ttu-id="4347d-112">**TTL**: 3600</span><span class="sxs-lookup"><span data-stu-id="4347d-112">**TTL**: 3600</span></span>

   <span data-ttu-id="4347d-113">\<DomainGUID\>je text naľavo `.mail.protection.outlook.com` od prispôsobeného záznamu MX pre vlastnú doménu (napríklad `contoso-com` pre contoso.com domény).</span><span class="sxs-lookup"><span data-stu-id="4347d-113">\<DomainGUID\> is the text to the left of `.mail.protection.outlook.com` in the customized MX record for the custom domain (for example, `contoso-com` for the domain contoso.com).</span></span> <span data-ttu-id="4347d-114">\<InitialDomain\>je doména, ktorú ste použili pri registrácii v programe Microsoft 365 (napríklad contoso.onmicrosoft.com).</span><span class="sxs-lookup"><span data-stu-id="4347d-114">\<InitialDomain\> is the domain you used when you signed up for Microsoft 365 (for example, contoso.onmicrosoft.com).</span></span>

2. <span data-ttu-id="4347d-115">Po vytvorení cname záznamov pre vlastné domény, postupujte podľa nasledujúcich pokynov:</span><span class="sxs-lookup"><span data-stu-id="4347d-115">After you've created the CNAME records for your custom domains, complete the following instructions:</span></span>

   <span data-ttu-id="4347d-116">a.</span><span class="sxs-lookup"><span data-stu-id="4347d-116">a.</span></span> <span data-ttu-id="4347d-117">[prihláste sa do služby Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) pomocou pracovného alebo školského konta.</span><span class="sxs-lookup"><span data-stu-id="4347d-117">[sign in to Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) with your work or school account.</span></span>

   <span data-ttu-id="4347d-118">b.</span><span class="sxs-lookup"><span data-stu-id="4347d-118">b.</span></span> <span data-ttu-id="4347d-119">V ľavom hornom rohu vyberte ikonu spúšťača aplikácií a vyberte **položku Správca**.</span><span class="sxs-lookup"><span data-stu-id="4347d-119">Select the app launcher icon in the upper-left and choose **Admin**.</span></span>

   <span data-ttu-id="4347d-120">c.</span><span class="sxs-lookup"><span data-stu-id="4347d-120">c.</span></span> <span data-ttu-id="4347d-121">V ľavom dolnom paneli rozbaľte položku **Správca** a vyberte položku **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="4347d-121">In the lower-left navigation, expand **Admin** and choose **Exchange**.</span></span>

   <span data-ttu-id="4347d-122">D.</span><span class="sxs-lookup"><span data-stu-id="4347d-122">d.</span></span> <span data-ttu-id="4347d-123">Prejsť na **Ochrana**  >  **DKIM**.</span><span class="sxs-lookup"><span data-stu-id="4347d-123">Go to **Protection** > **DKIM**.</span></span>

   <span data-ttu-id="4347d-124">E.</span><span class="sxs-lookup"><span data-stu-id="4347d-124">e.</span></span> <span data-ttu-id="4347d-125">Vyberte doménu a potom vyberte **položku Povoliť** **pre podpisy pre túto doménu s podpismi DKIM**.</span><span class="sxs-lookup"><span data-stu-id="4347d-125">Select the domain and then choose **Enable** for **Sign messages for this domain with DKIM signatures**.</span></span> <span data-ttu-id="4347d-126">Zopakujte tento krok pre každú vlastnú doménu.</span><span class="sxs-lookup"><span data-stu-id="4347d-126">Repeat this step for each custom domain.</span></span>

---
title: DLP nefunguje podľa očakávania
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530309"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="74c24-102">DLP nefunguje podľa očakávania</span><span class="sxs-lookup"><span data-stu-id="74c24-102">DLP not working as expected</span></span>

<span data-ttu-id="74c24-103">Máte problémy s **Data Loss Prevention (DLP)** v Office 365 nefunguje ako sa očakávalo?</span><span class="sxs-lookup"><span data-stu-id="74c24-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="74c24-104">Ak áno, uistite sa, že **DLP politiky** je nastavený správne, a že údaje obsahujú aké **DLP politiky** hľadá, keď je hodnotený.</span><span class="sxs-lookup"><span data-stu-id="74c24-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="74c24-105">**Nastavenie DLP**</span><span class="sxs-lookup"><span data-stu-id="74c24-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="74c24-106">DLP politiky umožňuje identifikovať a chrániť citlivé informácie v organizácii.</span><span class="sxs-lookup"><span data-stu-id="74c24-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="74c24-107">Nastavenie politiky DLP, používať informácie [tu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="74c24-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="74c24-108">**Pozrite sa aké DLP politiky**</span><span class="sxs-lookup"><span data-stu-id="74c24-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="74c24-109">Pri použití **vstavaný citlivé informácie typy** v Office 365 zabezpečenia a zhody centrum, DLP politiky hľadať konkrétne vzory a prvky pri odhaľovaní týchto citlivých druhov.</span><span class="sxs-lookup"><span data-stu-id="74c24-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="74c24-110">**Typov vstavaných citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="74c24-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="74c24-111">Informácie o vstavanej citlivých druhov a čo DLP politiky hľadá pri detekcii citlivý typ, pozri: [Aké typy citlivé informácie vyhľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="74c24-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="74c24-112">**Typy vlastných citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="74c24-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="74c24-113">Ak sa snažíte vytvoriť typy vlastných citlivých informácií, použite nasledujúci článok informácie o tom, ako vytvoriť vlastné citlivý typ: [vytvoriť typ vlastné citlivé informácie](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="74c24-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="74c24-114">**Test DLP politiky**</span><span class="sxs-lookup"><span data-stu-id="74c24-114">**Test a DLP policy**</span></span>

<span data-ttu-id="74c24-115">Otestovať vaše dáta s typom vstavané alebo vlastné citlivé informácie, použite možnosť **skúšky typu** podľa **klasifikácie** > **typy citlivých informácií**.</span><span class="sxs-lookup"><span data-stu-id="74c24-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="74c24-116">Ďalšie informácie sa nachádzajú v téme [Test vlastné citlivé informácie typy](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="74c24-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="74c24-117">**Správy**</span><span class="sxs-lookup"><span data-stu-id="74c24-117">**Reports**</span></span>
  
- <span data-ttu-id="74c24-118">Nahliadnite viac citlivé údaje s [DLP správ.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="74c24-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="74c24-119">Pozrite si konkrétne podrobnosti udalosti [Incident správa](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="74c24-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>

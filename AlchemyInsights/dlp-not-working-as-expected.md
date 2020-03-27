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
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977453"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="2a8fb-102">DLP nefunguje podľa očakávania</span><span class="sxs-lookup"><span data-stu-id="2a8fb-102">DLP not working as expected</span></span>

<span data-ttu-id="2a8fb-103">**Dôležité**: počas týchto nebývalé časy, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné-navštívte [SharePoint Online dočasné funkcie úpravy](https://aka.ms/ODSPAdjustments) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="2a8fb-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="2a8fb-104">**Nastavenie DLP**</span><span class="sxs-lookup"><span data-stu-id="2a8fb-104">**Setting up DLP**</span></span>

<span data-ttu-id="2a8fb-105">Máte problémy s **únikom údajov (DLP)** v balíku Office 365 nefunguje podľa očakávania?</span><span class="sxs-lookup"><span data-stu-id="2a8fb-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="2a8fb-106">Ak áno, uistite sa, že **DLP politika** je nastavená správne, a že vaše údaje obsahuje to, čo **DLP politika** hľadá, keď sa hodnotí.</span><span class="sxs-lookup"><span data-stu-id="2a8fb-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="2a8fb-107">Politiky DLP vám umožňujú identifikovať a chrániť citlivé informácie vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="2a8fb-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="2a8fb-108">Ak chcete nastaviť politiky DLP, použite informácie [tu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="2a8fb-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="2a8fb-109">**Čo DLP politiky Hľadať**</span><span class="sxs-lookup"><span data-stu-id="2a8fb-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="2a8fb-110">Pri použití **vstavané typy citlivých informácií** v Office 365 zabezpečenia a súladu centrum, DLP politiky Hľadať špecifické vzory a prvky pri zisťovaní týchto citlivých typov.</span><span class="sxs-lookup"><span data-stu-id="2a8fb-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="2a8fb-111">**Vstavané typy citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="2a8fb-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="2a8fb-112">Informácie o vstavaných citlivých typoch a o tom, čo politika DLP vyhľadáva pri zisťovaní citlivého typu, nájdete v téme: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="2a8fb-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="2a8fb-113">**Vlastné citlivé typy informácií**</span><span class="sxs-lookup"><span data-stu-id="2a8fb-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="2a8fb-114">Ak sa pokúšate vytvoriť vlastné citlivé typy informácií, použite nasledujúci článok informácie o tom, ako vytvoriť vlastný citlivý typ: [vytvoriť vlastné citlivé informácie typu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="2a8fb-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="2a8fb-115">**Testovanie politiky DLP**</span><span class="sxs-lookup"><span data-stu-id="2a8fb-115">**Test a DLP policy**</span></span>

<span data-ttu-id="2a8fb-116">Ak chcete otestovať údaje pomocou vstavaného alebo vlastného typu citlivých informácií, použite možnosť **typ testu** podľa **klasifikácie** > **citlivých typov**informácií.</span><span class="sxs-lookup"><span data-stu-id="2a8fb-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="2a8fb-117">Ďalšie informácie nájdete v téme [testovanie vlastných typov citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="2a8fb-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="2a8fb-118">**Správy**</span><span class="sxs-lookup"><span data-stu-id="2a8fb-118">**Reports**</span></span>
  
- <span data-ttu-id="2a8fb-119">Získajte citlivé údaje s [prehľadom DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="2a8fb-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="2a8fb-120">Pozrite si konkrétne podrobnosti udalosti so [správou o incidente](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="2a8fb-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>

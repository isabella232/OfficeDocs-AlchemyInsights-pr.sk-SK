---
title: DLP nefunguje podľa očakávania
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e96904e2f0da2fe1fafb3f8722465eaf22681b71
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507493"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="a08d5-102">DLP nefunguje podľa očakávania</span><span class="sxs-lookup"><span data-stu-id="a08d5-102">DLP not working as expected</span></span>

<span data-ttu-id="a08d5-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="a08d5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="a08d5-104">**Nastavenie DLP**</span><span class="sxs-lookup"><span data-stu-id="a08d5-104">**Setting up DLP**</span></span>

<span data-ttu-id="a08d5-105">Máte problémy s **funkciou Ochrana pred únikom údajov (DLP)** v službách Office 365, ktoré nefungujú podľa očakávania?</span><span class="sxs-lookup"><span data-stu-id="a08d5-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="a08d5-106">Ak áno, skontrolujte, či je **politika DLP** nastavená správne a či vaše údaje obsahujú to, čo **politika DLP** hľadá pri hodnotení.</span><span class="sxs-lookup"><span data-stu-id="a08d5-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="a08d5-107">Politiky DLP umožňujú identifikovať a chrániť citlivé informácie vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="a08d5-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="a08d5-108">Ak chcete nastaviť politiky DLP, použite informácie [tu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="a08d5-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="a08d5-109">**Čo je to za politiky DLP**</span><span class="sxs-lookup"><span data-stu-id="a08d5-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="a08d5-110">Pri používaní **vstavaných typov citlivých informácií v** centrách zabezpečenia a dodržiavania súladu politiky DLP hľadajú pri zisťovaní týchto citlivých typov špecifické vzory a prvky.</span><span class="sxs-lookup"><span data-stu-id="a08d5-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="a08d5-111">**Vstavané typy citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="a08d5-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="a08d5-112">Informácie o vstavaných typoch citlivých údajov a o tom, čo politika DLP hľadá pri zisťovaní citlivého typu, nájdete v téme: [Čo vyzerajú typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="a08d5-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="a08d5-113">**Vlastné typy citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="a08d5-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="a08d5-114">Ak sa pokúšate vytvoriť vlastné typy citlivých informácií, informácie o vytvorení vlastného typu citlivého obsahu: [Vytvorenie vlastného typu citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)použite nasledujúci článok.</span><span class="sxs-lookup"><span data-stu-id="a08d5-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="a08d5-115">**Testovanie politiky DLP**</span><span class="sxs-lookup"><span data-stu-id="a08d5-115">**Test a DLP policy**</span></span>

<span data-ttu-id="a08d5-116">Ak chcete otestovať údaje pomocou vstavaného alebo vlastného typu citlivých informácií, použite možnosť **Typ testu** v časti **Klasifikácie**  >  **Citlivé typy informácií**.</span><span class="sxs-lookup"><span data-stu-id="a08d5-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="a08d5-117">Ďalšie informácie nájdete v téme [Testovanie vlastných typov citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="a08d5-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="a08d5-118">**Správy**</span><span class="sxs-lookup"><span data-stu-id="a08d5-118">**Reports**</span></span>
  
- <span data-ttu-id="a08d5-119">Získajte prehľady citlivých údajov pomocou [zostáv DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="a08d5-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="a08d5-120">Pozrite si konkrétne podrobnosti o udalosti so [správou o incidente](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="a08d5-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>

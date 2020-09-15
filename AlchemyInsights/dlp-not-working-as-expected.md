---
title: DLP nefunguje podľa očakávania
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679708"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="cc60e-102">DLP nefunguje podľa očakávania</span><span class="sxs-lookup"><span data-stu-id="cc60e-102">DLP not working as expected</span></span>

<span data-ttu-id="cc60e-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="cc60e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="cc60e-104">**Nastavenie DLP**</span><span class="sxs-lookup"><span data-stu-id="cc60e-104">**Setting up DLP**</span></span>

<span data-ttu-id="cc60e-105">Vyskytli sa problémy s **prevenciou pred stratou údajov (DLP)** v Office 365 nefunguje podľa očakávania?</span><span class="sxs-lookup"><span data-stu-id="cc60e-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="cc60e-106">Ak áno, uistite sa, že **politika DLP** je nastavená správne a že vaše údaje obsahujú informácie o tom, čo **politika DLP** hľadá pri jej vyhodnocovaní.</span><span class="sxs-lookup"><span data-stu-id="cc60e-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="cc60e-107">Politiky DLP vám umožňujú identifikovať a chrániť citlivé informácie vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="cc60e-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="cc60e-108">Ak chcete nastaviť politiky DLP, použite informácie [tu](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span><span class="sxs-lookup"><span data-stu-id="cc60e-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="cc60e-109">**Čo politiky DLP hľadajú**</span><span class="sxs-lookup"><span data-stu-id="cc60e-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="cc60e-110">Pri používaní **vstavaných typov citlivých informácií** v centre zabezpečenia a dodržiavania súladu majú politiky DLP pri zisťovaní týchto citlivých typov vyhľadať konkrétne vzory a prvky.</span><span class="sxs-lookup"><span data-stu-id="cc60e-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="cc60e-111">**Vstavané typy citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="cc60e-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="cc60e-112">Informácie o vstavaných citlivých typoch a o tom, čo politika DLP vyhľadáva pri zisťovaní citlivého typu, nájdete v téme: [Aké typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)vyhľadávajú.</span><span class="sxs-lookup"><span data-stu-id="cc60e-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="cc60e-113">**Vlastné typy citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="cc60e-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="cc60e-114">Ak sa pokúšate vytvoriť vlastné typy citlivých informácií, použite nasledujúci článok, kde nájdete informácie o tom, ako vytvoriť vlastný typ citlivosti: [Vytvorenie vlastného typu citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="cc60e-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="cc60e-115">**Testovanie politiky DLP**</span><span class="sxs-lookup"><span data-stu-id="cc60e-115">**Test a DLP policy**</span></span>

<span data-ttu-id="cc60e-116">Ak chcete otestovať údaje pomocou vstavaného alebo vlastného typu citlivých informácií, použite možnosť **testovať typ** v časti **klasifikácie**  >  **citlivé typy informácií**.</span><span class="sxs-lookup"><span data-stu-id="cc60e-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="cc60e-117">Ďalšie informácie nájdete v téme [testovanie vlastných typov citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="cc60e-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="cc60e-118">**Zostavy**</span><span class="sxs-lookup"><span data-stu-id="cc60e-118">**Reports**</span></span>
  
- <span data-ttu-id="cc60e-119">Získajte podrobné informácie o citlivých údajoch so [zostavami DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="cc60e-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="cc60e-120">Pozrite si konkrétne podrobnosti o udalosti s [hlásením incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="cc60e-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>

---
title: Pravidlo DLP pre číslo cestovného pasu USA a Spojeného kráľovstva nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507313"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="4de4b-102">Problémy s DLP - čísla pasov VUSA a Veľkej Británii</span><span class="sxs-lookup"><span data-stu-id="4de4b-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="4de4b-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="4de4b-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4de4b-104">**DLP problémy s číslami pasov uSA a Veľkej Británie**</span><span class="sxs-lookup"><span data-stu-id="4de4b-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="4de4b-105">Máte problémy s **funkciou Ochrana pred únikom údajov (DLP),** ktorá nepracuje pre obsah obsahujúci **číslo pasu USA a Veľkej Británie** pri používaní typu citlivých informácií DLP v systéme O365?</span><span class="sxs-lookup"><span data-stu-id="4de4b-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="4de4b-106">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá pri hodnotení.</span><span class="sxs-lookup"><span data-stu-id="4de4b-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="4de4b-107">Napríklad v prípade politiky **čísla pasov USA a Spojeného kráľovstva** nakonfigurovanej s úrovňou spoľahlivosti 75 % sa vyhodnotia nasledujúce možnosti a musí sa zistiť, aby sa pravidlo spustilo.</span><span class="sxs-lookup"><span data-stu-id="4de4b-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="4de4b-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Deväť číslic</span><span class="sxs-lookup"><span data-stu-id="4de4b-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="4de4b-109">**[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Deväť po sebe idúcich číslic</span><span class="sxs-lookup"><span data-stu-id="4de4b-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="4de4b-110">**[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, nie je tam žiadny kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="4de4b-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="4de4b-111">**[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Politika DLP je 75% presvedčená, že zistila tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="4de4b-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4de4b-112">Funkcia Func_usa_uk_passport nájde obsah, ktorý sa zhoduje so vzorom.</span><span class="sxs-lookup"><span data-stu-id="4de4b-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4de4b-113">Nájde sa kľúčové slovo z Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="4de4b-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="4de4b-114">Napríklad nasledujúca vzorka by sa spustiť pre **us / UK číslo pasu číslo** politiky: Číslo cestovného pasu USA 123456789</span><span class="sxs-lookup"><span data-stu-id="4de4b-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="4de4b-115">Ďalšie informácie o tom, čo je potrebné pre US / UK Passport číslo, ktoré majú byť zistené pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Čo citlivé informácie typy hľadať us / UK Passport číslo](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="4de4b-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="4de4b-116">Pomocou iného vstavaného typu citlivých informácií nájdete v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Čo vyzerajú typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="4de4b-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  
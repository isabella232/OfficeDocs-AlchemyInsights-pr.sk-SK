---
title: Pravidlo DLP pre číslo kreditnej karty nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 80ff41b3e746f95278ccbf0df19eebb61f7f9ee0
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704216"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="9311d-102">DLP problémy s číslami kreditných kariet</span><span class="sxs-lookup"><span data-stu-id="9311d-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="9311d-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="9311d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="9311d-104">**DLP problémy s číslami kreditných kariet**</span><span class="sxs-lookup"><span data-stu-id="9311d-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="9311d-105">Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **číslo kreditnej karty** pri použití DLP citlivé informácie typu v služby O365?</span><span class="sxs-lookup"><span data-stu-id="9311d-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="9311d-106">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie na spustenie politiky DLP, keď je hodnotená.</span><span class="sxs-lookup"><span data-stu-id="9311d-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="9311d-107">Napríklad pri **politike kreditnej karty** nakonfigurovanej s úrovňou spoľahlivosti 85% sa vyhodnocujú nasledovné a musia sa zistiť pre pravidlo, ktoré sa má spustiť:</span><span class="sxs-lookup"><span data-stu-id="9311d-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="9311d-108">**[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 číslic, ktoré môžu byť formátované alebo neformátovaný (dddddddddddddddd) a musí prejsť Luhn test.</span><span class="sxs-lookup"><span data-stu-id="9311d-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="9311d-109">**[Vzor:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Veľmi zložitý a robustný vzor, ktorý detekuje karty zo všetkých hlavných značiek po celom svete, vrátane Visa, MasterCard, Discover Card, JCB, American Express, darčekové karty, a Diner karty.</span><span class="sxs-lookup"><span data-stu-id="9311d-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="9311d-110">**[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Áno, Luhn kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="9311d-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="9311d-111">**[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Politika DLP je 85% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="9311d-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="9311d-112">Funkcia Func_credit_card vyhľadá obsah zodpovedajúci vzoru.</span><span class="sxs-lookup"><span data-stu-id="9311d-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="9311d-113">Je splnená jedna z nasledujúcich možností:</span><span class="sxs-lookup"><span data-stu-id="9311d-113">One of the following is true:</span></span>

  - <span data-ttu-id="9311d-114">Našiel sa kľúčové slovo z Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="9311d-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="9311d-115">Kľúčové slovo z Keyword_cc_name sa nachádza</span><span class="sxs-lookup"><span data-stu-id="9311d-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="9311d-116">Funkcia Func_expiration_date nájde dátum v správnom formáte dátumu.</span><span class="sxs-lookup"><span data-stu-id="9311d-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="9311d-117">Kontrolný súčet prejde</span><span class="sxs-lookup"><span data-stu-id="9311d-117">The checksum passes</span></span>

    <span data-ttu-id="9311d-118">Napríklad nasledujúca vzorka by spúšťač DLP číslo kreditnej karty:</span><span class="sxs-lookup"><span data-stu-id="9311d-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="9311d-119">Vízum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="9311d-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="9311d-120">Uplynie: 2/2009</span><span class="sxs-lookup"><span data-stu-id="9311d-120">Expires: 2/2009</span></span>

<span data-ttu-id="9311d-121">Ďalšie informácie o tom, čo je potrebné pre **číslo kreditnej karty** , ktoré sa majú zistiť pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Aké typy citlivých informácií Hľadať kreditnú kartu #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="9311d-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="9311d-122">Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="9311d-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  
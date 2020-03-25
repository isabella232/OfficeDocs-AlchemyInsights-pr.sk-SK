---
title: Pravidlo DLP pre číslo kreditnej karty nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932458"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="b20d0-102">DLP problémy s číslami kreditných kariet</span><span class="sxs-lookup"><span data-stu-id="b20d0-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="b20d0-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="b20d0-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b20d0-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="b20d0-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b20d0-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="b20d0-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b20d0-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="b20d0-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b20d0-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="b20d0-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b20d0-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="b20d0-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b20d0-109">**DLP problémy s číslami kreditných kariet**</span><span class="sxs-lookup"><span data-stu-id="b20d0-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="b20d0-110">Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **číslo kreditnej karty** pri použití DLP citlivé informácie typu v služby O365?</span><span class="sxs-lookup"><span data-stu-id="b20d0-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="b20d0-111">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie na spustenie politiky DLP, keď je hodnotená.</span><span class="sxs-lookup"><span data-stu-id="b20d0-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="b20d0-112">Napríklad pri **politike kreditnej karty** nakonfigurovanej s úrovňou spoľahlivosti 85% sa vyhodnocujú nasledovné a musia sa zistiť pre pravidlo, ktoré sa má spustiť:</span><span class="sxs-lookup"><span data-stu-id="b20d0-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="b20d0-113">**[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 číslic, ktoré môžu byť formátované alebo neformátovaný (dddddddddddddddd) a musí prejsť Luhn test.</span><span class="sxs-lookup"><span data-stu-id="b20d0-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="b20d0-114">**[Vzor:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Veľmi zložitý a robustný vzor, ktorý detekuje karty zo všetkých hlavných značiek po celom svete, vrátane Visa, MasterCard, Discover Card, JCB, American Express, darčekové karty, a Diner karty.</span><span class="sxs-lookup"><span data-stu-id="b20d0-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="b20d0-115">**[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Áno, Luhn kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="b20d0-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="b20d0-116">**[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** Politika DLP je 85% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="b20d0-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="b20d0-117">Funkcia Func_credit_card vyhľadá obsah zodpovedajúci vzoru.</span><span class="sxs-lookup"><span data-stu-id="b20d0-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="b20d0-118">Je splnená jedna z nasledujúcich možností:</span><span class="sxs-lookup"><span data-stu-id="b20d0-118">One of the following is true:</span></span>

  - <span data-ttu-id="b20d0-119">Našiel sa kľúčové slovo z Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="b20d0-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="b20d0-120">Kľúčové slovo z Keyword_cc_name sa nachádza</span><span class="sxs-lookup"><span data-stu-id="b20d0-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="b20d0-121">Funkcia Func_expiration_date nájde dátum v správnom formáte dátumu.</span><span class="sxs-lookup"><span data-stu-id="b20d0-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="b20d0-122">Kontrolný súčet prejde</span><span class="sxs-lookup"><span data-stu-id="b20d0-122">The checksum passes</span></span>

    <span data-ttu-id="b20d0-123">Napríklad nasledujúca vzorka by spúšťač DLP číslo kreditnej karty:</span><span class="sxs-lookup"><span data-stu-id="b20d0-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="b20d0-124">Vízum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="b20d0-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="b20d0-125">Uplynie: 2/2009</span><span class="sxs-lookup"><span data-stu-id="b20d0-125">Expires: 2/2009</span></span>

<span data-ttu-id="b20d0-126">Ďalšie informácie o tom, čo je potrebné pre **číslo kreditnej karty** , ktoré sa majú zistiť pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Aké typy citlivých informácií Hľadať kreditnú kartu #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="b20d0-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="b20d0-127">Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="b20d0-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  
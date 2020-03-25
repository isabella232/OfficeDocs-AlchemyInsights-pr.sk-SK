---
title: Pravidlo DLP pre SSN nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932550"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="f4cc5-102">DLP problémy s číslami sociálneho zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="f4cc5-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="f4cc5-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="f4cc5-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f4cc5-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="f4cc5-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f4cc5-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="f4cc5-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f4cc5-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="f4cc5-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f4cc5-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="f4cc5-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f4cc5-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="f4cc5-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f4cc5-109">**DLP problémy s SSNs**</span><span class="sxs-lookup"><span data-stu-id="f4cc5-109">**DLP issues with SSNs**</span></span>

<span data-ttu-id="f4cc5-110">Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **číslo sociálneho zabezpečenia (SSN)** pri používaní citlivé informácie typu v balíku Office 365?</span><span class="sxs-lookup"><span data-stu-id="f4cc5-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="f4cc5-111">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo DLP politiky hľadá.</span><span class="sxs-lookup"><span data-stu-id="f4cc5-111">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="f4cc5-112">Napríklad pre politiku SSN nakonfigurovaný s úrovňou spoľahlivosti 85%, sú vyhodnotené a musia byť detekované pre pravidlo spustiť:</span><span class="sxs-lookup"><span data-stu-id="f4cc5-112">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="f4cc5-113">**[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 číslic, ktoré môžu byť vo formáte alebo neformátovaný vzor</span><span class="sxs-lookup"><span data-stu-id="f4cc5-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="f4cc5-114">**[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie Hľadať SSNs v štyroch rôznych vzorov:</span><span class="sxs-lookup"><span data-stu-id="f4cc5-114">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="f4cc5-115">Func_ssn nájde SSNs s pre-2011 silné formátovanie, ktoré sú formátované pomlčkami alebo medzerami (DDD-DD-dddd alebo DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="f4cc5-115">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f4cc5-116">Func_unformatted_ssn nájde SSNs s pre-2011 silné formátovanie, ktoré sú neformátované ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f4cc5-116">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="f4cc5-117">Func_randomized_formatted_ssn nájde post-2011 SSNs, ktoré sú formátované pomlčkami alebo medzerami (DDD-DD-dddd alebo DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="f4cc5-117">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="f4cc5-118">Func_randomized_unformatted_ssn nájde post-2011 SSNs, ktoré sú neformátované ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="f4cc5-118">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="f4cc5-119">**[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nie, nie je tam žiadny kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="f4cc5-119">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="f4cc5-120">**[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Politika DLP je 85% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="f4cc5-120">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="f4cc5-121">[Funkcia Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) vyhľadá obsah zodpovedajúci vzoru.</span><span class="sxs-lookup"><span data-stu-id="f4cc5-121">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="f4cc5-122">Našiel sa kľúčové slovo z [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="f4cc5-122">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="f4cc5-123">Príklady kľúčových slov zahŕňa: *sociálne zabezpečenie, sociálne zabezpečenie #, SoC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="f4cc5-123">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="f4cc5-124">Napríklad nasledujúca vzorka by vyvolať DLP SSN politiky: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="f4cc5-124">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="f4cc5-125">Ďalšie informácie o tom, čo je potrebné pre SSNs byť detekovaný pre váš obsah, nájdete v nasledujúcej časti v tomto článku: [Aké typy citlivých informácií Hľadať SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="f4cc5-125">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="f4cc5-126">Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="f4cc5-126">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  
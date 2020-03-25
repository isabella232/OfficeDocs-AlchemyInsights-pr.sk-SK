---
title: Pravidlo DLP pre číslo pasu USA/UK nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931277"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="fb1e6-102">Problémy s DLP-USA/UK čísla pasu</span><span class="sxs-lookup"><span data-stu-id="fb1e6-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="fb1e6-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="fb1e6-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="fb1e6-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="fb1e6-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="fb1e6-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="fb1e6-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="fb1e6-109">**DLP problémy s USA/UK čísla pasu**</span><span class="sxs-lookup"><span data-stu-id="fb1e6-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="fb1e6-110">Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **USA/UK číslo pasu** pri použití DLP citlivé informácie typu v službe O365?</span><span class="sxs-lookup"><span data-stu-id="fb1e6-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="fb1e6-111">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo DLP politika hľadá, keď je hodnotená.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="fb1e6-112">Napríklad v prípade politiky **čísla pasu USA/Spojeného kráľovstva** nakonfigurovanej s úrovňou spoľahlivosti 75% sa vyhodnocujú nasledovné a musia sa zistiť pre pravidlo na spustenie</span><span class="sxs-lookup"><span data-stu-id="fb1e6-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="fb1e6-113">**[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deväť číslic</span><span class="sxs-lookup"><span data-stu-id="fb1e6-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="fb1e6-114">**[Vzor:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deväť po sebe idúcich číslic</span><span class="sxs-lookup"><span data-stu-id="fb1e6-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="fb1e6-115">**[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie je tam žiadny kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="fb1e6-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="fb1e6-116">**[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Politika DLP je 75% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="fb1e6-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="fb1e6-117">Funkcia Func_usa_uk_passport vyhľadá obsah zodpovedajúci vzoru.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="fb1e6-118">Našiel sa kľúčové slovo z Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="fb1e6-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="fb1e6-119">Napríklad nasledujúca vzorka by spúšť pre **USA/UK Passport číslo** politiky: US passport číslo 123456789</span><span class="sxs-lookup"><span data-stu-id="fb1e6-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="fb1e6-120">Ďalšie informácie o tom, čo je potrebné pre USA/UK číslo pasu, ktoré majú byť detekované pre váš obsah, nájdete v nasledujúcej časti v tomto článku: [Aké typy citlivých informácií hľadať pre nás/UK číslo pasu](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="fb1e6-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="fb1e6-121">Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="fb1e6-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  
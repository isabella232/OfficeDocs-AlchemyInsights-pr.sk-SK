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
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977121"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="838e5-102">Problémy s DLP-USA/UK čísla pasu</span><span class="sxs-lookup"><span data-stu-id="838e5-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="838e5-103">**Dôležité**: počas týchto nebývalé časy, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné-navštívte [SharePoint Online dočasné funkcie úpravy](https://aka.ms/ODSPAdjustments) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="838e5-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="838e5-104">**DLP problémy s USA/UK čísla pasu**</span><span class="sxs-lookup"><span data-stu-id="838e5-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="838e5-105">Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **USA/UK číslo pasu** pri použití DLP citlivé informácie typu v službe O365?</span><span class="sxs-lookup"><span data-stu-id="838e5-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="838e5-106">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo DLP politika hľadá, keď je hodnotená.</span><span class="sxs-lookup"><span data-stu-id="838e5-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="838e5-107">Napríklad v prípade politiky **čísla pasu USA/Spojeného kráľovstva** nakonfigurovanej s úrovňou spoľahlivosti 75% sa vyhodnocujú nasledovné a musia sa zistiť pre pravidlo na spustenie</span><span class="sxs-lookup"><span data-stu-id="838e5-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="838e5-108">**[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deväť číslic</span><span class="sxs-lookup"><span data-stu-id="838e5-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="838e5-109">**[Vzor:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deväť po sebe idúcich číslic</span><span class="sxs-lookup"><span data-stu-id="838e5-109">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="838e5-110">**[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, nie je tam žiadny kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="838e5-110">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="838e5-111">**[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** Politika DLP je 75% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="838e5-111">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="838e5-112">Funkcia Func_usa_uk_passport vyhľadá obsah zodpovedajúci vzoru.</span><span class="sxs-lookup"><span data-stu-id="838e5-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="838e5-113">Našiel sa kľúčové slovo z Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="838e5-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="838e5-114">Napríklad nasledujúca vzorka by spúšť pre **USA/UK Passport číslo** politiky: US passport číslo 123456789</span><span class="sxs-lookup"><span data-stu-id="838e5-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="838e5-115">Ďalšie informácie o tom, čo je potrebné pre USA/UK číslo pasu, ktoré majú byť detekované pre váš obsah, nájdete v nasledujúcej časti v tomto článku: [Aké typy citlivých informácií hľadať pre nás/UK číslo pasu](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="838e5-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="838e5-116">Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="838e5-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  
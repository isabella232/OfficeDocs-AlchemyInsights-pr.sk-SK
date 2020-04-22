---
title: Pravidlo DLP pre SSN nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: cfe884a207490a19325ce059652de158c16dc801
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704100"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="7cf11-102">DLP problémy s číslami sociálneho zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="7cf11-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="7cf11-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="7cf11-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="7cf11-104">**DLP problémy s SSNs**</span><span class="sxs-lookup"><span data-stu-id="7cf11-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="7cf11-105">Máte problémy s **únikom údajov (DLP)** nepracuje pre obsah obsahujúci **číslo sociálneho zabezpečenia (SSN)** pri používaní citlivé informácie typu v balíku Office 365?</span><span class="sxs-lookup"><span data-stu-id="7cf11-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="7cf11-106">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo DLP politiky hľadá.</span><span class="sxs-lookup"><span data-stu-id="7cf11-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="7cf11-107">Napríklad pre politiku SSN nakonfigurovaný s úrovňou spoľahlivosti 85%, sú vyhodnotené a musia byť detekované pre pravidlo spustiť:</span><span class="sxs-lookup"><span data-stu-id="7cf11-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="7cf11-108">**[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 číslic, ktoré môžu byť vo formáte alebo neformátovaný vzor</span><span class="sxs-lookup"><span data-stu-id="7cf11-108">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="7cf11-109">**[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie Hľadať SSNs v štyroch rôznych vzorov:</span><span class="sxs-lookup"><span data-stu-id="7cf11-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="7cf11-110">Func_ssn nájde SSNs s pre-2011 silné formátovanie, ktoré sú formátované pomlčkami alebo medzerami (DDD-DD-dddd alebo DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="7cf11-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="7cf11-111">Func_unformatted_ssn nájde SSNs s pre-2011 silné formátovanie, ktoré sú neformátované ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="7cf11-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="7cf11-112">Func_randomized_formatted_ssn nájde post-2011 SSNs, ktoré sú formátované pomlčkami alebo medzerami (DDD-DD-dddd alebo DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="7cf11-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="7cf11-113">Func_randomized_unformatted_ssn nájde post-2011 SSNs, ktoré sú neformátované ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="7cf11-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="7cf11-114">**[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nie, nie je tam žiadny kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="7cf11-114">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="7cf11-115">**[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** Politika DLP je 85% presvedčená, že je detekovaný tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="7cf11-115">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="7cf11-116">[Funkcia Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) vyhľadá obsah zodpovedajúci vzoru.</span><span class="sxs-lookup"><span data-stu-id="7cf11-116">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="7cf11-117">Našiel sa kľúčové slovo z [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="7cf11-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="7cf11-118">Príklady kľúčových slov zahŕňa: *sociálne zabezpečenie, sociálne zabezpečenie #, SoC SEC, SSN* .</span><span class="sxs-lookup"><span data-stu-id="7cf11-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="7cf11-119">Napríklad nasledujúca vzorka by vyvolať DLP SSN politiky: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="7cf11-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="7cf11-120">Ďalšie informácie o tom, čo je potrebné pre SSNs byť detekovaný pre váš obsah, nájdete v nasledujúcej časti v tomto článku: [Aké typy citlivých informácií Hľadať SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="7cf11-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="7cf11-121">Pomocou iného vstavaného typu citlivé informácie nájdete v nasledujúcom článku informácie o tom, čo je potrebné pre iné typy: [Aké typy citlivých informácií Hľadať](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="7cf11-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  
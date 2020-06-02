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
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507385"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="4ac3f-102">DLP otázky s číslami sociálneho zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="4ac3f-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="4ac3f-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="4ac3f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4ac3f-104">**Problémy s DLP s SSNs**</span><span class="sxs-lookup"><span data-stu-id="4ac3f-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="4ac3f-105">Máte problémy s **funkciou Ochrana pred únikom údajov (DLP)** nefunguje pre obsah obsahujúci **číslo sociálneho zabezpečenia (SSN)** pri používaní typu citlivých informácií v microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="4ac3f-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="4ac3f-106">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá.</span><span class="sxs-lookup"><span data-stu-id="4ac3f-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4ac3f-107">Napríklad pre politiku SSN nakonfigurovaný s úrovňou spoľahlivosti 85%, sa vyhodnotia nasledovné a musí byť detekovaný pre pravidlo spustiť:</span><span class="sxs-lookup"><span data-stu-id="4ac3f-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4ac3f-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 číslic, ktoré môžu byť vo formáte formátovaný alebo neformátovaný vzor</span><span class="sxs-lookup"><span data-stu-id="4ac3f-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="4ac3f-109">**[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie hľadajú SSN v štyroch rôznych vzoroch:</span><span class="sxs-lookup"><span data-stu-id="4ac3f-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="4ac3f-110">Func_ssn nájde SSN so silným formátovaním pred 2011, ktoré sú formátované pomlčkami alebo medzerami (ddd-ddddd alebo ddd dd dd dd ddddd)</span><span class="sxs-lookup"><span data-stu-id="4ac3f-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4ac3f-111">Func_unformatted_ssn nájde SSN s pre-2011 silné formátovanie, ktoré sú neformátované ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4ac3f-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="4ac3f-112">Func_randomized_formatted_ssn nájde ssn po roku 2011, ktoré sú formátované pomlčkami alebo medzerami (ddd-ddddd alebo ddd dd dd ddddd)</span><span class="sxs-lookup"><span data-stu-id="4ac3f-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4ac3f-113">Func_randomized_unformatted_ssn nájde ssn po roku 2011, ktoré nie sú formátované ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4ac3f-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="4ac3f-114">**[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nie, nie je tam žiadny kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="4ac3f-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="4ac3f-115">**[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Politika DLP je 85% presvedčená, že sa zistil tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="4ac3f-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4ac3f-116">[Funkcia Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) nájde obsah, ktorý sa zhoduje so vzorom.</span><span class="sxs-lookup"><span data-stu-id="4ac3f-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4ac3f-117">Nájde sa kľúčové slovo z [Keyword_ssn.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn)</span><span class="sxs-lookup"><span data-stu-id="4ac3f-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="4ac3f-118">Príklady kľúčových slov zahŕňajú: *Sociálne zabezpečenie, sociálne zabezpečenie #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="4ac3f-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="4ac3f-119">Napríklad nasledujúca vzorka by sa spustiť pre Politiku DLP SSN: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="4ac3f-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="4ac3f-120">Ďalšie informácie o tom, čo je potrebné pre SSN zistiť obsah, nájdete v nasledujúcej časti tohto článku: [Čo citlivé informácie typy hľadať SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="4ac3f-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4ac3f-121">Pomocou iného vstavaného typu citlivých informácií nájdete v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Čo vyzerajú typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="4ac3f-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  
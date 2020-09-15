---
title: Pravidlo DLP pre SSN nefunguje
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679384"
---
# <a name="dlp-issues-with-social-security-numbers"></a><span data-ttu-id="4baa3-102">Problémy s DLP s číslami sociálneho zabezpečenia</span><span class="sxs-lookup"><span data-stu-id="4baa3-102">DLP issues with Social Security Numbers</span></span>

<span data-ttu-id="4baa3-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="4baa3-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4baa3-104">**Problémy s DLP s čísla SSN**</span><span class="sxs-lookup"><span data-stu-id="4baa3-104">**DLP issues with SSNs**</span></span>

<span data-ttu-id="4baa3-105">Vyskytli sa problémy so zabezpečením **ochrany pred únikom údajov (DLP)** , ktoré nefungujú s obsahom, ktorý obsahuje **číslo sociálneho zabezpečenia (SSN)** pri použití citlivého typu informácií v Microsoft 365?</span><span class="sxs-lookup"><span data-stu-id="4baa3-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Microsoft 365?</span></span> <span data-ttu-id="4baa3-106">Ak áno, uistite sa, že obsah obsahuje potrebné informácie o tom, čo sa pri vyhľadávaní politiky DLP nachádza.</span><span class="sxs-lookup"><span data-stu-id="4baa3-106">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="4baa3-107">Napríklad pre politiku SSN nakonfigurovanú s úrovňou spoľahlivosti 85% sa vyhodnotia a pre pravidlo sa musí zistiť, či sa má spustiť nasledovné:</span><span class="sxs-lookup"><span data-stu-id="4baa3-107">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="4baa3-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 číslic, ktoré môžu byť formátované alebo nenaformátované</span><span class="sxs-lookup"><span data-stu-id="4baa3-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span>

- <span data-ttu-id="4baa3-109">**[Vzor:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie vyhľadávajú čísla SSN v štyroch rôznych vzorcoch:</span><span class="sxs-lookup"><span data-stu-id="4baa3-109">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span>

  - <span data-ttu-id="4baa3-110">Func_ssn nájde čísla SSN s vopred 2011 silným formátovaním s pomlčkami alebo medzerami (DDD – DD-dddd alebo DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="4baa3-110">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4baa3-111">Func_unformatted_ssn nájde čísla SSN s formátovaním pre-2011 silné formátovanie, ktoré nie je formátované ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4baa3-111">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>

  - <span data-ttu-id="4baa3-112">Func_randomized_formatted_ssn nájde čísla SSN post-2011, ktoré sú formátované pomlčkami alebo medzerami (DDD – DD-dddd alebo DDD DD dddd)</span><span class="sxs-lookup"><span data-stu-id="4baa3-112">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>

  - <span data-ttu-id="4baa3-113">Func_randomized_unformatted_ssn nájde čísla SSN post-2011, ktoré nie sú formátované ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="4baa3-113">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>

- <span data-ttu-id="4baa3-114">**[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nie, kontrolný súčet nie je k dispozícii</span><span class="sxs-lookup"><span data-stu-id="4baa3-114">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** No, there is no Checksum</span></span>

- <span data-ttu-id="4baa3-115">**[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Politika DLP je 85% presvedčená, že zistí tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="4baa3-115">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="4baa3-116">[Funkcia Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) nájde obsah, ktorý zodpovedá vzoru.</span><span class="sxs-lookup"><span data-stu-id="4baa3-116">The [function Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) finds content that matches the pattern.</span></span>

  - <span data-ttu-id="4baa3-117">Nájde sa kľúčové slovo z [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="4baa3-117">A keyword from [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) is found.</span></span> <span data-ttu-id="4baa3-118">Príklady kľúčových slov zahŕňajú:  *sociálne zabezpečenie, sociálna bezpečnosť #, SoC SEC, SSN*  .</span><span class="sxs-lookup"><span data-stu-id="4baa3-118">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="4baa3-119">Pre politiku DLP SSN by sa napríklad spustila nasledujúca vzorka: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="4baa3-119">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
  
<span data-ttu-id="4baa3-120">Ďalšie informácie o tom, čo sa vyžaduje pre čísla SSN, ktoré sa majú zistiť pre svoj obsah, nájdete v tejto časti tohto článku: [Aké typy citlivých informácií vyhľadávajú čísla SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="4baa3-120">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="4baa3-121">Ak používate iný vstavaný typ citlivých informácií, prečítajte si v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="4baa3-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  
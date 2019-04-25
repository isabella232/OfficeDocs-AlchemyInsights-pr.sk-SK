---
title: DLP pravidlo pre SSN nefunguje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404432"
---
<span data-ttu-id="13e32-102">Máte problémy s **Data Loss Prevention (DLP)** nefunguje pre obsah obsahujúce **Číslo sociálneho poistenia (SSN)** , pri použití typu citlivých informácií v službách Office 365?</span><span class="sxs-lookup"><span data-stu-id="13e32-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="13e32-103">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie pre to, čo hľadá DLP politiky.</span><span class="sxs-lookup"><span data-stu-id="13e32-103">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="13e32-104">Napríklad SSN politiky nakonfigurované s 85% úrovni spoľahlivosti, takto sa vyhodnocujú a musí zistiť pravidlo spustiť:</span><span class="sxs-lookup"><span data-stu-id="13e32-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="13e32-105">**[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 číslic, ktoré môže byť formátovaný alebo neformátovaný vzor</span><span class="sxs-lookup"><span data-stu-id="13e32-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="13e32-106">**[Vzorka:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Štyri funkcie Hľadať SSNs v štyroch rôznych modelov:</span><span class="sxs-lookup"><span data-stu-id="13e32-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="13e32-107">Func_ssn nájde SSNs pred-2011 výrazné formátovanie, ktoré sú formátované pomlčky alebo medzery (ddd-dd-dddd alebo ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="13e32-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="13e32-108">Func_unformatted_ssn nájde SSNs pred-2011 silné formátovania, ktoré sú naformátovaná ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="13e32-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="13e32-109">Func_randomized_formatted_ssn nájde SSNs roku 2011, ktoré sú formátované pomlčky alebo medzery (ddd-dd-dddd alebo ddd dd dddd)</span><span class="sxs-lookup"><span data-stu-id="13e32-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="13e32-110">Func_randomized_unformatted_ssn nájde SSNs roku 2011, ktorá je naformátovaná ako deväť po sebe idúcich číslic (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="13e32-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="13e32-111">**[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nie, neexistuje žiadny kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="13e32-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="13e32-112">**[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politiky je 85% presvedčení, že to zistil citlivé informácie tohto typu, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="13e32-112">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="13e32-113">[Funkcia Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) nájde obsah, ktorý zodpovedá vzoru.</span><span class="sxs-lookup"><span data-stu-id="13e32-113">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="13e32-114">Nájsť slovo od [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) .</span><span class="sxs-lookup"><span data-stu-id="13e32-114">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="13e32-115">Obsahuje príklady kľúčových slov: *sociálne zabezpečenie, sociálne zabezpečenie #, Soc Sec, SSN* .</span><span class="sxs-lookup"><span data-stu-id="13e32-115">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="13e32-116">Napríklad nasledujúca ukážka by vyvolať DLP SSN politiky: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="13e32-116">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="13e32-117">Pre viac informácií o čo je potrebné pre SSNs majú byť zistené pre svoj obsah, nájdete v nasledujúcej časti v tomto článku: [Čo citlivé druhy informácií pozrite sa na SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="13e32-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="13e32-118">Pomocou rôznych vstavaných citlivé informácie typu, pozri nasledujúci článok informácie na čo je potrebné pre iné typy: [čo citlivé druhy informácií pozrite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="13e32-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  


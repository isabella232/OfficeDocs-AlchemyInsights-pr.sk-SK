---
title: DLP pravidlo číslo kreditnej karty nefunguje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919095"
---
<span data-ttu-id="3bd63-p101">Máte problémy s **Data Loss Prevention (DLP)** nefunguje pre obsah obsahujúcich **Čísla kreditnej karty** pri použití typu DLP citlivých informácií v služby O365? Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie pre spustenie DLP politiky, keď sa vyhodnotí. Napríklad pre **kreditnú kartu politiky** nakonfigurované s 85% úrovni spoľahlivosti, takto hodnotia a musí zistiť pravidlo spustiť:</span><span class="sxs-lookup"><span data-stu-id="3bd63-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="3bd63-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 číslic, ktoré môže byť formátovaný alebo neformátovaný (dddddddddddddddd) a musí vyhovieť skúške Luhn.</span><span class="sxs-lookup"><span data-stu-id="3bd63-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="3bd63-106">**[Vzorka:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Veľmi komplexný a robustný vzor, ktorý detekuje karty od všetkých významných značiek po celom svete, vrátane Visa, Mastercard, Discover Card, JCB, American Express, darčekové poukážky a karty stravník.</span><span class="sxs-lookup"><span data-stu-id="3bd63-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="3bd63-107">**[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Áno, Luhn kontrolný</span><span class="sxs-lookup"><span data-stu-id="3bd63-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="3bd63-108">**[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politiky je 85% presvedčení, že to zistil citlivé informácie tohto typu, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="3bd63-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="3bd63-109">Funkcia Func_credit_card nájde obsah, ktorý zodpovedá vzoru.</span><span class="sxs-lookup"><span data-stu-id="3bd63-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="3bd63-110">Je splnená jedna z nasledujúcich možností:</span><span class="sxs-lookup"><span data-stu-id="3bd63-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="3bd63-111">Nájsť slovo od Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="3bd63-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="3bd63-112">Kľúčové slovo z Keyword_cc_name nájdených</span><span class="sxs-lookup"><span data-stu-id="3bd63-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="3bd63-113">Funkcia Func_expiration_date zistí dátum správny dátum formát.</span><span class="sxs-lookup"><span data-stu-id="3bd63-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="3bd63-114">Kontrolný prechádza</span><span class="sxs-lookup"><span data-stu-id="3bd63-114">The checksum passes</span></span>
    
    <span data-ttu-id="3bd63-115">Napríklad nasledujúca ukážka by spúšť pre DLP politika číslo kreditnej karty:</span><span class="sxs-lookup"><span data-stu-id="3bd63-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="3bd63-116">Víza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="3bd63-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="3bd63-117">Platnosť: 2/2009</span><span class="sxs-lookup"><span data-stu-id="3bd63-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="3bd63-118">Pre viac informácií o čo je nevyhnutné pre **Číslo kreditnej karty** je možné pre svoj obsah, nájdete v nasledujúcej časti v tomto článku: [Čo citlivé druhy informácií vyhľadajte kreditnú kartu #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="3bd63-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="3bd63-119">Pomocou rôznych vstavaných citlivé informácie typu, pozri nasledujúci článok informácie na čo je potrebné pre iné typy: [čo citlivé druhy informácií pozrite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="3bd63-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  


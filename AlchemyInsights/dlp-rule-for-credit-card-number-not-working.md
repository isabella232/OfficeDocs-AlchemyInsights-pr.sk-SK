---
title: DLP pravidlo pre číslo kreditnej karty nefunguje
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
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507421"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="82db8-102">DLP problémy s číslami kreditných kariet</span><span class="sxs-lookup"><span data-stu-id="82db8-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="82db8-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="82db8-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="82db8-104">**DLP problémy s číslami kreditných kariet**</span><span class="sxs-lookup"><span data-stu-id="82db8-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="82db8-105">Máte problémy s **funkciou Ochrana pred únikom údajov (DLP)** nefunguje pre obsah obsahujúci **číslo kreditnej karty** pri používaní typu citlivých informácií DLP v systéme O365?</span><span class="sxs-lookup"><span data-stu-id="82db8-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="82db8-106">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie na spustenie politiky DLP pri jej vyhodnocovaní.</span><span class="sxs-lookup"><span data-stu-id="82db8-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="82db8-107">Napríklad pre **politiku kreditnej karty** nakonfigurovaný s úrovňou spoľahlivosti 85%, sa vyhodnotia nasledovné a musí sa zistiť, aby pravidlo spúšťať:</span><span class="sxs-lookup"><span data-stu-id="82db8-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="82db8-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 číslic, ktoré môžu byť formátované alebo neformátované (dddddddddddddddddddd) a musia prejsť Luhnovou skúškou.</span><span class="sxs-lookup"><span data-stu-id="82db8-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="82db8-109">**[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Veľmi zložitý a robustný vzor, ktorý detekuje karty od všetkých hlavných značiek po celom svete, vrátane Visa, MasterCard, Discover Card, JCB, American Express, darčekových kariet a kariet stravníkov.</span><span class="sxs-lookup"><span data-stu-id="82db8-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="82db8-110">**[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Áno, kontrolný súčet Luhna.</span><span class="sxs-lookup"><span data-stu-id="82db8-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="82db8-111">**[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Politika DLP je 85% presvedčená, že sa zistil tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="82db8-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="82db8-112">Funkcia Func_credit_card nájde obsah, ktorý zodpovedá vzoru.</span><span class="sxs-lookup"><span data-stu-id="82db8-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="82db8-113">Jedna z nasledujúcich je splnená:</span><span class="sxs-lookup"><span data-stu-id="82db8-113">One of the following is true:</span></span>

  - <span data-ttu-id="82db8-114">Nájde sa kľúčové slovo od Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="82db8-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="82db8-115">Kľúčové slovo z Keyword_cc_name sa nachádza</span><span class="sxs-lookup"><span data-stu-id="82db8-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="82db8-116">Funkcia Func_expiration_date vyhľadá dátum v správnom formáte dátumu.</span><span class="sxs-lookup"><span data-stu-id="82db8-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="82db8-117">Kontrolný súčet prechádza</span><span class="sxs-lookup"><span data-stu-id="82db8-117">The checksum passes</span></span>

    <span data-ttu-id="82db8-118">Napríklad nasledujúca vzorka by sa spustiť pre DLP číslo kreditnej karty politiky:</span><span class="sxs-lookup"><span data-stu-id="82db8-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="82db8-119">Vízum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="82db8-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="82db8-120">Uplynie: 2/2009</span><span class="sxs-lookup"><span data-stu-id="82db8-120">Expires: 2/2009</span></span>

<span data-ttu-id="82db8-121">Ďalšie informácie o tom, čo je potrebné pre **číslo kreditnej karty,** ktoré majú byť zistené pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Čo citlivé informácie typy hľadať kreditnej karty #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="82db8-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="82db8-122">Pomocou iného vstavaného typu citlivých informácií nájdete v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Čo vyzerajú typy citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="82db8-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  
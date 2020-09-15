---
title: Pravidlo DLP pre číslo kreditnej karty nefunguje
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679456"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="84ae9-102">Problémy s DLP s číslami kreditných kariet</span><span class="sxs-lookup"><span data-stu-id="84ae9-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="84ae9-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="84ae9-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="84ae9-104">**Problémy s DLP s číslami kreditných kariet**</span><span class="sxs-lookup"><span data-stu-id="84ae9-104">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="84ae9-105">Vyskytli sa problémy s **prevenciou pred stratou údajov (DLP)** , ktorá nepracuje s obsahom, ktorý obsahuje **číslo kreditnej karty** , ak sa v službe O365 používa typ informácií s informáciami o DLP?</span><span class="sxs-lookup"><span data-stu-id="84ae9-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="84ae9-106">Ak áno, uistite sa, že obsah obsahuje potrebné informácie na spustenie politiky DLP, keď sa vyhodnotí.</span><span class="sxs-lookup"><span data-stu-id="84ae9-106">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="84ae9-107">Napríklad pre **politiku kreditnej karty** nakonfigurovanú s úrovňou spoľahlivosti 85% sa vyhodnotia a pre pravidlo sa musí zistiť, či sa má spustiť nasledovné:</span><span class="sxs-lookup"><span data-stu-id="84ae9-107">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="84ae9-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 číslic, ktoré môžu byť formátované alebo nenaformátované (dddddddddddddddd) a musia prejsť testom Luhn.</span><span class="sxs-lookup"><span data-stu-id="84ae9-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="84ae9-109">**[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Veľmi zložitý a robustný vzor, ktorý detekuje karty zo všetkých hlavných značiek na celom svete vrátane víz, kariet MasterCard, Discover Card, JCB, American Express, darčekových poukazov a stravníkov.</span><span class="sxs-lookup"><span data-stu-id="84ae9-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="84ae9-110">**[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Áno, kontrolný súčet Luhn</span><span class="sxs-lookup"><span data-stu-id="84ae9-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="84ae9-111">**[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Politika DLP je 85% presvedčená, že zistí tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="84ae9-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="84ae9-112">Funkcia Func_credit_card nájde obsah, ktorý zodpovedá vzoru.</span><span class="sxs-lookup"><span data-stu-id="84ae9-112">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="84ae9-113">Je splnená jedna z nasledujúcich možností:</span><span class="sxs-lookup"><span data-stu-id="84ae9-113">One of the following is true:</span></span>

  - <span data-ttu-id="84ae9-114">Nájde sa kľúčové slovo z Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="84ae9-114">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="84ae9-115">Našlo sa kľúčové slovo z Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="84ae9-115">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="84ae9-116">Funkcia Func_expiration_date nájde dátum v správnom formáte dátumu.</span><span class="sxs-lookup"><span data-stu-id="84ae9-116">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="84ae9-117">Kontrolný súčet prechádza</span><span class="sxs-lookup"><span data-stu-id="84ae9-117">The checksum passes</span></span>

    <span data-ttu-id="84ae9-118">Nasledujúci príklad by sa spustil pre politiku kreditnej karty DLP:</span><span class="sxs-lookup"><span data-stu-id="84ae9-118">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="84ae9-119">Vízum: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="84ae9-119">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="84ae9-120">Platnosť uplynie: 2/2009</span><span class="sxs-lookup"><span data-stu-id="84ae9-120">Expires: 2/2009</span></span>

<span data-ttu-id="84ae9-121">Ďalšie informácie o tom, čo sa vyžaduje pri zisťovaní **čísla kreditných kariet** pre váš obsah, nájdete v tejto časti tohto článku: informácie o tom, [ktoré typy citlivých informácií vyhľadávajú kreditnú kartu #](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="84ae9-121">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)</span></span>
  
<span data-ttu-id="84ae9-122">Ak používate iný vstavaný typ citlivých informácií, prečítajte si v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="84ae9-122">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  
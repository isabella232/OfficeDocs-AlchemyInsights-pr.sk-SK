---
title: Pravidlo DLP pre US/UK Passport číslo nefunguje
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679239"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="c9479-102">Problémy s číslami služby DLP – US/UK Passport</span><span class="sxs-lookup"><span data-stu-id="c9479-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="c9479-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="c9479-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="c9479-104">**Problémy s DLP s číslami o pasoch v USA a Spojenom kráľovstve**</span><span class="sxs-lookup"><span data-stu-id="c9479-104">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="c9479-105">Vyskytli sa problémy s **prevenciou pred stratou údajov (DLP)** , ktorá nepracuje s obsahom, ktorý obsahuje **číslo cestovného pasu USA/UK** pri použití údajového typu DLP s citlivými informáciami v službe O365?</span><span class="sxs-lookup"><span data-stu-id="c9479-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c9479-106">Ak áno, uistite sa, že obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá, keď je vyhodnotená.</span><span class="sxs-lookup"><span data-stu-id="c9479-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="c9479-107">Napríklad pre politiku **číslo Passport USA/UK** nakonfigurovanú s úrovňou spoľahlivosti 75% sa vyhodnotia a pre pravidlo sa musí zistiť, či sa má spustiť</span><span class="sxs-lookup"><span data-stu-id="c9479-107">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="c9479-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Deväť číslic</span><span class="sxs-lookup"><span data-stu-id="c9479-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Nine digits</span></span>

- <span data-ttu-id="c9479-109">**[Vzor:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Deväť po sebe idúcich číslic</span><span class="sxs-lookup"><span data-stu-id="c9479-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="c9479-110">**[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, kontrolný súčet nie je k dispozícii</span><span class="sxs-lookup"><span data-stu-id="c9479-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="c9479-111">**[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Politika DLP je 75% presvedčená, že zistí tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="c9479-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c9479-112">Funkcia Func_usa_uk_passport nájde obsah, ktorý zodpovedá vzoru.</span><span class="sxs-lookup"><span data-stu-id="c9479-112">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c9479-113">Nájde sa kľúčové slovo z Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="c9479-113">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="c9479-114">Nasledujúca vzorka by napríklad spustila politiku **Passport pre USA a Veľkú Britániu** : US passport Number 123456789</span><span class="sxs-lookup"><span data-stu-id="c9479-114">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="c9479-115">Ďalšie informácie o tom, čo sa vyžaduje pre číslo pasu USA/UK, ktoré sa má zistiť pre váš obsah, nájdete v nasledujúcej časti tohto článku: [Aké typy citlivých informácií vyhľadávajú číslo cestovného pasu pre USA alebo UK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number) .</span><span class="sxs-lookup"><span data-stu-id="c9479-115">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)</span></span>
  
<span data-ttu-id="c9479-116">Ak používate iný vstavaný typ citlivých informácií, prečítajte si v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="c9479-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  
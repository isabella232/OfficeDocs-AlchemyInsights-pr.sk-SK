---
title: Pravidlo DLP pre číslo bankového účtu USA nefunguje
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679311"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="7f31c-102">Problémy s DLP s číslami bankových kont USA</span><span class="sxs-lookup"><span data-stu-id="7f31c-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="7f31c-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="7f31c-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="7f31c-104">**Problémy s DLP s číslami bankových kont USA**</span><span class="sxs-lookup"><span data-stu-id="7f31c-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="7f31c-105">Vyskytli sa problémy s **prevenciou pred stratou údajov (DLP)** , ktorá nepracuje s obsahom, ktorý obsahuje **číslo bankového účtu USA** pri použití údajového typu DLP s citlivými informáciami v službe O365?</span><span class="sxs-lookup"><span data-stu-id="7f31c-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="7f31c-106">Ak áno, uistite sa, že obsah obsahuje potrebné informácie o tom, čo politika DLP hľadá, keď je vyhodnotená.</span><span class="sxs-lookup"><span data-stu-id="7f31c-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="7f31c-107">Napríklad pre politiku **číslo bankového účtu USA** nakonfigurovanú s úrovňou spoľahlivosti 85% sa vyhodnotia a pre pravidlo sa musí zistiť, či sa má spustiť:</span><span class="sxs-lookup"><span data-stu-id="7f31c-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="7f31c-108">**[Formát:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 číslic</span><span class="sxs-lookup"><span data-stu-id="7f31c-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="7f31c-109">**[Vzorka:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 po sebe idúcich číslic.</span><span class="sxs-lookup"><span data-stu-id="7f31c-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="7f31c-110">**[Kontrolný súčet:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nie, kontrolný súčet nie je k dispozícii</span><span class="sxs-lookup"><span data-stu-id="7f31c-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="7f31c-111">**[Definícia:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Politika DLP je 75% presvedčená, že zistí tento typ citlivých informácií, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="7f31c-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="7f31c-112">Regulárny výraz Regex_usa_bank_account_number nájde obsah, ktorý zodpovedá vzoru</span><span class="sxs-lookup"><span data-stu-id="7f31c-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="7f31c-113">Nájde sa kľúčové slovo z Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="7f31c-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="7f31c-114">Pre politiku **bankového konta USA** by sa napríklad spustila nasledujúca vzorka: kontrola konta 78344011</span><span class="sxs-lookup"><span data-stu-id="7f31c-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="7f31c-115">Ďalšie informácie o tom, čo sa vyžaduje pri zisťovaní **čísla bankového konta v USA** , nájdete v nasledujúcej časti tohto článku: [Aké typy citlivých informácií vyhľadávajú číslo bankového účtu USA](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number) .</span><span class="sxs-lookup"><span data-stu-id="7f31c-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="7f31c-116">Ak používate iný vstavaný typ citlivých informácií, prečítajte si v nasledujúcom článku informácie o tom, čo sa vyžaduje pre iné typy: [Aké typy citlivých informácií hľadajú](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="7f31c-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  
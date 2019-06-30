---
title: DLP pravidlo pre nás bankový účet číslo nefunguje
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 83050b05cffacd3e81d34f05383c213eb0042fae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389484"
---
<span data-ttu-id="72fbc-102">Máte problémy s **Data Loss Prevention (DLP)** nefunguje pre obsah obsahujúce **Číslo bankového účtu v USA** pri použití typu DLP citlivých informácií v služby O365?</span><span class="sxs-lookup"><span data-stu-id="72fbc-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="72fbc-103">Ak áno, uistite sa, že váš obsah obsahuje potrebné informácie pre čo DLP politiky hľadá, keď sa vyhodnotí.</span><span class="sxs-lookup"><span data-stu-id="72fbc-103">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="72fbc-104">Napríklad, **Číslo bankového účtu v USA** politika nakonfigurovaná s 85% úrovni spoľahlivosti, takto hodnotia a musí zistiť pravidlo spustiť:</span><span class="sxs-lookup"><span data-stu-id="72fbc-104">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="72fbc-105">**[Formát:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 číslic</span><span class="sxs-lookup"><span data-stu-id="72fbc-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="72fbc-106">**[Vzorka:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 číslic.</span><span class="sxs-lookup"><span data-stu-id="72fbc-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="72fbc-107">**[Kontrolný súčet:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nie, neexistuje žiadny kontrolný súčet</span><span class="sxs-lookup"><span data-stu-id="72fbc-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="72fbc-108">**[Definícia:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politiky je 75% presvedčení, že to zistil citlivé informácie tohto typu, ak v blízkosti 300 znakov:</span><span class="sxs-lookup"><span data-stu-id="72fbc-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="72fbc-109">Regulárny výraz Regex_usa_bank_account_number nájde obsah, ktorý zodpovedá vzoru</span><span class="sxs-lookup"><span data-stu-id="72fbc-109">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="72fbc-110">Nájsť slovo od Keyword_usa_Bank_Account.</span><span class="sxs-lookup"><span data-stu-id="72fbc-110">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="72fbc-111">Napríklad nasledujúca ukážka by spúšť pre politiky **USA číslo bankového účtu** : bežný účet 78344011</span><span class="sxs-lookup"><span data-stu-id="72fbc-111">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="72fbc-112">Pre viac informácií o čo je potrebné **Číslo bankového účtu v USA** sa vyhľadávajú pre svoj obsah, nájdete v nasledujúcej časti v tomto článku: [Čo citlivé druhy informácií pozrite sa na číslo bankového účtu v USA](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="72fbc-112">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)</span></span>
  
<span data-ttu-id="72fbc-113">Pomocou rôznych vstavaných citlivé informácie typu, pozri nasledujúci článok informácie na čo je potrebné pre iné typy: [čo citlivé druhy informácií pozrite](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="72fbc-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  
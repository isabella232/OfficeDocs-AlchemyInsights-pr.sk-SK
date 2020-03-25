---
title: DLP môže potrebovať vlastný typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932673"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="6d0df-102">DLP môže potrebovať vlastný typ</span><span class="sxs-lookup"><span data-stu-id="6d0df-102">DLP might need a custom type</span></span>

<span data-ttu-id="6d0df-103">**Dôležité**: mnoho zákazníkov SharePoint Online a OneDrive spúšťať kritické aplikácie proti služby, ktoré sa spúšťajú na pozadí.</span><span class="sxs-lookup"><span data-stu-id="6d0df-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="6d0df-104">Patria sem migrácia obsahu, ochrana pred únikom údajov (DLP) a riešenia zálohovania.</span><span class="sxs-lookup"><span data-stu-id="6d0df-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="6d0df-105">Počas týchto bezprecedentných časoch, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné a spoľahlivé pre používateľov, ktorí závisia od služby viac ako inokedy v situáciách vzdialenej práce.</span><span class="sxs-lookup"><span data-stu-id="6d0df-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="6d0df-106">Na podporu tohto cieľa sme implementovali prísnejšie obmedzenia pre aplikácie na pozadí (migrácia, DLP a záložné riešenia) počas denných hodín pracovného dňa.</span><span class="sxs-lookup"><span data-stu-id="6d0df-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="6d0df-107">Mali by ste očakávať, že tieto aplikácie dosiahnu veľmi obmedzenú priepustnosť v týchto časoch.</span><span class="sxs-lookup"><span data-stu-id="6d0df-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="6d0df-108">Avšak, počas večera a víkendové hodiny pre región, bude služba pripravená spracovať výrazne vyšší objem žiadostí z aplikácií na pozadí.</span><span class="sxs-lookup"><span data-stu-id="6d0df-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="6d0df-109">**DLP môže vyžadovať typ vlastného informácie**</span><span class="sxs-lookup"><span data-stu-id="6d0df-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="6d0df-110">Pomocou politiky ochrany pred únikom údajov (DLP) môžete identifikovať a chrániť citlivé údaje vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="6d0df-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="6d0df-111">V niektorých prípadoch môže byť potrebné **vytvoriť vlastný typ citlivých informácií** na ochranu údajov organizácie.</span><span class="sxs-lookup"><span data-stu-id="6d0df-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="6d0df-112">Vaša organizácia môže napríklad potrebovať identifikovať a chrániť identifikátory zamestnancov alebo iné údaje v určitom formáte špecifickom pre vašu organizáciu. Ak áno, pozrite si nasledujúce články pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="6d0df-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="6d0df-113">**Prispôsobenie vstavaného typu citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="6d0df-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="6d0df-114">Ak by vstavaný typ citlivých informácií spĺňal vaše potreby len s niekoľkými vylepšeniami, môžete [prispôsobiť vstavaný typ citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="6d0df-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="6d0df-115">Môžete napríklad pridať alebo odstrániť kľúčové slová alebo pridať alebo odstrániť podporné dôkazy, ako je napríklad dátum alebo adresa.</span><span class="sxs-lookup"><span data-stu-id="6d0df-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="6d0df-116">**Vytvorenie vlastného typu citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="6d0df-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="6d0df-117">Ak však potrebujete úplne identifikovať a ochrániť iný typ citlivých informácií, môžete [vytvoriť vlastný typ citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) v používateľskom rozhraní centra zabezpečenia & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="6d0df-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="6d0df-118">**Vytvoriť vlastné citlivé informácie typu zabezpečenia & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="6d0df-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="6d0df-119">Nakoniec, ak UI neposkytuje všetky možnosti, ktoré potrebujete, môžete [vytvoriť vlastné citlivé informácie typu zabezpečenia & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="6d0df-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="6d0df-120">Spustením súboru XML môžete použiť každú dostupnú možnosť.</span><span class="sxs-lookup"><span data-stu-id="6d0df-120">By starting with an XML file, you can use every option available.</span></span>

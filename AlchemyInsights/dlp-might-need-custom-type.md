---
title: DLP môže potrebovať vlastný typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712199"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="07ca8-102">DLP môže potrebovať vlastný typ</span><span class="sxs-lookup"><span data-stu-id="07ca8-102">DLP might need a custom type</span></span>

<span data-ttu-id="07ca8-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="07ca8-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="07ca8-104">**DLP môže vyžadovať vlastný typ informácií**</span><span class="sxs-lookup"><span data-stu-id="07ca8-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="07ca8-105">Pomocou politiky ochrany pred únikom údajov (DLP) môžete identifikovať a chrániť citlivé údaje vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="07ca8-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="07ca8-106">V niektorých prípadoch možno budete musieť **vytvoriť vlastný typ citlivých** informácií na ochranu údajov vašej organizácie.</span><span class="sxs-lookup"><span data-stu-id="07ca8-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="07ca8-107">Vaša organizácia môže napríklad potrebovať identifikovať a chrániť identifikácie zamestnancov alebo iné údaje v určitom formáte, ktorý je špecifický pre vašu organizáciu. Ak áno, ďalšie informácie nájdete v nasledujúcich článkoch.</span><span class="sxs-lookup"><span data-stu-id="07ca8-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="07ca8-108">**Prispôsobenie typu vstavaných citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="07ca8-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="07ca8-109">Ak vstavaný typ citlivých informácií vyhovuje vašim potrebám len pomocou niekoľkých vylepšení, môžete [prispôsobiť vstavaný typ informácií](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="07ca8-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="07ca8-110">Môžete napríklad pridať alebo odstrániť kľúčové slová alebo pridať alebo odstrániť podporné dôkazy, ako je napríklad dátum alebo adresa.</span><span class="sxs-lookup"><span data-stu-id="07ca8-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="07ca8-111">**Vytvorenie vlastného typu citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="07ca8-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="07ca8-112">Ak však potrebujete úplne identifikovať a chrániť iný typ citlivých informácií, môžete [vytvoriť vlastný typ citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) v používateľskom rozhraní centra zabezpečenia & dodržiavania súladu.</span><span class="sxs-lookup"><span data-stu-id="07ca8-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="07ca8-113">**Vytvorenie vlastného typu citlivých informácií v prostredí zabezpečenia & prostredie na zabezpečenie súladu**</span><span class="sxs-lookup"><span data-stu-id="07ca8-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="07ca8-114">A nakoniec, ak používateľské rozhranie neposkytuje všetky potrebné možnosti, môžete [vytvoriť vlastný typ citlivých informácií v prostredí zabezpečenia & v centre súladu](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="07ca8-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="07ca8-115">Spustením súboru XML môžete použiť všetky dostupné možnosti.</span><span class="sxs-lookup"><span data-stu-id="07ca8-115">By starting with an XML file, you can use every option available.</span></span>

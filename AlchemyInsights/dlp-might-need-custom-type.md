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
ms.openlocfilehash: 87fcb5c3cc9ccd525265097b66d9d9b3a85c5feb
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977285"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="344d1-102">DLP môže potrebovať vlastný typ</span><span class="sxs-lookup"><span data-stu-id="344d1-102">DLP might need a custom type</span></span>

<span data-ttu-id="344d1-103">**Dôležité**: počas týchto nebývalé časy, robíme kroky, aby zabezpečili, že SharePoint Online a OneDrive služby zostávajú vysoko dostupné-navštívte [SharePoint Online dočasné funkcie úpravy](https://aka.ms/ODSPAdjustments) pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="344d1-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="344d1-104">**DLP môže vyžadovať typ vlastného informácie**</span><span class="sxs-lookup"><span data-stu-id="344d1-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="344d1-105">Pomocou politiky ochrany pred únikom údajov (DLP) môžete identifikovať a chrániť citlivé údaje vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="344d1-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="344d1-106">V niektorých prípadoch môže byť potrebné **vytvoriť vlastný typ citlivých informácií** na ochranu údajov organizácie.</span><span class="sxs-lookup"><span data-stu-id="344d1-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="344d1-107">Vaša organizácia môže napríklad potrebovať identifikovať a chrániť identifikátory zamestnancov alebo iné údaje v určitom formáte špecifickom pre vašu organizáciu. Ak áno, pozrite si nasledujúce články pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="344d1-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="344d1-108">**Prispôsobenie vstavaného typu citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="344d1-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="344d1-109">Ak by vstavaný typ citlivých informácií spĺňal vaše potreby len s niekoľkými vylepšeniami, môžete [prispôsobiť vstavaný typ citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="344d1-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="344d1-110">Môžete napríklad pridať alebo odstrániť kľúčové slová alebo pridať alebo odstrániť podporné dôkazy, ako je napríklad dátum alebo adresa.</span><span class="sxs-lookup"><span data-stu-id="344d1-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="344d1-111">**Vytvorenie vlastného typu citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="344d1-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="344d1-112">Ak však potrebujete úplne identifikovať a ochrániť iný typ citlivých informácií, môžete [vytvoriť vlastný typ citlivých informácií](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) v používateľskom rozhraní centra zabezpečenia & Compliance Center.</span><span class="sxs-lookup"><span data-stu-id="344d1-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="344d1-113">**Vytvoriť vlastné citlivé informácie typu zabezpečenia & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="344d1-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="344d1-114">Nakoniec, ak UI neposkytuje všetky možnosti, ktoré potrebujete, môžete [vytvoriť vlastné citlivé informácie typu zabezpečenia & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="344d1-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="344d1-115">Spustením súboru XML môžete použiť každú dostupnú možnosť.</span><span class="sxs-lookup"><span data-stu-id="344d1-115">By starting with an XML file, you can use every option available.</span></span>

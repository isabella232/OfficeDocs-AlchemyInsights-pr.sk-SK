---
title: DLP môže potrebovať vlastný typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507529"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="8117d-102">DLP môže potrebovať vlastný typ</span><span class="sxs-lookup"><span data-stu-id="8117d-102">DLP might need a custom type</span></span>

<span data-ttu-id="8117d-103">**Dôležité**: V tejto výnimočnej situácií vykonávame kroky na to, aby sme zabezpečili, že služby SharePoint Online a OneDrive zostanú vysoko dostupné. Ďalšie informácie nájdete v téme [Dočasné úpravy funkcií SharePointu Online](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="8117d-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="8117d-104">**DLP môže vyžadovať vlastný typ informácií**</span><span class="sxs-lookup"><span data-stu-id="8117d-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="8117d-105">Pomocou politiky ochrany pred únikom údajov (DLP) môžete identifikovať a chrániť citlivé údaje vo vašej organizácii.</span><span class="sxs-lookup"><span data-stu-id="8117d-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="8117d-106">V niektorých prípadoch môže byť potrebné vytvoriť vlastný typ **citlivých** informácií na ochranu údajov organizácie.</span><span class="sxs-lookup"><span data-stu-id="8117d-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="8117d-107">Vaša organizácia môže napríklad potrebovať identifikovať a chrániť identifikácie zamestnancov alebo iné údaje v nejakom formáte špecifickom pre vašu organizáciu. Ak áno, nájdete v nasledujúcich článkoch pre viac informácií.</span><span class="sxs-lookup"><span data-stu-id="8117d-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="8117d-108">**Prispôsobenie vstavaného typu citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="8117d-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="8117d-109">Ak by vstavaný typ citlivých informácií vyhovoval vašim potrebám len niekoľkými vylepšeniami, môžete [prispôsobiť vstavaný typ citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="8117d-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="8117d-110">Môžete napríklad pridať alebo odstrániť kľúčové slová alebo pridať alebo odstrániť podporné dôkazy, ako je dátum alebo adresa.</span><span class="sxs-lookup"><span data-stu-id="8117d-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="8117d-111">**Vytvorenie vlastného typu citlivých informácií**</span><span class="sxs-lookup"><span data-stu-id="8117d-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="8117d-112">Ak však potrebujete úplne identifikovať a chrániť iný typ citlivých informácií, môžete [vytvoriť vlastný typ citlivých informácií](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) v ui centra zabezpečenia & súladu.</span><span class="sxs-lookup"><span data-stu-id="8117d-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="8117d-113">**Vytvorenie vlastného typu citlivých informácií v prostredí PowerShell & Centrum zabezpečenia**</span><span class="sxs-lookup"><span data-stu-id="8117d-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="8117d-114">Nakoniec, ak ui neposkytuje všetky potrebné možnosti, môžete [vytvoriť vlastný typ citlivých informácií v prostredí PowerShell security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="8117d-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="8117d-115">Spustením súboru XML môžete použiť každú dostupnú možnosť.</span><span class="sxs-lookup"><span data-stu-id="8117d-115">By starting with an XML file, you can use every option available.</span></span>

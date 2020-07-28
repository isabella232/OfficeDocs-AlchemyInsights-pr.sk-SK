---
title: Intune inventár zariadenia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440476"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="7abc9-102">Intune inventár zariadenia</span><span class="sxs-lookup"><span data-stu-id="7abc9-102">Intune Device Inventory</span></span>

<span data-ttu-id="7abc9-103">Čepeľ Zariadenia poskytuje správcovi prehľad o zariadeniach, ktoré sú pod správou v intune na základe zariadenia.</span><span class="sxs-lookup"><span data-stu-id="7abc9-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="7abc9-104">Zobrazené informácie zahŕňajú: Hardvér, Objavené aplikácie, Stav súladu zariadenia a Stav konfigurácie zariadenia.</span><span class="sxs-lookup"><span data-stu-id="7abc9-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="7abc9-105">Údaje o zásobách pre hardvér a objavené aplikácie sa zhromažďujú v sedemdňovom cykle.</span><span class="sxs-lookup"><span data-stu-id="7abc9-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="7abc9-106">Aplikácie a konkrétne prvky nahláseného hardvéru sa líšia v závislosti od operačného systému zariadenia a od toho, či je zariadenie osobne alebo vo vlastníctve podniku.</span><span class="sxs-lookup"><span data-stu-id="7abc9-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="7abc9-107">Ďalšie informácie nájdete v téme Zobrazenie [podrobností o zariadení v programe Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="7abc9-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="7abc9-108">**Najčastejšie otázky**</span><span class="sxs-lookup"><span data-stu-id="7abc9-108">**FAQ**</span></span>

<span data-ttu-id="7abc9-109">Otázka: Nedostávam úplný zoznam aplikácií prítomných v zariadeniach s Windowsom zaregistrované v intune.</span><span class="sxs-lookup"><span data-stu-id="7abc9-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="7abc9-110">prečo nie?</span><span class="sxs-lookup"><span data-stu-id="7abc9-110">Why not?</span></span>

<span data-ttu-id="7abc9-111">A: V tomto čase sú pre počítače s Windowsom 10, ktoré sú identifikované ako podnikové zariadenia, sú v zozname iba moderné aplikácie.</span><span class="sxs-lookup"><span data-stu-id="7abc9-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="7abc9-112">Intune nezhromažďuje informácie o aplikáciách Win32 nainštalovaných v týchto zariadeniach.</span><span class="sxs-lookup"><span data-stu-id="7abc9-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="7abc9-113">Otázka: Prečo sa telefónne čísla nezhromažďujú zo všetkých zariadení?</span><span class="sxs-lookup"><span data-stu-id="7abc9-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="7abc9-114">A: Telefóny kategorizované ako podnikové zariadenia v programe Intune nie sú identifikované s celým telefónnym číslom, keď napríklad spustíte správu o inventári mobilného zariadenia.</span><span class="sxs-lookup"><span data-stu-id="7abc9-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="7abc9-115">Telefónne čísla na vlastné zariadenia sú vždy čiastočne zamaskované hviezdičkami (\*\*\*\*) a zobrazujú len posledné štyri číslice.</span><span class="sxs-lookup"><span data-stu-id="7abc9-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>
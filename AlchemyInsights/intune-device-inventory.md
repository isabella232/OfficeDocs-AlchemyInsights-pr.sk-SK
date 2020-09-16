---
title: Inventár zariadenia služby Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667893"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="cd486-102">Inventár zariadenia služby Intune</span><span class="sxs-lookup"><span data-stu-id="cd486-102">Intune Device Inventory</span></span>

<span data-ttu-id="cd486-103">Blade zariadenia poskytuje správcovi prehľad o zariadeniach v rámci správy v službe Intune na základe jednotlivých zariadení.</span><span class="sxs-lookup"><span data-stu-id="cd486-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="cd486-104">Zobrazené informácie zahŕňajú: hardvér, nájdené aplikácie, stav súladu zariadenia a stav konfigurácie zariadenia.</span><span class="sxs-lookup"><span data-stu-id="cd486-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="cd486-105">Údaje o zásobách pre hardvér a nájdené aplikácie sa zhromažďujú v priebehu siedmich dní cyklu.</span><span class="sxs-lookup"><span data-stu-id="cd486-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="cd486-106">Nahlásené aplikácie a špecifické prvky hardvéru sa líšia v závislosti od operačného systému zariadenia a od toho, či je zariadenie osobne alebo podnikovo vlastnené.</span><span class="sxs-lookup"><span data-stu-id="cd486-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="cd486-107">Ďalšie informácie nájdete v téme [Zobrazenie podrobností o zariadení v službe Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="cd486-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="cd486-108">**Najčastejšie otázky**</span><span class="sxs-lookup"><span data-stu-id="cd486-108">**FAQ**</span></span>

<span data-ttu-id="cd486-109">Otázka: Neprijímam úplný zoznam aplikácií, ktoré sú prítomné v zariadeniach s Windowsom Intune.</span><span class="sxs-lookup"><span data-stu-id="cd486-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="cd486-110">prečo nie?</span><span class="sxs-lookup"><span data-stu-id="cd486-110">Why not?</span></span>

<span data-ttu-id="cd486-111">A: v súčasnosti sú na počítačoch s Windowsom 10, ktoré sú identifikované ako podnikové zariadenia, uvedené len moderné aplikácie.</span><span class="sxs-lookup"><span data-stu-id="cd486-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="cd486-112">Intune nezhromažďuje informácie o aplikáciách Win32 nainštalovaných v týchto zariadeniach.</span><span class="sxs-lookup"><span data-stu-id="cd486-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="cd486-113">Otázka: prečo sa nezhromažďujú telefónne čísla zo všetkých zariadení?</span><span class="sxs-lookup"><span data-stu-id="cd486-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="cd486-114">A: telefóny kategorizované ako podnikové zariadenia v službe Intune nie sú identifikované s úplným telefónnym číslom, napríklad keď spustíte zostavu inventára mobilného zariadenia.</span><span class="sxs-lookup"><span data-stu-id="cd486-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="cd486-115">Telefónne čísla s prihlásením do vlastných zariadení sú vždy čiastočne zamaskované hviezdičkou (\* \* \* \*) a zobrazia sa iba posledné štyri číslice.</span><span class="sxs-lookup"><span data-stu-id="cd486-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>
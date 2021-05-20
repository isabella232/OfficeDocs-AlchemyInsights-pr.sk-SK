---
title: Problémy s odstránením vyradeného alebo vyradeného zariadenia z inventára zariadení
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564608"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="8bc36-102">Problémy s odstránením vyradeného alebo vyradeného zariadenia z inventára zariadení</span><span class="sxs-lookup"><span data-stu-id="8bc36-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="8bc36-103">Microsoft Defender pre koncový bod momentálne neumožňuje manuálne odstránenie záznamu zariadenia pre vyradeného alebo vyradeného zariadenia z inventára zariadení.</span><span class="sxs-lookup"><span data-stu-id="8bc36-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="8bc36-104">Z bezpečnostných dôvodov zostane zariadenie na portáli ako historický záznam do 180 dní.</span><span class="sxs-lookup"><span data-stu-id="8bc36-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="8bc36-105">Údaje zariadenia sa však vymaka v súlade s nakonfigurovaným obdobím uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="8bc36-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="8bc36-106">**Poznámka:** Vypnuté alebo vyradené zariadenie sa po siedmich dňoch **automaticky prepne do** stavu Neaktívne.</span><span class="sxs-lookup"><span data-stu-id="8bc36-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="8bc36-107">Okrem toho zariadenia, ktoré nie sú aktívne za posledných 30 dní, sa neza faktoria v údajoch, ktoré odrážajú údaje vašej organizácie Spravovanie hrozieb a rizík alebo výsledky zabezpečenia spoločnosti Microsoft pre zariadenia.</span><span class="sxs-lookup"><span data-stu-id="8bc36-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="8bc36-108">Ak nechcete zobraziť niektoré zariadenia v zobrazení Inventár zariadení, skúste umiestnenie značky zariadenia vyfiltrovať zariadenie vyradené zo zobrazenia Inventár zariadenia.</span><span class="sxs-lookup"><span data-stu-id="8bc36-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="8bc36-109">Ďalšie informácie nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="8bc36-109">For more information, see:</span></span>

[<span data-ttu-id="8bc36-110">Zariadenia s vypnutou mapou zo služby Microsoft Defender pre koncový bod</span><span class="sxs-lookup"><span data-stu-id="8bc36-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="8bc36-111">Skóre expozície v Spravovanie hrozieb a rizík</span><span class="sxs-lookup"><span data-stu-id="8bc36-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="8bc36-112">Oprava nevhodných senzorov v aplikácii Microsoft Defender pre koncový bod</span><span class="sxs-lookup"><span data-stu-id="8bc36-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="8bc36-113">Efektívne používanie označovania (časť 1)</span><span class="sxs-lookup"><span data-stu-id="8bc36-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="8bc36-114">Efektívne používanie označovania (časť 2)</span><span class="sxs-lookup"><span data-stu-id="8bc36-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="8bc36-115">Efektívne používanie označovania (časť 3)</span><span class="sxs-lookup"><span data-stu-id="8bc36-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)





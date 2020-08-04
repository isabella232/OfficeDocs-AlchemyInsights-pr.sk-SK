---
title: Automatické čistenie zastaraných zariadení v intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555733"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="fbaa1-102">Automatické čistenie zastaraných zariadení v intune</span><span class="sxs-lookup"><span data-stu-id="fbaa1-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="fbaa1-103">Intune umožňuje správcovi nakonfigurovať časový interval medzi 90 a 270 dňami, po ktorom sa zo služby odstránia zastarané zariadenia.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="fbaa1-104">Toto nastavenie je organizácia široká a po aktivácii nadobúda účinnosť okamžite.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="fbaa1-105">Všetky zariadenia, ktoré nie sú kontrolované na serveri Intune po dobu presahujúcu nastavenie sa natrvalo odstránia.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="fbaa1-106">**Upozornenie:** Iba objekty zariadenia MDM sú vhodné pre túto akciu čistenia.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="fbaa1-107">EAS iba objekty zariadenia sú vylúčené.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="fbaa1-108">Ďalšie informácie o tom, kedy sa zariadenie stane spôsobilým na vymazanie na základe nastavenia zariadenia na čistenie a jeho "stavu":</span><span class="sxs-lookup"><span data-stu-id="fbaa1-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="fbaa1-109">Nastavenie: **Odstrániť zariadenia po dátume poslednej registrácie: Áno (niektoré hodnoty (N) v zadaných dňoch)**</span><span class="sxs-lookup"><span data-stu-id="fbaa1-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="fbaa1-110">Na základe hodnoty (N) nakonfigurovanej v nastavení služba Intune odstráni zariadenie v zadaných dňoch po tom, ako sa naposledy úspešne skontroluje.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="fbaa1-111">Nastavenie: **Odstrániť zariadenia po poslednej registrácii dátum: Nie**</span><span class="sxs-lookup"><span data-stu-id="fbaa1-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="fbaa1-112">180 dní po vypršaní platnosti certifikátu zariadenia a neobnoví sa, zariadenie sa odstráni.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="fbaa1-113">**Upozornenie:** V oboch prípadoch musí byť zariadenie úspešne zaregistrované v intune.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="fbaa1-114">Registrácia sa vyskytuje počas prvého zariadenia checkin so službou Intune.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="fbaa1-115">Ak sa zariadenie úspešne zaregistruje do intune, ale neregistruje sa intune, zariadenie sa odstráni 270 dní po registrácii.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="fbaa1-116">(90 dní na označenie zariadenia ako zrušené a ďalších 180 dní na odstránenie záznamu.)</span><span class="sxs-lookup"><span data-stu-id="fbaa1-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="fbaa1-117">V konzole Intune momentálne neexistuje mechanizmus na stanovenie dátumu uplynutia platnosti certifikácie zariadenia pre dané zariadenie.</span><span class="sxs-lookup"><span data-stu-id="fbaa1-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>
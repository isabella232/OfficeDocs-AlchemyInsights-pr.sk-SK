---
title: V Centre zabezpečenia sa nenašli žiadne správy o predplatných
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544123"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="8e623-102">V Centre zabezpečenia sa nenašli žiadne správy o predplatných</span><span class="sxs-lookup"><span data-stu-id="8e623-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="8e623-103">Ak sa počas prístupu k Centrum zabezpečenia v programe Microsoft Defender zobrazí hlásenie Nenašli sa žiadne predplatné, znamená to, že Azure Active Directory (AAD) používaný na prihlásenie používateľa na portál nemá licenciu na Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="8e623-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="8e623-104">Licencie Windows E5 a Office E5 sú samostatné licencie.</span><span class="sxs-lookup"><span data-stu-id="8e623-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="8e623-105">Otvorte prípad podpory, ak bola licencia zakúpená, ale nie je ustavená v tejto inštancii služby AAD.</span><span class="sxs-lookup"><span data-stu-id="8e623-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="8e623-106">Či už máte:</span><span class="sxs-lookup"><span data-stu-id="8e623-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="8e623-107">Možný problém s poskytovaním licencií.</span><span class="sxs-lookup"><span data-stu-id="8e623-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="8e623-108">Neúmyselne ste licenciu zverejňujú inej službe Microsoft AAD ako ten, ktorý sa používa na overovanie do služby.</span><span class="sxs-lookup"><span data-stu-id="8e623-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>
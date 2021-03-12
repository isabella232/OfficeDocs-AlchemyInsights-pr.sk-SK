---
title: V centre zabezpečenia nie sú nájdené žiadne predplatné
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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713965"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="5472e-102">V centre zabezpečenia nie sú nájdené žiadne predplatné</span><span class="sxs-lookup"><span data-stu-id="5472e-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="5472e-103">Ak sa pri prístupe k centru zabezpečenia programu Microsoft Defender zobrazí hlásenie žiadne nájdené predplatné, znamená to, že v službe Azure Active Directory (AAD), ktorá sa používa na prihlásenie používateľa na portál, nie je k dispozícii licencia Microsoft Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="5472e-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="5472e-104">Licencie na Windows E5 a Office E5 sú samostatné licencie.</span><span class="sxs-lookup"><span data-stu-id="5472e-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="5472e-105">Otvorte prípad podpory, ak bola licencia zakúpená, ale nebola poskytnutá tejto inštancii AAD.</span><span class="sxs-lookup"><span data-stu-id="5472e-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="5472e-106">Buď máte:</span><span class="sxs-lookup"><span data-stu-id="5472e-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="5472e-107">Možný problém s poskytovaním licencií.</span><span class="sxs-lookup"><span data-stu-id="5472e-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="5472e-108">Ste neúmyselne ustanovili licenciu na inú spoločnosť Microsoft AAD, než je tá, ktorá sa použila na overenie do služby.</span><span class="sxs-lookup"><span data-stu-id="5472e-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>
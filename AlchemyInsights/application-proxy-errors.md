---
title: Riešenie chýb súvisiacich so serverom proxy aplikácie
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "9686"
ms.openlocfilehash: fe0bae35942af9925e8a5f90f966e204d7f84fd2
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/22/2021
ms.locfileid: "51038168"
---
# <a name="troubleshoot-errors-related-to-application-proxy"></a><span data-ttu-id="b5f5e-102">Riešenie chýb súvisiacich so serverom proxy aplikácie</span><span class="sxs-lookup"><span data-stu-id="b5f5e-102">Troubleshoot errors related to Application Proxy</span></span>

- <span data-ttu-id="b5f5e-103">Ďalšie informácie o častejších chybách, ktoré pochádzajú z nastavenia a konfigurácie modulu Kerberos, a návrhy na riešenie problémov nájdete v téme [Riešenie problémov s proxy aplikáciami a chybové hlásenia](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-troubleshoot#kerberos-errors).</span><span class="sxs-lookup"><span data-stu-id="b5f5e-103">To learn about the more common errors that come from Kerberos setup and configuration, and suggestions for resolution, see [Troubleshoot Application Proxy problems and error messages](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-troubleshoot#kerberos-errors).</span></span>
- <span data-ttu-id="b5f5e-104">Ak ide o chyby aplikácie proxy 404, pozrite si tému [stránka aplikácie sa nezobrazuje správne pre aplikáciu proxy aplikácie | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-page-appearance-broken-problem).</span><span class="sxs-lookup"><span data-stu-id="b5f5e-104">For App Proxy 404 errors, see [App page doesn't display correctly for Application Proxy app | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-page-appearance-broken-problem).</span></span>
- <span data-ttu-id="b5f5e-105">V službe Azure Active Directory (Azure AD) sa konfigurácia veľkého počtu lokálnych aplikácií môže rýchlo stať nezvládnuteľnou a predstavuje zbytočné riziko chýb konfigurácie, ak niektoré z nich vyžadujú rovnaké nastavenia.</span><span class="sxs-lookup"><span data-stu-id="b5f5e-105">In Azure Active Directory (Azure AD), configuring a large number of on-premises applications can quickly become unmanageable and introduces unnecessary risks for configuration errors if many of them require the same settings.</span></span> <span data-ttu-id="b5f5e-106">So [serverom proxy aplikácie Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy)môžete tento problém vyriešiť pomocou aplikácie na publikovanie zástupných znakov na publikovanie a spravovanie mnohých aplikácií naraz.</span><span class="sxs-lookup"><span data-stu-id="b5f5e-106">With [Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy), you can address this issue by using wildcard application publishing to publish and manage many applications at once.</span></span> <span data-ttu-id="b5f5e-107">Ďalšie informácie nájdete v téme [zástupné aplikácie v serveri proxy aplikácie Azure AD | Dokumenty Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard).</span><span class="sxs-lookup"><span data-stu-id="b5f5e-107">For more information, see [Wildcard applications in the Azure AD Application Proxy | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard).</span></span>

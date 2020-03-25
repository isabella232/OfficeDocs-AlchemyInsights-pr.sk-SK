---
title: Nie je možné prihlásiť sa do služby Teams z dôvodu chyby autologon.microsoftazuread-sso.com:443
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932290"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="7f9df-102">Nie je možné prihlásiť sa do služby Teams z dôvodu tejto autologon.microsoftazuread-sso dot com:443</span><span class="sxs-lookup"><span data-stu-id="7f9df-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="7f9df-103">Ak je v rámci overovania služby O365 zapnutá funkcia Seamless SSO, je možné, že je potrebné pridať URL adresu "autologon.microsoftazuread-sso.com" na intranetové lokality.</span><span class="sxs-lookup"><span data-stu-id="7f9df-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="7f9df-104">Ak sa už predtým pridala medzi dôveryhodné lokality a používa sa funkcia Seamless SSO, mala by sa odstrániť z dôveryhodných lokalít.</span><span class="sxs-lookup"><span data-stu-id="7f9df-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="7f9df-105">Prečítajte si [Kontrolný zoznam riešenia problémov s funkciou Seamless SSO](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="7f9df-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="7f9df-106">Ak chcete pridať URL adresu do zoznamu intranetových lokalít, postupujte podľa týchto krokov:</span><span class="sxs-lookup"><span data-stu-id="7f9df-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="7f9df-107">Otvorte Internet Explorer kliknutím na tlačidlo **Štart**</span><span class="sxs-lookup"><span data-stu-id="7f9df-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="7f9df-108">Do vyhľadávacieho poľa zadajte text Internet Explorer a potom v zozname výsledkov kliknite na položku **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="7f9df-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="7f9df-109">Kliknite na položku **Nástroje** a potom kliknite na možnosť **Možnosti siete internet**.</span><span class="sxs-lookup"><span data-stu-id="7f9df-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="7f9df-110">Kliknite na kartu **Zabezpečenie**.</span><span class="sxs-lookup"><span data-stu-id="7f9df-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="7f9df-111">Teraz kliknite na položku **Lokálne intranetové lokality** a potom kliknite na tlačidlo **lokalít** a potom na tlačidlo **Rozšírené**.</span><span class="sxs-lookup"><span data-stu-id="7f9df-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="7f9df-112">Zadajte URL adresu webovej lokality a kliknite na položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="7f9df-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="7f9df-113">Po dokončení nastavovania kliknite na tlačidlo **Zavrie5**.</span><span class="sxs-lookup"><span data-stu-id="7f9df-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="7f9df-114">Ďalšie informácie nájdete v téme [Dokumentácia pre nasadenie funkcie Seamless SSO pre službu O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (zahŕňa proces založený na zásadách na pridanie URL adresy na intranetové lokality v kroku 3).</span><span class="sxs-lookup"><span data-stu-id="7f9df-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>

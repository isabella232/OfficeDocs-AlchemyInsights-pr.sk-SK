---
title: Problémy pri prihlasovaní do aplikácií Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836618"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="8111f-102">Problémy s prihlásením do aplikácií Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="8111f-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="8111f-103">Ak chcete opraviť problémy s prihlásením v aplikáciách služby Microsoft 365, vyskúšajte v vplyvnení počítača tieto možnosti:</span><span class="sxs-lookup"><span data-stu-id="8111f-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="8111f-104">V prípade Windowsu [si pozrite odporúčania na riešenie bežných problémov s prihlásením.](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span><span class="sxs-lookup"><span data-stu-id="8111f-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="8111f-105">Pre Mac si pozrite  [článok Nie je možné prihlásiť sa do aplikácie balíka Office 2016 pre Mac.](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="8111f-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="8111f-106">**Tip** Na zariadeniach s Windowsom pre vás môžeme diagnostikovať a automaticky opraviť niekoľko bežných problémov s prihlasovaním na do balíka Office.</span><span class="sxs-lookup"><span data-stu-id="8111f-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="8111f-107">Stiahnite a spustite asistenta **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)**, aby ste mohli používať náš automatický nástroj.</span><span class="sxs-lookup"><span data-stu-id="8111f-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="8111f-108">**Poznámka:** Na riešenie problémov s prihlásením alebo aktiváciou sa neodporúča vypnúť moderné overovanie (ADAL) alebo správu webového konta (WAM).</span><span class="sxs-lookup"><span data-stu-id="8111f-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="8111f-109">Ak sa chyby vyskytnú pri pripájaní k službe Microsoft 365 pomocou balíka Office 2013, uistite sa, že pre klienta Office [povolíte](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  moderné overovanie.</span><span class="sxs-lookup"><span data-stu-id="8111f-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="8111f-110">Konkrétne akcie na riešenie problémov nájdete v týchto téme:</span><span class="sxs-lookup"><span data-stu-id="8111f-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="8111f-111">Problémy s pripojením sa pri prihlasovaní po aktualizácii na zostavu balíka Office 2016 16.0.7967 vo Windowse 10</span><span class="sxs-lookup"><span data-stu-id="8111f-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="8111f-112">Nemôžete sa prihlásiť do konta prideleného vašou organizáciou, ako je napríklad Office 365, Azure alebo Intune</span><span class="sxs-lookup"><span data-stu-id="8111f-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="8111f-113">Riešenie problémov s aplikáciami, ktoré nie sú prehliadačmi a nemožno sa prihlásiť do služieb Office 365, Azure alebo Intune</span><span class="sxs-lookup"><span data-stu-id="8111f-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="8111f-114">Opakovane výzva na zadanie poverení v Office</span><span class="sxs-lookup"><span data-stu-id="8111f-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)
---
title: Problémy s podmieneným prístupom
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015000"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="0af3e-102">Problémy s podmieneným prístupom</span><span class="sxs-lookup"><span data-stu-id="0af3e-102">Conditional access issues</span></span>

<span data-ttu-id="0af3e-103">**Riešenie problémov s diagnostickým prihlasovaním**</span><span class="sxs-lookup"><span data-stu-id="0af3e-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="0af3e-104">Pomocou [diagnostiky prihlásenia](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)môžete rýchlo zistiť, čo sa stalo alebo diagnostikovať problémy súvisiace s prihlasovaním používateľa:</span><span class="sxs-lookup"><span data-stu-id="0af3e-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="0af3e-105">Spustite diagnostické prihlásenie.</span><span class="sxs-lookup"><span data-stu-id="0af3e-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="0af3e-106">Nájdite udalosť, ktorú chcete analyzovať, zadaním podrobností o používateľovi, aplikácii, čase prihlásenia, ID požiadavky alebo identifikácii korelácie.</span><span class="sxs-lookup"><span data-stu-id="0af3e-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="0af3e-107">Prezrite si výsledky diagnostiky zobrazujúce Podrobnosti o tom, čo sa stalo a aké akcie môžete vykonať na vykonanie zmien (ak sú potrebné nejaké zmeny).</span><span class="sxs-lookup"><span data-stu-id="0af3e-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="0af3e-108">**Postup pri riešení problémov s prihlásením**</span><span class="sxs-lookup"><span data-stu-id="0af3e-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="0af3e-109">Prejdite na prihlasovaciu stránku služby Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0af3e-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="0af3e-110">Filtrovanie prihlasovacích hodnôt podľa používateľov, časového rozsahu, aplikácie, stavu, klientskej aplikácie atď.</span><span class="sxs-lookup"><span data-stu-id="0af3e-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="0af3e-111">Vyberte udalosť prihlásenia a zobrazte kartu podmieneného prístupu a zistite, ktoré politiky boli vyhodnotené.</span><span class="sxs-lookup"><span data-stu-id="0af3e-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="0af3e-112">Kliknutím na riadok politiky zobrazíte Podrobnosti o politike a rozumiete, prečo sa používa.</span><span class="sxs-lookup"><span data-stu-id="0af3e-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="0af3e-113">**Nástroje na riešenie politiky podmieneného prístupu**</span><span class="sxs-lookup"><span data-stu-id="0af3e-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="0af3e-114">Režim iba zostavy vám umožňuje vyhodnotiť politiku bez ovplyvnenia používateľov.</span><span class="sxs-lookup"><span data-stu-id="0af3e-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="0af3e-115">Nástroj co-If vám umožní simulovať udalosti pri prihlasovaní a zistiť, ktoré politiky sa používajú.</span><span class="sxs-lookup"><span data-stu-id="0af3e-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="0af3e-116">V zošite s prehľadmi a správami sa zobrazuje vplyv každej politiky v reálnom čase.</span><span class="sxs-lookup"><span data-stu-id="0af3e-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="0af3e-117">**Politiky ochrany podľa pôvodného plánu**</span><span class="sxs-lookup"><span data-stu-id="0af3e-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="0af3e-118">Politiky ochrany podľa pôvodného plánu boli zastarané.</span><span class="sxs-lookup"><span data-stu-id="0af3e-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="0af3e-119">Už nie sú presadzované a čoskoro sa odstránia z portálu Azure.</span><span class="sxs-lookup"><span data-stu-id="0af3e-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="0af3e-120">Odporúčame povoliť [predvolené nastavenia zabezpečenia](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="0af3e-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="0af3e-121">Ďalšie informácie o podmienenom prístupe nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="0af3e-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="0af3e-122">[Najvhodnejšie postupy pri podmienenom prístupe v službe Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Podmienky v podmienenom prístupe](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ovládacie prvky v podmienenom prístupe](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Umiestnenia v podmienenom prístupe](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="0af3e-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>

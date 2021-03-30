---
title: Aplikácia na overovanie
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405680"
---
# <a name="authentication-app"></a><span data-ttu-id="757e7-102">Aplikácia na overovanie</span><span class="sxs-lookup"><span data-stu-id="757e7-102">Authentication app</span></span>

<span data-ttu-id="757e7-103">Ak ste globálny správca, pomocou diagnostických nástrojov na prihlásenie môžete rýchlo zistiť, čo sa stalo, alebo diagnostikovať problémy súvisiace s [prihlásením používateľov.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="757e7-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="757e7-104">Spustite diagnostiku kliknutím na tlačidlo[Spustiť diagnostiku.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="757e7-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="757e7-105">Udalosť, ktorú chcete analyzovať, nájdete zadaním podrobností o používateľovi, aplikácii, čase prihlásenia, identifikácii požiadavky alebo identifikácii korelácie.</span><span class="sxs-lookup"><span data-stu-id="757e7-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="757e7-106">Skontrolujte diagnostické výsledky a pozrite si podrobnosti o tom, čo sa udialo, a aké akcie môžete vykonať na jej zmenu v prípade potreby.</span><span class="sxs-lookup"><span data-stu-id="757e7-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="757e7-107">**Skontrolujte scenár, ktorý je k dispozícii:**</span><span class="sxs-lookup"><span data-stu-id="757e7-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="757e7-108">Ak sa používateľovi v aplikácii Microsoft Authenticator nezobrazuje oznámenie bez oznámenia, overte, či sa nezobrazuje v časti Zablokovaní používatelia mfa, ako je to popísané v časti Blokovanie a [odblokovanie používateľov.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="757e7-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="757e7-109">Ak používateľ nie je zablokovaný pre MFA, ale nedoručuje sa upozornenie, môže otvoriť aplikáciu Microsoft Authenticator, ktorá vytiahne čakajúce žiadosti o schválenie.</span><span class="sxs-lookup"><span data-stu-id="757e7-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="757e7-110">Ako alternatívny spôsob prihlásenia môže používateľ kliknúť aj na položku Prihlásiť sa iným spôsobom a vybrať si z mojej mobilnej aplikácie overovací kód.</span><span class="sxs-lookup"><span data-stu-id="757e7-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="757e7-111">Aplikácia Microsoft Authenticator je jediným dostupným spôsobom pre mnohých používateľov.</span><span class="sxs-lookup"><span data-stu-id="757e7-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="757e7-112">[Prečítajte si ďalšie informácie o predvolených nastaveniach](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)zabezpečenia, najčastejšie [otázky o aplikácii Authenticator a](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) zistite, ako ich vyriešiť.</span><span class="sxs-lookup"><span data-stu-id="757e7-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="757e7-113">**Odporúčané videá**</span><span class="sxs-lookup"><span data-stu-id="757e7-113">**Recommended Videos**</span></span>

<span data-ttu-id="757e7-114">[Ako nastaviť aplikáciu Authenticator v novom telefóne (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="757e7-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>

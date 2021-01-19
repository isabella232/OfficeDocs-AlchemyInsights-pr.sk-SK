---
title: Chyby pri prihlasovaní používateľa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7790"
- "9004355"
ms.openlocfilehash: 05bd31cb4afecf1342e040eecd9e58cd38bd8d49
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901254"
---
# <a name="user-sign-in-errors"></a><span data-ttu-id="94178-102">Chyby pri prihlasovaní používateľa</span><span class="sxs-lookup"><span data-stu-id="94178-102">User sign-in errors</span></span>

<span data-ttu-id="94178-103">**Riešenie problémov s diagnostickým prihlasovaním**</span><span class="sxs-lookup"><span data-stu-id="94178-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="94178-104">Ak chcete zistiť príčinu alebo diagnostikovať problémy súvisiace s prihlásením používateľa, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="94178-104">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="94178-105">Spustite [diagnostické prihlásenie](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span><span class="sxs-lookup"><span data-stu-id="94178-105">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="94178-106">Nájdite udalosť, ktorú chcete analyzovať, zadaním podrobností o používateľovi, aplikácii, čase prihlásenia, ID požiadavky alebo identifikácii korelácie.</span><span class="sxs-lookup"><span data-stu-id="94178-106">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="94178-107">Skontrolujte výsledky diagnostiky, v ktorých sa zobrazujú Podrobnosti o tom, čo sa stalo a aké akcie môžete vykonať na vykonanie zmien, ak sú potrebné nejaké zmeny.</span><span class="sxs-lookup"><span data-stu-id="94178-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="94178-108">**Hľadáte informácie o chybových kódoch AADSTS, ktoré sa vracajú zo služby tokenu zabezpečenia služby Azure Active Directory (Azure AD) (STS)?**</span><span class="sxs-lookup"><span data-stu-id="94178-108">**Looking for information about the AADSTS error codes that are returned from the Azure Active Directory (Azure AD) security token service (STS)?**</span></span> <span data-ttu-id="94178-109">Prečítajte si [Tento článok](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) a nájdite AADSTS popisy chýb, opravy a niektoré navrhované alternatívne riešenia.</span><span class="sxs-lookup"><span data-stu-id="94178-109">Read [this article](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) to find AADSTS error descriptions, fixes, and some suggested workarounds</span></span>
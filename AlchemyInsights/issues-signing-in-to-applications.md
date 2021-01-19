---
title: Problémy s prihlásením do aplikácií
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
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901326"
---
# <a name="issues-signing-in-to-applications"></a>Problémy s prihlásením do aplikácií

Ak chcete zistiť príčinu alebo diagnostikovať problémy súvisiace s prihlásením používateľa, vykonajte tieto kroky:

1. Spustite [diagnostické prihlásenie](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Nájdite udalosť, ktorú chcete analyzovať, zadaním podrobností o používateľovi, aplikácii, čase prihlásenia, ID požiadavky alebo identifikácii korelácie.
3. Skontrolujte výsledky diagnostiky, v ktorých sa zobrazujú Podrobnosti o tom, čo sa stalo a aké akcie môžete vykonať na vykonanie zmien, ak sú potrebné nejaké zmeny.

Nižšie sú uvedené niektoré bežné problémy, ktoré sa môžu vyskytnúť pri prihlasovaní do aplikácií:

1. Vy alebo používateľ **dokončíte prihlásenie do služby Azure AD, ale zobrazuje sa neočakávaná výzva** – Pozrite si články [neočakávaný súhlas s výzvou pri prihlasovaní do aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) a [neočakávaná chyba pri vykonávaní súhlasu s aplikáciou](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Vy alebo používateľ **sa prihlásil priamo do aplikácie, ale nemôžete sa v ňom prihlásiť z deeplink na vlastnom portáli alebo na paneli prístupu**: Pozrite si tému [Riešenie problémov s prihlásením do aplikácie zo služby Azure AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Vy alebo používateľ **dokončil prihlásenie do služby Azure AD, ale aplikácia zobrazí chybové hlásenie a nedovolí používateľovi dokončiť prihlasovací tok**: problém je v tom, že aplikácia neprijala odpoveď, ktorú Azure AD vydal. Ak chcete riešiť problémy, postupujte podľa [týchto krokov](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) .
4. Vy alebo používateľ sa **nemôžete prihlásiť do aplikácie, ktorá nie je v galérii nakonfigurovaná na jediné prihlásenie na používanie hesla**: postupujte podľa pokynov v [týchto krokoch](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) na riešenie problémov.
5. Vy alebo používateľ sa **nemôžete prihlásiť do aplikácie galérie služby Azure AD nakonfigurovanej na jediné prihlásenie hesla**: postupujte podľa [týchto krokov](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) na riešenie problémov.
6. Vy alebo používateľ sa **nemôžete prihlásiť do aplikácie spoločnosti Microsoft**: Ak chcete riešiť problémy, postupujte podľa [týchto krokov](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) .
7. Vy alebo používateľ sa **nemôžete prihlásiť do aplikácie, ktorá nie je v galérii nakonfigurovaná pre externý jeden prihlasovanie**: postupujte podľa [týchto krokov](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) na riešenie problémov.
8. Používateľ sa **nemôže prihlásiť do aplikácie galérie služby Azure AD konfigurovanej pre externé jediné prihlásenie**: postupujte podľa [týchto krokov](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) na riešenie problémov.
9. Vy alebo používateľ sa **nemôžete prihlásiť do vlastnej aplikácie**: postupujte podľa [týchto krokov](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) na riešenie problémov.
10. Vy alebo používateľ sa **nemôžete prihlásiť do lokálnej aplikácie pomocou proxy aplikácie Azure AD**: postupujte podľa [týchto krokov](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) na riešenie problémov.


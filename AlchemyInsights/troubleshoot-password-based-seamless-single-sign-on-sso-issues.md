---
title: Riešenie problémov s bezproblémovým jediným prihlásením (SSO) založeného na hesle
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714886"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Riešenie problémov s bezproblémovým jediným prihlásením (SSO) založeného na hesle

Ak sa chcete dozvedieť základy SSO na základe hesla, pozrite si tému [overovanie na základe hesla so službou Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).

**Konfigurovanie SSO na základe hesla**

1. [Konfigurácia jediného prihlásenia založeného na hesle – v](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) tomto článku nájdete podrobnejšie informácie o možnosti SSO na základe hesla. Ak pridávaná aplikácia vyžaduje vlastnú konfiguráciu a potrebujete použiť SSO na základe hesla, tento článok je určený vám.
2. [Konfigurácia jediného prihlásenia založeného na hesle pre aplikácie v službe Prem](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) – server proxy aplikácie podporuje viaceré režimy jediného prihlásenia. Prihlásenie na základe hesla je určené pre aplikácie, ktoré používajú kombináciu používateľského mena a hesla na overenie. Pri konfigurácii prihlásenia na základe hesla pre svoju aplikáciu sa používatelia musia prihlásiť do lokálnej aplikácie raz. Za to, Azure Active Directory ukladá prihlasovacie údaje a automaticky ju poskytne aplikácii, keď používatelia prístup na diaľku.
    - Aplikáciu by ste už mali publikovať a otestovať pomocou servera proxy aplikácie. Ak nie, postupujte podľa krokov v téme [publikovanie aplikácií pomocou servera proxy aplikácie Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) a potom pokračujte v konfigurácii SSO na základe hesla pre aplikácie v službe Prem.

Riešenie problémov s SSO na základe hesla nájdete [v téme Riešenie problémov s jediným prihlásením založeným na hesle v službe Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)

---
title: Riešenie problémov s bezproblémovým jediným prihlásením pomocou hesla
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
ms.openlocfilehash: 6b4d7335461c913a6b5f782756684c5526a96c58c44853ddf9154aa51607bd4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972839"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Riešenie problémov s bezproblémovým jediným prihlásením pomocou hesla

Základy jediného prihlásenia na základe hesla nájdete v téme Overovanie na [základe hesla pomocou Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Konfigurácia jediného prihlásenia na základe hesla**

1. [Nakonfigurujte jediné prihlásenie na základe](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) hesla – tento článok obsahuje podrobnejšie informácie o možnosti jediného prihlásenia na základe hesla. Ak pridávaná aplikácia vyžaduje vlastnú konfiguráciu a potrebujete použiť jediné prihlásenie na základe hesla, tento článok je pre vás.
2. [Nakonfigurujte jediné prihlásenie na](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) základe hesla pre jednorazové aplikácie – aplikačný proxy server podporuje viaceré režimy jediného prihlásenia. Prihlásenie na základe hesla je určené pre aplikácie, ktoré na overovanie používajú kombináciu používateľského mena a hesla. Keď pre svoju aplikáciu nakonfigurujete prihlasovanie na základe hesla, používatelia sa musia raz prihlásiť do lokálnej aplikácie. Potom Azure Active Directory prihlasovacie údaje a automaticky ich poskytne aplikácii, keď k nim používatelia pristupujú na diaľku.
    - Mali by ste už publikovať a otestovať aplikáciu s aplikačným serverom proxy. Ak nie, postupujte podľa krokov v článku Publikovanie aplikácií pomocou aplikačného servera proxy služby [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) a potom pokračujte vo konfigurácii jediného prihlásenia založeného na hesloch pre predbežné aplikácie.

Informácie o riešení problémov s jediným prihlásením pomocou hesla nájdete v téme Riešenie problémov s jediným [prihlásením pomocou hesla v službe Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)

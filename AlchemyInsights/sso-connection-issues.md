---
title: Problémy s pripojením SSO
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935159"
---
# <a name="sso-connection-issues"></a>Problémy s pripojením SSO

1. Postupujte podľa pokynov pre rýchly štart [: Konfigurácia vlastností aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) sprievodca na konfiguráciu aplikácie.
2. V závislosti od zvolenej možnosti aplikácie a [jediného prihlásenia](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) postupujte podľa príslušných pokynov uvedených nižšie:
    - Ak chcete nakonfigurovať **lokálnu aplikáciu** na **jediné prihlásenie založené** na systéme SAML, pozrite si tému Nastavenie [jediného prihlásenia pre lokálne aplikácie pomocou servera proxy aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Ak chcete nakonfigurovať **cloudovú aplikáciu** na **jediné prihlásenie založeného na hesle**, pozrite si tému  [Konfigurácia jediného prihlásenia hesla](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).
    - Ak chcete nakonfigurovať **lokálnu aplikáciu** na **jediné prihlásenie prostredníctvom servera proxy aplikácie**, pozrite si tému [zaklenbovanie hesla pre jediné prihlásenie pomocou proxy aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Riešenie problémov s proxy aplikáciami**: Odporúčame vám začať s preskúmaním toku riešenia problémov, [ladenia problémov s konektormi servera proxy aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), na určenie, či sú konektory proxy aplikácie nakonfigurované správne. Ak sa stále vyskytujú problémy s pripojením k aplikácii, postupujte podľa postupu riešenia problémov v [aplikácii aplikácie proxy aplikácie Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Problémy s [Corsa môžete identifikovať](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomocou nástrojov na ladenie prehliadača:
    - Spustite prehliadač a prejdite na webovú aplikáciu.
    - Stlačením klávesu **F12** zobrazte konzolu ladenia.
    - Skúste reprodukovať transakciu a skontrolujte správu konzoly. Porušenie Corsa vytvára chybu konzoly o pôvode.
    - Niektoré problémy s Corsa nie je možné vyriešiť, napríklad ak sa vaša aplikácia presmeruje na login.microsoft.com na overenie a platnosť tokenu prístupu uplynie. Hovor Corsa potom zlyhá. Alternatívne riešenie tohto scenára je predĺžiť životnosť prístupového tokenu, aby sa zabránilo jeho platnosti počas relácie používateľa. Ďalšie informácie o postupe nájdete [v téme konfigurovateľné životnosť tokenov v platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **Riešenie problémov s jediným** prihlásením SAML: Odporúčame vám skontrolovať [problémy s prihlásením do jediného prihlásenia založeného na SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), aby ste našli riešenia problémov, s ktorými sa s najväčšou pravdepodobnosťou stretnete.
5. **Riešenie problémov s jediným prihlásením založeným na hesle**: Odporúčame overiť [Riešenie problémov s jediným prihlásením založeným na hesle v službe Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), aby ste našli riešenia problémov, s ktorými sa s najväčšou pravdepodobnosťou stretnete.
6. Informácie o problémoch s pripojením pri používaní siete VPN nájdete v téme [používanie jediného prihlásenia (SSO) cez siete VPN a pripojenia Wi-Fi](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).

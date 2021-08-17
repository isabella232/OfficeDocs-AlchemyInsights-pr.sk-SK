---
title: Problémy s pripojením jediného prihlásenia (SSO)
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
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084361"
---
# <a name="sso-connection-issues"></a>Problémy s pripojením jediného prihlásenia (SSO)

1. Postupujte podľa [funkcie Rýchly štart: Konfigurácia vlastností príručky](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) pre aplikáciu na konfiguráciu aplikácie.
2. V závislosti od vybratej [možnosti aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) a jediného prihlásenia postupujte podľa príslušných pokynov nižšie:
    - Ak chcete **nakonfigurovať** lokálnu aplikáciu pre jediné prihlásenie na základe licencie **SAML,** pozrite si časť SAML – jediné prihlásenie pre lokálne aplikácie pomocou aplikačného servera [proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - Ak chcete **nakonfigurovať cloudovú** **aplikáciu na** jediné prihlásenie na základe hesla, pozrite si [časť Konfigurácia jediného prihlásenia pomocou hesla.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)
    - Ak chcete **nakonfigurovať lokálnu aplikáciu** na jediné prihlásenie prostredníctvom aplikačného **servera proxy,** pozrite si časť Trezor hesiel pre jediné prihlásenie [s aplikačným serverom proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
3. **Riešenie problémov so serverom proxy** aplikácie: Odporúčame vám začať s revíziou toku riešenia problémov, problémov s ladením konektora [proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)aplikácie a zistiť, či sú správne nakonfigurované aplikačné proxy konektory. Ak máte stále problémy s pripojením k aplikácii, postupujte podľa pokynov na riešenie problémov v článku Ladenie problémov s aplikáciou [proxy aplikácie.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Problémy systému [CORS môžete identifikovať pomocou](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) nástrojov na ladenie prehliadača:
    - Spustite prehliadač a prejdite do webovej aplikácie.
    - Stlačte kláves **F12 a** otvorí sa ladiaca konzola.
    - Pokúste sa reprodukovať transakciu a skontrolujte správu konzoly. Porušenie cors vytvára chybu konzoly o pôvode.
    - Niektoré problémy so systémom CORS nie je možné vyriešiť, napríklad keď vaša aplikácia presmeruje do login.microsoft.com na overenie a platnosť prístupového tokenu uplynie. Hovor CORS potom zlyhá. Alternatívnym riešením pre tento scenár je predĺžiť čas platnosti prístupového tokenu a zabrániť jeho uplynutiu platnosti počas relácie používateľa. Ďalšie informácie o tom, ako to urobiť, nájdete v téme [Konfigurovateľné časy platnosti tokenov v Microsoft identity platform.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
4. Riešenie problémov s jediným prihlásením na základe kódu **SAML:** odporúčame vám skontrolovať problémy s prihlásením do aplikácií s konfiguráciou jediného prihlásenia na základe [saML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)a nájsť riešenia problémov, s ktorými sa s najväčšou pravdepodobnosťou stretnete.
5. **Riešenie problémov s jediným** prihlásením na základe hesla: ak chcete nájsť riešenia problémov s najpravdepodobnejšie, s ktorými sa môžete stretnúť, pozrite si tému Riešenie problémov s jediným prihlásením pomocou hesla v službe [Azure AD.](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
6. V prípade problémov s pripojením pri používaní siete VPN si pozrite časť Používanie jediného prihlásenia [(SSO) cez sieť VPN](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)a Wi-Fi pripojenia.

---
title: Problémy s integráciou funkcie Bezproblémové jediné prihlásenie s lokálnymi aplikáciami
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028307"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problémy s integráciou funkcie Bezproblémové jediné prihlásenie s lokálnymi aplikáciami

Pri riešení problémov s integráciou funkcie Bezproblémové jediné prihlásenie (SSO) s lokálnymi aplikáciami vykonajte tieto kroky:

**Odporúčané kroky**

1. Ak chcete **nakonfigurovať lokálnu aplikáciu** na jediné prihlásenie prostredníctvom aplikačného **servera proxy,** pozrite si časť Trezor hesiel pre jediné prihlásenie [s aplikačným serverom proxy.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **Riešenie problémov so serverom proxy** aplikácie: odporúčame vám začať s revíziou toku riešenia [problémov,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)problémov s ladením konektora proxy aplikácie a zistiť, či sú konektory proxy aplikácie správne nakonfigurované. Ak máte stále problémy s pripojením k aplikácii, postupujte podľa krokov na riešenie problémov v článku Ladenie problémov s [aplikáciou proxy aplikácie.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps) Problémy systému [CORS môžete identifikovať pomocou](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) nasledujúcich nástrojov na ladenie prehliadača:
    1. Spustite prehliadač a prejdite do webovej aplikácie.
    1. Stlačte kláves **F12 a** otvorí sa ladiaca konzola.
    1. Pokúste sa reprodukovať transakciu a skontrolujte správu konzoly. Porušenie cors vytvára chybu konzoly o pôvode.
    1. Niektoré problémy so systémom CORS nie je možné vyriešiť, napríklad keď vaša aplikácia presmeruje login.microsoftonline.com na overenie a platnosť prístupového tokenu uplynie. Hovor CORS potom zlyhá. Alternatívnym riešením pre tento scenár je predĺžiť čas platnosti prístupového tokenu a zabrániť jeho uplynutiu platnosti počas relácie používateľa. Ďalšie informácie o tom, ako to urobiť, nájdete v téme [Konfigurovateľné časy platnosti tokenov v Microsoft identity platform.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)

**Odporučené dokumenty**

- [Konfigurácia jediného prihlásenia do aplikácie proxy aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Jediné prihlásenie SAML pre lokálne aplikácie s aplikačným serverom proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Porozumenie a riešenie Azure Active Directory problémov servera proxy aplikácie CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Riešenie problémov s konfiguráciou delegovania s protokolom Kerberos v prípade aplikačného proxy servera](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
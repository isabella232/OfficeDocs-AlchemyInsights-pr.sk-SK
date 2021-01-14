---
title: Problémy so začlenením bezšvíkových SSO s lokálnymi aplikáciami
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
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/13/2021
ms.locfileid: "49868723"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>Problémy so začlenením bezšvíkových SSO s lokálnymi aplikáciami

Ak chcete riešiť problémy so začlenením bezproblémového SSO s lokálnymi aplikáciami, postupujte takto:

**Odporúčané kroky**

1. Ak chcete nakonfigurovať **lokálnu aplikáciu** na **jediné prihlásenie prostredníctvom servera proxy aplikácie**, pozrite si tému [zaklenbovanie hesla pre jediné prihlásenie pomocou proxy aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
1. **Riešenie problémov s proxy aplikáciami**: Odporúčame, aby ste začali s preskúmaním toku riešenia problémov, [ladenia problémov s konektormi servera proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), a zistite, či sú konektory aplikačného servera proxy správne nakonfigurované. Ak sa stále vyskytujú problémy s pripojením k aplikácii, postupujte podľa krokov na riešenie problémov v [aplikáciách aplikácie proxy aplikácie Debug](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). Problémy s [Corsa môžete identifikovať](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) pomocou nasledujúcich nástrojov ladenia prehliadača:
    1. Spustite prehliadač a prejdite na webovú aplikáciu.
    1. Stlačením klávesu **F12** zobrazte konzolu ladenia.
    1. Skúste reprodukovať transakciu a skontrolujte správu konzoly. Porušenie Corsa vytvára chybu konzoly o pôvode.
    1. Niektoré problémy s Corsa nie je možné vyriešiť, napríklad ak sa vaša aplikácia presmeruje na login.microsoftonline.com na overenie a platnosť tokenu prístupu uplynie. Hovor Corsa potom zlyhá. Alternatívne riešenie tohto scenára je predĺžiť životnosť prístupového tokenu, aby sa zabránilo jeho platnosti počas relácie používateľa. Ďalšie informácie o postupe nájdete [v téme konfigurovateľné životnosť tokenov v platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

**Odporúčané dokumenty**

- [Konfigurovanie jediného prihlásenia do aplikácie proxy aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [Použitie jediného prihlásenia cez SAML pre lokálne aplikácie so serverom proxy aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [Informácie o problémoch so serverom proxy aplikácie Azure Active Directory Corsa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [Riešenie problémov s obmedzeniami delegovania Kerberos pre aplikačný server proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
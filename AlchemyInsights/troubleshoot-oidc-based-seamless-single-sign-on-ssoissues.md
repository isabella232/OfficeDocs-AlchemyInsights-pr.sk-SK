---
title: Riešenie problémov s bezproblémovo jediným prihlásením pomocou OIDC
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
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105793"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Riešenie problémov s bezproblémovo jediným prihlásením pomocou OIDC

- Informácie o pridaní aplikácie typu OIDC do nájomníka služby Azure nájdete v téme Rýchly štart: Nastavenie jediného prihlásenia [(SSO)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)založeného na OIDC pre aplikáciu v nájomníkovi služieb Azure Active Directory (Azure AD).
- Ďalšie informácie o aplikáciách, ktoré používajú štandard OpenID Pripojenie na implementáciu jediného prihlásenia, nájdete v téme Informácie o jedinom prihlásení pomocou funkcie [OIDC.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)
- Informácie pre prípad, že sa rozhodnete vytvoriť kód priamo odoslaním a spracovaním požiadaviek HTTP alebo použijete knižnicu open-source tretej strany namiesto použitia jednej z našich knižníc s otvoreným zdrojovým kódom, pozrite si balíky [OAuth 2.0 a Protokoly OpenID Pripojenie](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)na serveri Microsoft identity platform.

**Protokoly**

1. Microsoft identity platform a [implicitné](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) udelenie – definovanou charakteristikou implicitného grantu je, že tokeny (ID tokeny alebo prístupové tokeny) sa vracajú priamo z koncového bodu /authorize namiesto koncového bodu /token. Tento postup sa často používa ako súčasť toku kódu oprávnenia v tzv. hybridnom toku – načítava sa ID token v žiadosti **/authorize** spolu s kódom oprávnenia . Tento článok popisuje, ako programovať priamo voči protokolu v aplikácii a požiadať o tokeny zo služby Azure AD.
2. [Microsoft identity platform a OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – tok kódu oprávnenia OAuth 2.0 sa môže používať v aplikáciách nainštalovaných v zariadení na získanie prístupu k chráneným zdrojom, ako je napríklad webové APIs. Pomocou Microsoft identity platform OAuth 2.0 môžete pridať prihlásenie a prístup rozhrania API k mobilným a počítačových **aplikáciám.** Tento článok popisuje, ako programovať priamo voči protokolu vo vašej aplikácii pomocou ľubovoľného jazyka.
3. Microsoft identity platform protokol [Pripojenie OpenID](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – pri implementácii protokolu OpenID Pripojenie Microsoft identity platform pre Microsoft identity platform môžete pridať prihlásenie a prístup k aplikáciám pomocou rozhrania API. Tento článok popisuje postup nezávisle od jazyka a popisuje, ako odosielať a prijímať správy HTTP bez použitia knižníc **s otvoreným zdrojovým zdrojom od spoločnosti Microsoft.**
4. Microsoft identity platform a tok poverení klienta [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – na prístup k zdrojom hosťovaných na webe pomocou identity aplikácie môžete použiť poskytnutie poverení klienta OAuth 2.0 zadané v RFC 6749, niekedy nazývané aj **OAuth** s dvomi tvormi. Tento typ grantu sa bežne používa na interakciu medzi servermi, ktoré sa musia spúšťať na pozadí bez okamžitej interakcie s používateľom. Tieto typy aplikácií sa často označujú ako **služba daemons** alebo **kontá služieb.** Tento článok popisuje, ako programovať priamo s protokolom vo vašej aplikácii.

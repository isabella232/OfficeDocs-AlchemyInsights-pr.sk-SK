---
title: Riešenie problémov s bezproblémovým jediným prihlásením na OIDC (SSO)
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
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747130"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>Riešenie problémov s bezproblémovým jediným prihlásením na OIDC (SSO)

- Ak chcete zistiť, ako pridať aplikáciu OIDC do nájomníka Azure, pozrite si tému rýchly [Štart: nastavenie jediného prihlásenia na OIDC (SSO) pre aplikáciu v nájomníkovi služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Ďalšie informácie o aplikáciách, ktoré používajú funkciu OpenID Connect Standard na implementáciu jediného prihlásenia, nájdete v téme [vysvetlenie jediného prihlásenia založeného na OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Informácie v prípade, že sa rozhodnete napísať svoj kód priamym odoslaním a spracovaním HTTP požiadaviek alebo pomocou knižnice s otvorenými zdrojmi tretej strany namiesto použitia niektorého z našich otvorených knižníc, pozrite si tému [OAuth 2,0 a OpenID Connect Protocols na platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokoly**

1. [Platforma Microsoft identity a implicitný tok grantov](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) – určujúca vlastnosť implicitnej subvencie je, že tokeny (tokeny identifikácie alebo Prístupové tokeny) sa vracajú priamo z koncového bodu/Authorize namiesto koncového bodu/token. Tento postup sa často používa ako súčasť toku kódu povolenia, v ktorom sa nazýva **"hybridný tok" – načítanie tokenu ID na žiadosť o/Authorize spolu s kódom autorizácie**. V tomto článku sa popisuje, ako program priamo v protokole v aplikácii požadovať tokeny zo služby Azure AD.
2. [Microsoft Identity Platform a oauth 2,0 autorizačný kód flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) – OAuth 2,0 autorizačný kód grant možno použiť v aplikáciách, ktoré sú nainštalované v zariadení na získanie prístupu k chráneným zdrojom, ako sú napríklad webové rozhrania API. Pomocou aplikácie Microsoft Identity Platform implementácia OAuth 2,0 môžete **pridať prihlásenie a API prístup k mobilnej a počítačovej aplikácii**. V tomto článku sa popisuje, ako naprogramovať priamo protokol v aplikácii pomocou ľubovoľného jazyka.
3. [Platforma Microsoft identity a OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) – Ak používate aplikáciu OpenID na pripojenie platformy Microsoft identity, môžete do svojich aplikácií pridať prihlasovacie rozhranie a prístup k nim. V tomto článku je znázornené, ako to urobiť nezávisle od jazyka a popisuje spôsob **odosielania a prijímania správ http bez použitia akýchkoľvek knižníc s otvorenými zdrojmi Microsoft**.
4. [Microsoft Identity Platform a tok poverení klienta oauth 2,0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) – môžete použiť poverenia klienta OAuth 2,0, ktoré sú uvedené v dokumente RFC 6749, niekedy sa nazývajú **dva-legged OAuth**, na prístup k webovým zdrojom s použitím totožnosti aplikácie. Tento typ grantu sa bežne používa pre interakcie medzi servermi a servermi, ktoré musia byť spustené na pozadí bez nutnosti okamžitej interakcie s používateľom. Tieto typy aplikácií sa často označujú ako **démoni** alebo **kontá služby**. V tomto článku sa popisuje, ako naprogramovať priamo voči protokolu v aplikácii.

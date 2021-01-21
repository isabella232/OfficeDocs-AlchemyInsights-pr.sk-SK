---
title: Problémy s tokenmi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917034"
---
# <a name="issues-with-tokens"></a>Problémy s tokenmi

Ak chcete spravovať problémy súvisiace s tokenmi, môžete vykonať tieto kroky:

1. Môžete zadať životnosť tokenu Accessu, ID alebo SAML vydaného spoločnosťou Microsoft Identity Platform. Môžete nastaviť životnosť tokenov pre všetky aplikácie vo vašej organizácii, pre aplikáciu viacerých nájomníkov (multi-Organization) alebo pre konkrétnu službu v organizácii. Ďalšie informácie nájdete v téme [konfigurovateľná životnosť tokenov v platforme Microsoft Identity (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Prístupové tokeny umožňujú klientom bezpečne zavolať na chránené webové rozhrania API a používajú webové rozhrania API na overovanie a autorizáciu. Pokiaľ ide o špecifikáciu OAuth, accessové tokeny sú nepriehľadné reťazce bez množiny formátov – niektorí poskytovatelia identity (IDP) používajú identifikátory GUID, iné používajú šifrované guličky. Platforma Microsoft Identity používa rôzne formáty prístupových tokenov v závislosti od konfigurácie rozhrania API, ktoré prijíma token. Ďalšie informácie o overení a používaní pohľadávok v accessovom tokene nájdete v téme [tokeny prístupu ku platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Knižnica Microsoft Authentication Library (MSAL) podporuje viacero tokov overovania, ktoré sa používajú v rôznych scenároch aplikácie. Ďalšie informácie nájdete v téme [toky overovania](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. Grantový kód autorizácie OAuth 2,0 možno použiť v aplikáciách, ktoré sú nainštalované v zariadení na získanie prístupu k chráneným zdrojom, ako sú napríklad webové rozhrania API. Pomocou aplikácie Microsoft Identity Platform implementácia OAuth 2,0 môžete pridať prihlasovacie a API prístup k mobilnej a počítačovej aplikácii. Pozrite si tému [Microsoft Identity Platform and OAuth 2,0 autorizačný kód](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) na spôsob, akým program priamo v protokole v aplikácii používa ľubovoľný jazyk.
5. OpenID Connect (OIDC) je overovací protokol založený na OAuth 2,0, ktorý môžete použiť na bezpečné prihlásenie používateľa do aplikácie. Keď použijete koncové body aplikácie Microsoft Identity Platform na implementáciu funkcie OpenID Connect, môžete do svojich aplikácií pridať prihlasovacie rozhranie a prístup k nim. [Microsoft Identity Platform a OpenID Connect Protocol](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) ukazuje, ako to urobiť nezávisle od jazyka a popisuje, ako odosielať a dostávať http správy bez použitia akýchkoľvek knižníc s otvorenými zdrojmi Microsoft.
    - Koncový bod UserInfo je súčasťou štandardu OIDC, ktorý je určený na vrátenie pohľadávok o používateľoch, ktorých overenie je overené. Ďalšie informácie nájdete v téme [koncového bodu platformy Microsoft Identity UserInfo](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Volanie webového rozhrania API vo webovej aplikácii pomocou služby Azure AD a OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) sample ukazuje, ako vytvoriť MVC webovú aplikáciu, ktorá používa Azure AD na prihlásenie pomocou protokolu OpenID Connect, a potom zavolať na webové rozhranie API pod identitou prihláseného používateľa pomocou tokenov získaných prostredníctvom OAuth 2,0. Táto vzorka používa funkciu OpenID Connect ASP .net OWIN middleware a ADAL .net.
6. [Konfigurácia aplikácie na vystavenie webového rozhrania API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) – v tomto rýchlych nastaveniach môžete zaregistrovať webovú API s platformou Microsoft identity a vystaviť ju klientskym aplikáciám pridaním príkladu rozsahu. Registráciou webového rozhrania API a jeho vystavením prostredníctvom rozsahov môžete na základe povolení poskytnúť prístup k svojim zdrojom pre oprávnených používateľov a klientske aplikácie, ktoré majú prístup k vášmu API.
7. V službe Azure Active Directory B2C (Azure AD B2C) je tok prostriedkov na zadanie hesla vlastníka zdroja (ROPC) vlastníkom OAuth štandardný tok overovania. V tomto toku sa aplikácia, ktorá sa označuje aj ako závislá strana, vymieňa platné poverenia pre tokeny. Poverenia zahŕňajú identifikáciu používateľa a heslo. Vrátené tokeny sú IDENTIFIKAČNÝm tokenom, tokenom prístupu a tokenom obnovenia. Ďalšie informácie nájdete v téme [Nastavenie toku poverení hesla vlastníka prostriedku v službe Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 


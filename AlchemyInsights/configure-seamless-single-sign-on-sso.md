---
title: Konfigurácia bezproblémového jediného prihlásenia (SSO)
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: 62f667cccd0761e081b3f651709fadfec12500e76fd8e30b8649a28e99001e4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53966052"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurácia bezproblémového jediného prihlásenia (SSO)

**Konfigurovanie aplikácií**

1. Hodnoty by ste mali získať od dodávateľa aplikácie. Hodnoty môžete manuálne zadať alebo nahrať súbor metaúdajov na extrahovanie hodnoty polí.
2. Mnohé aplikácie už boli vopred nakonfigurované na prácu so službou Azure AD. Tieto aplikácie sú uvedené v galérii aplikácií, ktoré môžete prehľadávať po pridaní aplikácie do nájomníka služby Azure AD. Séria [Rýchly štart](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) vás procesom obsahuje.
3. Ak chcete vytvoriť aplikáciu, ktorá nie je galéria, môžete kliknúť na **položku +** Vytvoriť vlastnú aplikáciu a pomenovať aplikáciu.
    - Predvolene sa vyberie možnosť Integrovať **všetky ostatné** aplikácie, ktoré v galérii nenájdete, čo je správna možnosť pre aplikácie, ktoré nie sú galériami.
    - Po uvedení **názvu aplikácie** na tlačidlo Vytvoriť sa vytvorí nová podniková aplikácia mimo galérie.
    - Potom môžete prejsť na položku Jediné  prihlásenie **v** časti Spravovanie tejto aplikácie a uvidíte rôzne spôsoby jej implementácie vo svojom prostredí.

**Konfigurácia bezproblémového jediného prihlásenia pre konkrétnu aplikáciu**

Pre aplikácie v galérii nájdete podrobné podrobné pokyny. Ak chcete získať prístup k postupu, môžete prehľadávať zoznam všetkých kurzov o konfigurácii aplikácií v kurzoch konfigurácie aplikácie [SaaS.](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)

**Konfigurácia jediného prihlásenia na základe súborov SAML**

1. Rýchly štart: Nastavte jediné prihlásenie (SSO) založené na saML pre aplikáciu v [nájomníkovi služby Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso)
2. Ďalšie informácie o možnosti založenej na saml pre jediné prihlásenie nájdete v téme Oboznámte sa s jediným prihlásením na [základe saml.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)
3. Ďalšie informácie o žiadostiach o overovanie SAML 2.0 a odpovediach, ktoré podporuje Azure Active Directory (Azure AD) pre jediné prihlásenie Sign-On (SSO), nájdete v téme Jediné prihlásenie [Sign-On SAML.](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
4. Informácie o vytvorení a konfigurácii jediného prihlásenia (SSO) založeného na saML pre aplikáciu v službe Azure Active Directory (Azure AD) pomocou rozhrania Microsoft Graph API nájdete v téme Konfigurácia jediného prihlásenia pomocou rozhrania API založeného na saML pre aplikáciu pomocou rozhrania [Microsoft Graph API.](https://docs.microsoft.com/graph/application-saml-sso-configure-api)
5. Ak chcete zistiť, ako Azure AD používa protokol SAML, pozrite si [časť Microsoft identity platform používa protokol SAML.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)

**Konfigurácia tokenov a nárokov**

1. [Postup: prispôsobenie nárokov vydaných v tokene SAML pre podnikové aplikácie.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)
2. Informácie o konfigurácii nárokov pomocou prostredia PowerShell nájdete v téme Postup: Prispôsobenie nárokov, ktoré sa vynechajú v tokenoch pre konkrétnu aplikáciu v [nájomníkovi (verzia Preview).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
3. Informácie o konfigurácii voliteľných nárokov nájdete v [téme Postup: Poskytnutie voliteľných nárokov do aplikácie.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
4. Ak chcete zistiť, ako používať atribúty prípony schémy adresára na odosielanie používateľských údajov do aplikácií v nárokoch na tokeny, pozrite si časť Používanie atribútov [prípony schémy adresára v nárokoch.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)
5. Ak chcete zistiť, ako konfigurovať časy platnosti tokenov, pozrite si tému Konfigurovateľné [časy platnosti tokenov Microsoft identity platform (ukážka).](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Konfigurácia politík platnosti tokenov (ukážka)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – V tomto článku sa nachádza bežný scenár politiky, ktorý vám môže pomôcť nastaviť nové pravidlá pre čas platnosti tokenov. V uvedenom príklade sa naučíte, ako vytvoriť politiku, ktorá vyžaduje od používateľov častejšie overenie vo vašej webovej aplikácii.

**Riešenie problémov s konfiguráciou jediného prihlásenia (SSO)**

- Najčastejšie otázky o jedinom prihlásení Azure Active Directory bezproblémové jediné prihlásenie Sign-On (seamless SSO) nájdete Azure Active Directory bezproblémové jediné [prihlásenie: najčastejšie otázky.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)
- Informácie o riešení bežných problémov týkajúcich sa služieb Azure Active Directory (Azure AD) Bezproblémové jediné prihlásenie Sign-On (seamless SSO) nájdete v Azure Active Directory Riešenie problémov s jediným [prihlásením.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)

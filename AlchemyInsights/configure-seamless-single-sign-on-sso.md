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
- "9384"
ms.openlocfilehash: 32790b23547de36cd2864e85ebae67f54ad91707
ms.sourcegitcommit: 309b9f3e6e2ff622f95bb860d337d2c05b7bbe54
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/15/2021
ms.locfileid: "50841673"
---
# <a name="configure-seamless-single-sign-on-sso"></a>Konfigurácia bezproblémového jediného prihlásenia (SSO)

**Konfigurácia aplikácií**

1. Mali by ste získať hodnoty od dodávateľa aplikácie. Ak chcete extrahovať hodnotu polí, môžete manuálne zadať hodnoty alebo nahrať súbor metaúdajov.
2. Mnohé aplikácie už boli vopred nakonfigurované tak, aby fungovali so službou Azure AD. Tieto aplikácie sú uvedené v galérii aplikácií, ktoré môžete prehľadávať pri pridávaní aplikácie do nájomníka služby Azure AD. [Rad](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) rýchlych krokov vás bude sprevádzať procesom.
3. Ak chcete vytvoriť aplikáciu, ktorá nie je Galéria, môžete kliknúť na položku **+ vytvoriť vlastnú aplikáciu** a pomenovať ju do aplikácie.
    - Predvolene sa vyberie možnosť **integrovať všetky ostatné aplikácie, ktoré nenájdete v galérii** , ktorá je správnou možnosťou pre aplikácie mimo galérie.
    - Keď po zadaní názvu aplikácie stlačíte kláves **Create** , vytvorí sa nová podniková aplikácia, ktorá nie je Galéria.
    - Potom sa môžete prejsť na **jediné prihlásenie** v časti **spravovanie** tejto aplikácie a budete môcť zobraziť rôzne postupy na jej realizáciu vo vašom prostredí.

**Konfigurácia bezproblémového SSO pre konkrétnu aplikáciu**

Informácie o aplikáciách v galérii nájdete v podrobných pokynoch, krok za krokom. Ak chcete získať prístup k krokom, môžete si pozrieť zoznam všetkých kurzov konfigurácie aplikácií v [kurzoch konfigurácie aplikácií SaaS](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list).

**Konfigurácia jediného prihlásenia na základe SAML**

1. Rýchly [Štart: nastavenie jediného prihlásenia na základe SAML (SSO) pre aplikáciu v nájomníkovi služby Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso).
2. Ďalšie informácie o možnosti založenej na SAML pre jediné prihlásenie nájdete v téme [vysvetlenie jediného prihlásenia založeného na SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on).
3. Ďalšie informácie o požiadavkách na overenie SAML 2,0 a odpovediach, ktoré podporuje Azure Active Directory (Azure AD) pre jednu Sign-On (SSO), nájdete v téme [single Sign-On protokol SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol).
4. Ďalšie informácie o vytváraní a konfigurácii jediného prihlásenia (SSO) pre vašu aplikáciu v službe Azure Active Directory (Azure AD) pomocou rozhrania API Microsoft Graphu nájdete v téme [Konfigurácia jediného prihlásenia v službe SAML pre aplikáciu pomocou rozhrania Microsoft Graph API](https://docs.microsoft.com/graph/application-saml-sso-configure-api).
5. Informácie o tom, ako Azure AD používa protokol SAML, nájdete [v téme ako platforma Microsoft Identity používa protokol SAML](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference).

**Konfigurovanie tokenov a pohľadávok**

1. [Postup: prispôsobenie pohľadávok vydaných v tokene SAML pre podnikové aplikácie](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).
2. Informácie o konfigurácii tvrdení pomocou prostredia PowerShell nájdete v téme [postup: prispôsobenie pohľadávok emitovaných tokenmi pre konkrétnu aplikáciu v nájomníkovi (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).
3. Informácie o konfigurácii voliteľných pohľadávok nájdete v téme [postup: poskytovanie voliteľných nárokov v aplikácii](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).
4. Ďalšie informácie o používaní atribútov prípony v adresárovej schéme na odosielanie používateľských údajov do aplikácií v tokenových pohľadávkach nájdete [v téme Používanie atribútov rozšírenia schémy adresára v rámci pohľadávok](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions).
5. Ak sa chcete dozvedieť, ako nakonfigurovať životnosť tokenov, pozrite si tému [životnosť konfigurovaných tokenov v platforme Microsoft Identity (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
6. [Konfigurácia politík ochrany tokenov (Preview)](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) – v tomto článku prechádzame bežným politickým scenárom, ktorý vám môže pomôcť pri ukladaní nových pravidiel pre životnosť tokenov. V tomto príklade sa naučíte, ako vytvoriť politiku, ktorá vyžaduje, aby sa používatelia v rámci webovej aplikácie často overovali.

**Riešenie problémov s konfiguráciou SSO**

- Najčastejšie otázky o službe Azure Active Directory bezproblémová jednoduchá Sign-On (bezproblémové SSO) nájdete v téme [bezproblémové jediné prihlásenie v službe Azure Active Directory: najčastejšie otázky](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq).
- Riešenie problémov s informáciami o bežných problémoch týkajúcich sa jednoduchej služby Azure Active Directory (Azure AD) jednoduchého Sign-On (bezšvíkové SSO) nájdete v téme [Riešenie problémov so službou Azure Active Directory bezproblémové jediné prihlásenie](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso).

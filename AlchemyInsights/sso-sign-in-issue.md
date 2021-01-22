---
title: Problémy s prihlasovaním používateľov na bezproblémové prihlásenie
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
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935181"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Problémy s prihlasovaním používateľov na bezproblémové prihlásenie

Po overení používateľa bude prehliadač ukladať do vyrovnávacej pamäte poverenia používateľa tak, aby sa v tom istom prehliadači aplikácia automaticky prihlasoval s rovnakým kontom. Môže to sťažiť inému používateľovi alebo jednému používateľovi prihlásiť sa do viacerých kont v jednom zariadení. Ak chcete tento problém vyriešiť: 1. Skúste sa prihlásiť v inom prehliadači. 2. Vymažte vyrovnávaciu pamäť prehliadača a/alebo súbory cookie a skúste sa prihlásiť znova.

Ak sa stále vyskytujú problémy s prihlásením, odporúčame vám diagnostikovať a automatizovať kroky na riešenie problémov:

1. Nainštalujte si [rozšírenie zabezpečeného prehliadača My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) na pomoc služby Azure Active Directory (Azure AD), aby sa pri používaní skúšobných skúseností na portáli Azure zobrazila lepšia diagnóza a rozlíšenia.
2. Reprodukovať chybu s použitím skúšobnej skúsenosti na stránke konfigurácie aplikácie na portáli Azure Portal. Ďalšie informácie nájdete v téme [ladenie aplikácií jediného prihlásenia na základe SAML](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Ak používate skúšobnú službu na portáli Azure s príponou zabezpečeného prehliadača moje aplikácie, môžete **Preskočiť krok 4**.
4. Ak chcete otvoriť stránku konfigurácie jediného prihlásenia na stránke SAML:
    - Otvorte [portál Azure](https://portal.azure.com/) a prihláste sa ako **globálny správca** alebo správca .
    - Otvorte **rozšírenie Azure Active Directory** výberom položky **všetky služby** v hornej časti hlavnej navigačnej ponuky na ľavej strane.
    - Do vyhľadávacieho poľa filtra zadajte výraz "Azure Active Directory" a vyberte položku **Azure Active Directory** .
    - Vyberte položku **podnikové aplikácie** z ľavej navigačnej ponuky služby Azure Active Directory.
    - Ak chcete zobraziť zoznam všetkých aplikácií, vyberte položku **všetky aplikácie** . Ak sa vám nezobrazuje aplikácia, ktorú chcete zobraziť, použite ovládací prvok **Filter** v hornej časti **zoznamu všetky aplikácie** a nastavte možnosť **Zobraziť** na **všetky aplikácie**.
    - Vyberte aplikáciu, ktorú chcete nakonfigurovať na jediné prihlásenie.
    - Po načítaní aplikácie vyberte možnosť **jediné prihlásenie** z ľavej navigačnej ponuky aplikácie.
    - Vyberte položku **jediné prihlásenie na základe SAML**.
5. Na základe chyby sa dozviete viac o odporúčaných krokoch, ktoré je potrebné vykonať, nájdete [v téme problémy s prihlasovaním do aplikácií založených na SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Ak chcete riešiť problémy s prihlasovaním ostatných používateľov, pozrite si tieto pokyny:
    - [Jednoduché Sign-On protokolu SAML](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Postup: riešenie chýb prihlasovania pomocou zostáv služby Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Výzva na neočakávané schválenie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Chyba súhlasu používateľa](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problémy s prihlásením z priečinka Moje aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Chyba na prihlasovacej stránke aplikácie](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problém s prihlásením do aplikácie spoločnosti Microsoft](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)

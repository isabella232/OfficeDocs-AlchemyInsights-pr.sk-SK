---
title: Problémy s vývojom aplikácií
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974768"
---
# <a name="issues-developing-applications"></a>Problémy s vývojom aplikácií

Ak chcete riešiť najbežnejšie problémy pri budovaní aplikácií služby Azure Active Directory (AD), prečítajte si tieto články:

- [Zobrazujem problémy s prihlásením do aplikácie (s) iba pomocou prehliadača Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Neviem, ako zmeniť predvolené nastavenia tokenu životnosti pre moju aplikáciu](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Som zmätená o tom, ako funguje súhlas so žiadosťou](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Neviem, ako udeliť povolenia mojej aplikácii](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nechápem rozdiel medzi delegovanými povoleniami a povoleniami na aplikácie](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Koniec podpory pre Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph)** _

- Od 30. júna 2020, už nebudeme pridávať žiadne nové funkcie do služby Azure Active Directory Authentication Library (ADAL) a Azure AD Graph API (AAD Graph). Budeme aj naďalej poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudú poskytovať aktualizácie funkcií.

- Od 30. júna 2022, ukončíme podporu pre ADAL a AAD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia. Výsledkom tejto podmienky sú tieto dôsledky:

    - Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však mať žiadne technické podpory ani aktualizácie zabezpečenia.

    - Aplikácie, ktoré používajú AAD Graph po uplynutí tohto času, už nemusia dostávať odpovede od koncového bodu grafu AAD

_ *Migrácia ADAL**

Ak používate aplikácie spoločnosti Microsoft, odporúčame vám aktualizovať knižnicu Microsoft Authentication Library (MSAL), ktorá obsahuje najnovšie funkcie a aktualizácie zabezpečenia. Toto odporúčanie je v kontexte Microsoftu, ktorým sa iniciuje proces prechodu svojich aplikácií na MSAL podľa termínu ukončenia podpory. 

Migrácia aplikácií spoločnosti Microsoft na MSAL zabezpečuje, že aplikácie budú mať prospech z pokračujúcich funkcií zabezpečenia a vylepšení funkcie MSAL.

1. [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Informácie o tom, ako migrovať aplikácie na základe jednotlivých platforiem](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ak potrebujete pomoc pri pochopení, ktoré z vašich aplikácií používajú ADAL, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a prípadne osloviť nezávislých dodávateľov softvéru (ISV) alebo poskytovateľov aplikácií. Technická podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií, ktoré nie sú Microsoft ADAL v nájomníkovi.

**Migrácia grafu AAD**

V prípade aplikácií, ktoré používajú AAD Graph, postupujte podľa pokynov na migráciu aplikácie AAD Graph do programu Microsoft Graph:

1. [Náš kontrolný zoznam migrácie poskytuje bod začiatku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Na portáli registrácie aplikácie Azure sa zobrazuje, ktoré aplikácie používajú AAD Graph. Odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a v prípade potreby osloviť nezávislých dodávateľov softvéru (ISV) alebo poskytovateľov aplikácií. Technická podpora spoločnosti Microsoft vám tiež poskytuje informácie o používaní AAD grafov v nájomníkovi.








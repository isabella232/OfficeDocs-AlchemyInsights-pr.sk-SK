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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013439"
---
# <a name="issues-developing-applications"></a>Problémy s vývojom aplikácií

Ak chcete vyriešiť najčastejšie problémy pri budovaní Azure Active Directory (AD), pozrite si tieto články:

- [Mám problém prihlásiť sa len do aplikácií pomocou prehliadača Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Neviem, ako zmeniť predvolené hodnoty platnosti tokenu pre aplikáciu](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Nie som si istý tým, ako funguje súhlas k aplikácii](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Neviem, ako udeliť povolenia mojej aplikácii](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nerozumiem rozdielu medzi delegovanými povoleniami a povoleniami aplikácie](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Ukončenie podpory pre Azure Active Directory overovanie (ADAL) a Azure AD Graph API (AAD Graph)***

- Od 30. júna 2020 už nebudeme pridávať žiadne nové funkcie do knižnice Azure Active Directory Authentication Library (ADAL) a rozhrania AD Graph API (AAD Graph). Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.

- Od 30. júna 2022 ukončíme podporu pre ADAL a AAD Graph a nebudeme poskytovať technickú podporu ani aktualizácie zabezpečenia. Dôsledkom tejto podmienky sú dôsledky nasledovné:

    - Aplikácie používajúce ADAL v existujúcich verziách operačného systému budú fungovať aj naďalej, ale nebudú mať k dispozícii žiadnu technickú podporu ani aktualizácie zabezpečenia.

    - Aplikácie používajúce AAD Graph po tomto čase už nemusia prijímať odpovede z koncového bodu služby AAD Graph AAD

**Migrácia ADAL**

Ak používate aplikácie spoločnosti Microsoft, odporúčame vám aktualizovať na knižnicu Microsoft Authentication Library (MSAL), ktorá obsahuje najnovšie funkcie a aktualizácie zabezpečenia. Toto odporúčanie je v kontexte spoločnosti Microsoft, počas procesu migrácie aplikácií do služby MSAL do termínu ukončenia podpory. 

Migrácia aplikácií do MSAL spoločnosťou Microsoft zabezpečí, že aplikácie budú ťažiť z priebežného zabezpečenia a vylepšení funkcií spoločnosti MSAL.

1. [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Informácie o migrácii aplikácií na platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ak potrebujete pomoc s tým, ktoré z vašich aplikácií používajú ADAL, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a v prípade potreby sa kontaktovať akýchkoľvek nezávislých dodávateľov softvéru (ISVs) alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.

**Migrácia AAD Graph**

V prípade aplikácií, ktoré používajú službu AAD Graph, postupujte podľa našich pokynov na migráciu aplikácií AAD Graph do služby Microsoft Graph:

1. [Náš kontrolný zoznam migrácie obsahuje informácie na začiatok](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Portál registrácie aplikácie Azure zobrazuje aplikácie, ktoré používajú AAD Graph. Odporúčame vám skontrolovať všetky zdrojové kódy aplikácií a ak je to možné, kontaktovať všetkých nezávislých dodávateľov softvéru (ISVs) alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám môže tiež poskytnúť informácie o používaní AAD Graph používanie služby AAD vo vašom nájomníkovi.








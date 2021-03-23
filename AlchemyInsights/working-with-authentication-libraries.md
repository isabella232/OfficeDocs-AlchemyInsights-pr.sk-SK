---
title: Práca s knižnicami na overovanie
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036869"
---
# <a name="working-with-authentication-libraries"></a>Práca s knižnicami na overovanie

Ak chcete vyriešiť problém s knižnicou Microsoft Authentication Library (MSAL), vykonajte tieto Odporúčané kroky:

1. **Práca s MSAL**: [knižnice overovania platformy Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – v tomto článku sa zobrazuje podpora knižnice Microsoft Authentication Library pre viacero typov aplikácií. Obsahuje prepojenia na zdrojový kód knižnice. kde získate balík pre projekt vašej aplikácie, a či knižnica podporuje prihlásenie používateľa (overenie), prístup k zabezpečeným webovým rozhraniam API (autorizácia) alebo obom.

2. **Riešenie problémov s overovaním**: MSAL podporuje viacero tokov overovania, ktoré sa používajú v rôznych scenároch aplikácie. V závislosti od toho, ako je vaša klientska aplikácia vytvorená, môže MSAL použiť jeden alebo viacero overovacích tokov podporovaných platformou Microsoft Identity. Tieto toky môžu produkovať niekoľko typov tokenov a autorizačných kódov a vyžadovať rôzne tokeny, aby mohli pracovať.

3. **Prístupové tokeny**: [tokeny prístupu k platforme Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Zistite, ako môže vaše rozhranie API overiť a použiť nároky v accessovom tokene. Celá dokumentácia v tomto článku s výnimkou prípadov, keď je uvedené, sa vzťahuje len na tokeny vydané pre rozhrania API, ktoré ste zaregistrovali. Nevzťahuje sa na tokeny vydané pre rozhrania API vo vlastníctve spoločnosti Microsoft a nie je možné použiť tieto tokeny na overenie, akým spôsobom bude platforma Microsoft Identity vydávať tokeny pre vytvorené API.

**Ukončenie podpory pre knižnicu overovania služby Azure Active Directory (ADAL)**

- **Od 30. júna 2020,** už nebudeme pridávať žiadne nové funkcie do služby ADAL a Azure AD Graph. Naďalej budeme poskytovať technickú podporu a aktualizácie zabezpečenia, ale už nebudeme poskytovať aktualizácie funkcií.
- **Od 30. júna 2022,** ukončíme podporu pre ADAL a Azure AD Graph a už nebude poskytovať technickú podporu ani aktualizácie zabezpečenia.
- Aplikácie, ktoré používajú ADAL v existujúcich verziách operačného systému, budú fungovať aj po tomto čase, nebudú však *mať žiadne technické podpory ani aktualizácie zabezpečenia*.
- Aplikácie využívajúce Azure AD Graph po uplynutí tohto času už nemusia dostávať odpovede z koncového bodu služby Azure AD Graphu.

**Migrácia ADAL**

- Odporúčame aktualizáciu na MSAL, ktorá obsahuje najnovšie funkcie a aktualizácie zabezpečenia.
- Ak používate aplikácie spoločnosti Microsoft, viem, že spoločnosť Microsoft je v procese migrácie svojich aplikácií do MSAL podľa termínu ukončenia podpory, čím zabezpečí, že budú profitovať z priebežných vylepšení zabezpečenia a funkcií MSAL.

1. [Prečítajte si najčastejšie otázky o ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Zistite, ako migrovať aplikácie na základe jednotlivých platforiem](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Ak po prečítaní príručky pre platformu aplikácie máte ďalšie otázky, môžete uverejniť príspevok na [lokalite Microsoft Q&a](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) so značkou [Azure-AD-ADAL-odmietanie] alebo otvoriť problém v úložisku GitHub knižnice. Pozrite si časť [jazyky a rámce](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) v článku **Prehľad MSAL** pre prepojenia na repo služby jednotlivých knižníc.
4. **Ak potrebujete pomôcť s pochopením, ktoré z vašich aplikácií používajú ADAL**, odporúčame vám skontrolovať všetky zdrojové kódy aplikácií. Ak je to možné, Oslovte všetkých nezávislých dodávateľov softvéru (ISV) alebo poskytovateľov aplikácií. Podpora spoločnosti Microsoft vám tiež môže poskytnúť zoznam všetkých aplikácií v nájomníkovi, ktoré nie sú aplikácie ADAL od spoločnosti Microsoft.








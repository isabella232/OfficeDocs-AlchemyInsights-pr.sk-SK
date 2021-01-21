---
title: Konfigurovanie a predĺženie životnosti tokenov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917011"
---
# <a name="configure-and-extend-token-lifetimes"></a>Konfigurovanie a predĺženie životnosti tokenov

Môžete zadať životnosť tokenu Accessu, SAML alebo ID vydaného spoločnosťou Microsoft Identity Platform. Môžete nastaviť životnosť tokenov pre všetky aplikácie vo vašej organizácii, pre aplikáciu viacerých nájomníkov (multi-Organization) alebo pre konkrétnu službu v organizácii. Ďalšie informácie nájdete v téme [konfigurovateľné tokeny životnosti](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

Príklady si môžete prečítať v [téme ako nakonfigurovať životnosť tokenov](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

Ak chcete zistiť, ako nakonfigurovať životnosť a kompatibilitu tokenu v službe Azure Active Directory B2C (Azure AD B2C), pozrite si tému [Konfigurácia tokenov v službe Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

Článok [Konfigurácia správania relácie v službe Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) popisuje metódy jediného prihlásenia (SSO), ktoré sa používajú v službe Azure AD B2C, a pomáha vám pri konfigurácii politiky použiť NAJVHODNEJŠÍ spôsob SSO.

**Ako dlho trvajú tokeny? Ako dlho platia?**

Životnosť tokenov je 1 hodina a životnosť relácie je 24 hodín. To znamená, že ak sa nevykonajú žiadne žiadosti v priebehu 24 hodín, pred vyžiadaním nového tokenu sa budete musieť znova prihlásiť.

> [!NOTE]
> Po 30. mája 2020 bude mať žiadny nový nájomník možnosť použiť konfigurovateľné tokeny Lifetime Policy na konfiguráciu relácií a obnovenia tokenov. Nezhoda sa stane v priebehu niekoľkých mesiacov po tom, čo znamená, že zastavíme rešpektovanie existujúcich relácií a obnovenia tokenov polície. Životnosť tokenov prístupu môžete nakonfigurovať aj po uplynutí platnosti.







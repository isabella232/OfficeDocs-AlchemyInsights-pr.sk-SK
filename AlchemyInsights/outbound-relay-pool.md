---
title: Fond prenosu odchádzajúcich prenosov
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 8750c9036f258d9c5edc94bb027d564140bbd9914712cc1f25ff3abc3f4b9468
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54041601"
---
# <a name="outbound-relay-pool"></a>Fond prenosu odchádzajúcich prenosov

Spoločnosť Microsoft v konfigurácii robí určité zmeny týkajúce sa prenosu alebo preposielania e-mailov prostredníctvom Microsoft 365. Správy sa v určitých situáciách preposielajú alebo prenášajú Microsoft 365 prostredníctvom špeciálneho fondu prenosov. Správy odoslané pomocou fondu prenosu údajov môžu skončiť v priečinku nevyžiadanej pošty príjemcu. Ďalšie informácie nájdete v téme [Výstupné fondy doručovania](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Ak sa chcete vyhnúť scenáru používania fondu prenosov, uistite sa, že preposlané alebo presmerované správy spĺňajú jedno z nasledujúcich kritérií:

- Výstupný odosielateľ je akceptovaná doména nájomníka.
- SPF (Sender Policy Framework) prejde v čase, keď sa správa Microsoft 365.
- DomainKeys Identified Mail (DKIM) v doméne odosielateľa P2 prejde, keď sa správa Microsoft 365.
 
Správy, ktoré spĺňajú vyššie uvedené kritériá, nie sú prenášané prostredníctvom fondu prenosov.

Ak je MX záznam pre vašu doménu určený pre tretí alebo lokálny server, použite rozšírené filtrovanie, aby ste sa uistili, že pre prichádzajúce e-maily je správne overenie SPF, a vyhnete sa odosielaniu e-mailov prostredníctvom fondu prenosov.

**Ako zistiť, či je na nás vplyv fond prenosu?**

Ak preposlané alebo presmerované e-maily používajú jedno z vyššie uvedených kritérií, správy sa nebudú prenášať prostredníctvom fondu prenosov. Ak sa však správa odošle prostredníctvom fondu prenosu, IP server odchádzajúcej pošty je v rozsahu 40.95.0.0/16 a názov servera odchádzajúcej pošty obsahuje v názov **rly.**


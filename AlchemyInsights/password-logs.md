---
title: Denníky hesiel
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527181"
---
# <a name="password-logs"></a>Denníky hesiel

**Mám problémy s prístupom k denníkom auditu na vytvorenie nového hesla**

Ak chcete riešiť problémy týkajúce sa prístupu k denníkom auditu na vytvorenie nového hesla, vykonajte nasledujúci krok:

Uistite sa, že máte povolenie na zobrazenie denníkov auditu. 

Povolené sú len tieto roly:
 - Globálny správca
 - Správca zabezpečenia
 - Čítačka zabezpečenia

**Chcem Zobraziť všetky udalosti auditu obnovenia nového hesla od začiatku nasadeného času**

V zostavách za posledných 30 dní sú uložené až 120 000 heslá na vytvorenie nového hesla alebo udalosti registrácie. Tento maximálny limit sa vzťahuje na používateľské rozhranie pri sťahovaní súboru CSV. udalosti 1 000 000 sú k dispozícii v prostredí PowerShell.
Ďalšie informácie nájdete v prepojeniach nižšie:

- [Samoobslužné udalosti na vytvorenie nového hesla zo zostáv služby Azure AD a rozhrania API udalostí](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Ako stiahnuť nové heslo registrácia udalosti rýchlo s prostredím PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**Chcem sa dozvedieť viac o možnostiach vytvárania správ na vytvorenie nového hesla**

Skontrolujte, kto registruje alebo nastavuje heslá pomocou denníkov auditu obnovenia nového hesla Azure AD na portáli Azure v časti **Používatelia a skupiny**.
Ďalšie informácie nájdete v týchto prepojeniach:

- [Prehľad zostáv na vytvorenie nového hesla](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Zobrazenie zostáv na vytvorenie nového hesla na portáli Azure](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Samoobslužné udalosti na vytvorenie nového hesla zo zostáv služby Azure AD a rozhrania API udalostí](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Ako stiahnuť nové heslo registrácia udalosti rýchlo s prostredím PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)



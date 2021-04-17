---
title: Vytvorenie skupiny
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816387"
---
# <a name="create-a-group"></a>Vytvorenie skupiny

Táto téma popisuje vytváranie skupín.

**Povolenie na vytvorenie skupiny**

Uistite sa, že máte oprávnenie vytvoriť novú skupinu. Globálni správcovia môžu zakázať vytváranie skupín na portáli Azure alebo na paneli prístupu. Na vytvorenie novej skupiny alebo na zadanie príslušných povolení budete možno potrebovať správcu.

**Správa povolení na vytváranie skupín**

1. Globálni správcovia môžu spravovať povolenia na vytváranie skupín (z dôvodov zabezpečenia) alebo skupiny v Office 365 vytvorené na portáli Azure alebo na prístupnom paneli výberom možnosti Používatelia môžu vytvárať skupiny zabezpečenia na portáloch Azure alebo Možnosti Používatelia môžu vytvárať skupiny v Office 365 na portáloch Azure vo všetkých skupinách  >  **Všeobecné (Nastavenia).**
2. Môžete tiež obmedziť vytváranie skupín a vybrať skupinu používateľov, ak máte licenciu na Azure Active Directory P1 Premium.

**Vypnutie uvítacej oznámenia pre nových členov skupiny v Office 365**

Uvítacie oznámenie odoslané používateľom, ktorí sú pridaní do skupín v Office 365, možno vypnúť nastavením možnosti **UnifiedGroupWelcomeMessageEnabled** na hodnotu False v prostredí Powershell. Informácie o tomto nastavení nájdete [tu.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)


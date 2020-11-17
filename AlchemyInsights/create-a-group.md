---
title: Vytvorenie skupiny
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089175"
---
# <a name="create-a-group"></a>Vytvorenie skupiny

V tejto téme sa popisuje vytváranie skupín.

**Povolenie na vytvorenie skupiny**

Uistite sa, že máte oprávnenie na vytvorenie novej skupiny. Globálni správcovia môžu vypnúť vytváranie skupín na portáli Azure alebo v Accessovom paneli. Môže byť potrebné, aby správca vytvoril novú skupinu za vás alebo aby vám povolil príslušné povolenia.

**Správa povolení na vytváranie skupín**

1. Globálni správcovia môžu spravovať povolenia na vytváranie skupín (z dôvodov súvisiacich s bezpečnosťou) alebo skupiny služieb Office 365 vytvorené na portáli Azure alebo na prístupovom paneli výberom možnosti používatelia môžu vytvárať skupiny zabezpečenia na azúrových portáloch alebo môžu používatelia 365 vytvárať skupiny v službe Azure Portal vo **všetkých**  >  **všeobecných skupinách (nastavenia)**.
2. Môžete tiež obmedziť vytváranie skupín a vybrať skupinu používateľov, ak máte licenciu na Azure Active Directory P1 Premium.

**Vypnutie uvítacieho oznámenia pre nových členov skupiny v Office 365**

Uvítacia notifikácia odoslaná používateľom, ktorí boli pridaní do skupín služieb Office 365, môže byť zakázaná nastavením **UnifiedGroupWelcomeMessageEnabled** na hodnotu False v prostredí PowerShell. Oboznámte sa s týmto nastavením [tu](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).


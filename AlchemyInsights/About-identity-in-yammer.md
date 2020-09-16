---
title: Informácie o identite v Yammeri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664185"
---
# <a name="about-identity-in-yammer"></a>Informácie o identite v Yammeri

Odporúča sa, aby všetky siete vychádzali z nasledujúcich krokov, aby sa predišlo problémom s identitou:

1. Vynútenie identity balíka Office 365 po zriadení konta Microsoft 365 pre používateľov v službe Azure AD na zabezpečenie toho, aby sa všetci používatelia prihlásili pomocou svojho primárneho konta Microsoft 365. Ďalšie informácie nájdete v téme [vynútenie identity balíka Office 365 pre používateľov yammera](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Zlúčenie viacerých sietí Yammera. Staršie konfigurácie Yammera povoľujú pripojenie viacerých sietí siete Yammer k jednému nájomníkovi. Ďalšie informácie nájdete v téme [migrácia siete – zlúčenie viacerých sietí yammera](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Voliteľne môžete vynútiť licencie pre Yammer na blokovanie používateľov z Yammera, ak nemajú licenciu. Ďalšie informácie nájdete v téme [Správa používateľských licencií yammera v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Nakoniec auditovanie zoznamu používateľov pre staršie siete Yammer a pozastavenie starších používateľov. Namiesto ich odstránenia sa odporúča pozastaviť (deaktivovať) používateľov, pretože odstránenie je nezvratné. Ďalšie informácie nájdete v téme [auditovanie používateľov yammera v sieťach pripojených k Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) a [odstraňovanie používateľov](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Konfiguráciou Yammera pomocou týchto krokov budete tiež pripravení na konfiguráciu siete Yammer pre natívny režim pre Microsoft 365. Ďalšie informácie nájdete v téme [Konfigurácia siete Yammer pre natívny režim pre Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).
---
title: Informácie o identite v Yammeri
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148303"
---
# <a name="about-identity-in-yammer"></a>Informácie o identite v Yammeri

Odporúča sa, aby všetky siete prijali nasledujúce kroky, aby sa zabránilo otázkam súvisiacim s identitou:

1. Vynútenie identity služieb Office 365 po poskytnutí kont Microsoft 365 pre používateľov v službe Azure AD, aby ste sa uistili, že sa všetci používatelia prihlasujú pomocou primárneho konta Microsoft 365. Ďalšie informácie nájdete v téme [Vynútenie identity služieb Office 365 pre používateľov yammera](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).
2. Konsolidujte viaceré siete Yammer. Staršie konfigurácie yammera umožňujú pripojenie viacerých sietí Yammer k jednému nájomníkovi. Ďalšie informácie nájdete v téme [Migrácia siete – konsolidácia viacerých sietí Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).
3. Voliteľne vynútiť licencovanie pre Yammer blokovať používateľov z Yammer, ak nemajú licenciu. Ďalšie informácie nájdete v téme [Správa používateľských licencií yammera v službách Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).
4. Nakoniec auditovať zoznam používateľov starších sietí Yammer a pozastaviť starších používateľov. Odporúča sa, aby ste namiesto ich odstránenia pozastavili (deaktivovali) používateľov, pretože odstránenie je nezvratné. Ďalšie informácie nájdete [v témach Auditovanie používateľov Yammera v sieťach pripojených k službám Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) a [Odstránenie používateľov](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).

Konfigurácia Yammerpomocou týchto krokov, budete tiež pripravení nakonfigurovať sieť Yammer pre natívny režim pre Microsoft 365. Ďalšie informácie nájdete v téme [Konfigurácia siete Yammer pre natívny režim pre microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).
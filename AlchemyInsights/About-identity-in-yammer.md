---
title: Informácie o identite vo Yammer
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
ms.openlocfilehash: 57e7e6328747fc05b89799d631b2c6d7e0056547253aa3d75cdecb38cea3ad7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918952"
---
# <a name="about-identity-in-yammer"></a>Informácie o identite vo Yammer

Odporúča sa, aby všetky siete podnikli nasledovné kroky, aby sa zabránilo problémom súvisiacim s identitou:

1. Vynútenie Office 365 identity po poskytnutí Microsoft 365 pre používateľov v Azure AD, aby ste zabezpečili, že sa všetci používatelia prihlásia pomocou svojho primárneho Microsoft 365 konta. Ďalšie informácie nájdete v téme [Vynútenie Office 365 identity používateľov Yammer používateľov.](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)
2. Zlúčenie viacerých Yammer sietí. Staršie Yammer pripojenia umožňujú pripojenie Yammer viacerých Yammer k jedného nájomníkovi. Ďalšie informácie nájdete v téme [Migrácia siete – zlúčenie viacerých Yammer sietí.](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)
3. Prípadne vynútenie licencovania pre Yammer, ktoré zablokuje používateľom Yammer používateľom, ak nemajú licenciu. Ďalšie informácie nájdete v téme [Spravovanie Yammer používateľských licencií v Office 365.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)
4. Nakoniec pre audit zoznamu používateľov pre staršie Yammer a pozastavovanie starších používateľov. Odporúča sa pozastaviť (deaktivovať) používateľov namiesto ich odstránenia, pretože odstránenie je nezvratné. Ďalšie informácie nájdete v téme [Kontrola Yammer používateľov v sieťach pripojených k Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) a Odstránenie [používateľov.](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users)

Konfiguráciou Yammer pomocou týchto krokov tiež budete pripravení nakonfigurovať sieť Yammer pre natívny režim pre Microsoft 365. Ďalšie informácie nájdete v téme [Konfigurácia Yammer siete natívneho režimu pre Microsoft 365.](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)
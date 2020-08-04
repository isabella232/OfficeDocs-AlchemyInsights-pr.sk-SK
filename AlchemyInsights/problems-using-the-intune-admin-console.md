---
title: Problémy s používaním správcovskej konzoly Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555877"
---
# <a name="problems-using-the-intune-admin-console"></a>Problémy s používaním správcovskej konzoly Intune

**"Prístup odmietnutý" pri navigácii portálu na správu Intune.**

- Ak ste členom vlastnej roly Intune, uistite sa, že licenciu Intune alebo Enterprise Mobility Suite (EMS) je priradená k vášmu účtu.
- Ak používate Configuration Manager spravovať zariadenia, skontrolujte, či nie ste súčasťou kolekcie používateľov Intune Configuration Manager MDM.
- Overte, či vám boli priradené príslušné povolenia na správu na základe rolí (RBAC) v blade rolí Intune.
- Overte, či použitá skupina nie je distribučný zoznam. Intune na portáli Azure podporuje iba používateľské kontá, ktoré patria do skupín zabezpečenia Azure Active Directory. Skontrolujte skupiny na portáli Azure > **Skupiny Intune**  >  **Groups**alebo na portáli Azure > Azure **Active Directory**.

**Používateľ má príliš veľa povolení pre priradenú rolu Intune**

Učte používateľa, aby **prejsť na Intune**  >  **Intune**  >  **roly Moje povolenia**  >  **Export** na kontrolu udelených povolení.

**Skupina rozsahu bola pridaná do roly, ale používatelia v tejto roli stále vidia iných používateľov alebo zariadenia.**

Skupiny rozsahov nefiltruje používateľov alebo zariadenia. Skupiny rozsahu:

- Obmedzte používateľov, komu môžu priraďovať politiky alebo aplikácie.
- Povoliť spustenie vzdialených úloh v zariadeniach iba konkrétnym používateľom.

Ďalšie informácie o skupinách rozsahov nájdete v téme [Riadenie prístupu založené na rolách (RBAC) s programom Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Pridal som užívateľa do úlohy Intune, ale stále majú plný prístup k Admin Console Intune.**

Prejdite na Intune > **používateľov** na portáli Azure a overte, či používateľ nie je priradený žiadne z nasledujúcich rolí na portáli Azure:

- Globálny správca
- Správca služby Intune
- Správca služby SharePoint

Ďalšie informácie nájdete v téme [Riadenie prístupu založené na rolách (RBAC) s microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Problémy s prístupom**

Ďalšie informácie nájdete v téme [Nemôžete sa prihlásiť do služieb Office 365, Azure alebo Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).
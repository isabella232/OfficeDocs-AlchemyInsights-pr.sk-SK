---
title: Viacerí používatelia získajú chybu prístup odmietnutý pri pridávaní doplnkov v programe Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424174"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>Viacerí používatelia získajú chybu prístup odmietnutý pri pridávaní doplnkov v programe Outlook

Môžete určiť, ktorí správcovia vo vašej organizácii majú povolenia na inštaláciu a správu doplnkov pre program Outlook. Môžete tiež určiť, ktorí používatelia vo vašej organizácii majú povolenie na inštaláciu a správu doplnkov pre vlastné použitie.

Podrobnosti nájdete v [téme Určenie správcov a používateľov, ktorí môžu inštalovať a spravovať doplnky pre program Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

Ak chcete overiť, či ste úspešne priradili povolenia pre používateľa, nahraďte názov roly na overenie a spustite nasledujúci príkaz v <Role Name> prostredí Exchange Online PowerShell:

Získajte ManagementRoleAssignment -Úloha " <Role Name> " - GetEffectiveUsers

V tomto príklade sa uvádza, ako overiť, komu ste priradili povolenia na inštaláciu doplnkov z Office Obchodu pre organizáciu.

Powershell

-Role "Org Marketplace Apps" -GetEffectiveUsers

Vo výsledkoch Get-ManagementRoleAssignment, skontrolujte položky v stĺpci Efektívni používatelia.

Podrobné informácie o syntaxi a parametroch nájdete [v téme Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).
 
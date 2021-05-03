---
title: Nasadenie doplnkov pre Aplikácie Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125685"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Nasadenie doplnkov pre Aplikácie Microsoft 365

Centralizované nasadenie je odporúčaným spôsobom nasadenia Office používateľom a skupinám vo vašej organizácii. Ak chcete nasadiť doplnky, postupujte podľa nasledujúcich krokov:

**Poznámka:** Ak chcete inštalovať doplnky pre Office ako jednotliví používateľ, pozrite si časť Zobrazenie, spravovanie a inštalácia doplnkov [Office programoch.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Takisto sa uistite, že je Office povolený individuálne získavanie doplnkov z Office Obchod. 

1. Uistite sa, že vaše prostredie spĺňa požiadavky na nasadenie doplnkov pomocou funkcie Centralizované nasadenie. Podrobnosti nájdete v téme [Požiadavky.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)
2. Ak chcete **Nastavenia,** prejdite do časti Nastavenia Integrated Apps Get apps (Získať aplikácie s integrovanými aplikáciami) v centre spravovania služby  >    >   Microsoft 365 pre správcov. 

Poznámky: 

- Integrované aplikácie vyžadujú, aby správca získal povolenia globálneho správcu Exchange správcu.

- Pri nasadzovaní doplnkov viacerým používateľom odporúčame priraďovanie pomocou skupín namiesto jednotlivých používateľov. Podrobnosti nájdete v [téme Dôležité informácie pri priraďovaní doplnku používateľom a skupinám.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Centralizované nasadenie nepodporuje používateľov vo vnorených skupinách ani skupinách, ktoré majú nadradené skupiny. Podrobnosti nájdete v téme [Priradenia používateľov a skupín.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Skontrolujte, či je služba správy aplikácií pre Microsoft 365 (GUID: 0517ffae-825d-4aff-999e-3f2336b8a20a) povolená pre používateľov na prihlásenie. Podrobnosti nájdete v téme [Konfigurácia vlastností aplikácie.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Ak sa vyskytnú problémy s nasadením doplnkov pomocou funkcie Integrované aplikácie, skúste ich nasadiť [pomocou doplnkov.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Ďalšie informácie nájdete v téme:

[Nasadenie doplnkov v Centre spravovania](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Spravovanie doplnkov v Centre spravovania](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Použitie rutín typu cmdlet prostredia PowerShell funkcie Centralizované](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) nasadenie na spravovanie doplnkov 
 [Publikovanie Office pomocou funkcie Centralizované nasadenie prostredníctvom Centra Microsoft 365 spravovania](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Riešenie problémov: Používateľovi sa doplnky nevidí](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Riešenie chýb používateľa Office inými doplnokmi](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)
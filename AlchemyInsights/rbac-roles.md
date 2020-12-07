---
title: 'Roly RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583952"
---
# <a name="rbac-rules"></a>Pravidlá RBAC

Ak sa zobrazí chyba povolenia: 

- **Klient s identifikáciou objektu nemá povolenie na vykonávanie akcie nad rozsahom (kód: AuthorizationFailed)**: pri pokuse o vytvorenie zdroja Skontrolujte, či ste momentálne prihlásení pomocou používateľa, ktorému je priradená rola, ktorá má k zdroju povolenie zapisovať vo vybratom rozsahu. Ak chcete napríklad spravovať virtuálne počítače v skupine zdrojov, mali by ste mať rolu [prispievateľa virtuálneho zariadenia](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) v skupine zdrojov (alebo nadradenom rozsahu). Zoznam povolení pre každú vstavanú rolu nájdete [v téme vstavané roly Azure zdrojov](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Nemáte povolenie na vytvorenie žiadosti o podporu**: pri pokuse o vytvorenie alebo aktualizáciu lístka technickej podpory Skontrolujte, či ste v súčasnosti prihlásení pomocou používateľa, ktorému je priradená rola s povolením Microsoft. support/supportTickets/write, ako je napríklad [prispievateľ žiadosti o podporu](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Nie je možné vytvoriť ďalšie priradenia rolí (kód: RoleAssignmentLimitExceeded)**: pri pokuse o priradenie roly skúste znížiť počet priradení rolí priradením rolí k skupinám. Azure podporuje priradenia rolí až **2000** na predplatné.

Ďalšie informácie o rolách v službe Azure RBAC nájdete v téme roly v službe [Azure RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

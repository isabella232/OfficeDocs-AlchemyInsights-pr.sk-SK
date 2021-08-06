---
title: 'Roly pre roly na roly na základe rol '
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
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923146"
---
# <a name="rbac-rules"></a>Pravidlá pre RBAC

Ak sa zobrazí chyba povolenia: 

- Klient s id objektu nemá oprávnenie na vykonanie akcie v rozsahu **(kód: AutorizačnéFailed):** pri pokuse o vytvorenie zdroja skontrolujte, či ste momentálne prihlásení s používateľom, ktorý má priradenú rolu s povolením na zápis k zdroju vo vybratom rozsahu. Ak chcete napríklad spravovať virtuálne počítače v skupine zdrojov, mali by ste mať rolu [Prispievateľ](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) virtuálneho počítača v skupine zdrojov (alebo nadradenom rozsahu). Zoznam povolení pre každú vstavanú rolu nájdete v téme Vstavané [roly pre zdroje Azure.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Nemáte **povolenie** na vytvorenie žiadosti o podporu: pri pokuse o vytvorenie alebo aktualizáciu žiadosti o podporu skontrolujte, či ste momentálne prihlásení s používateľom, ktorý má priradenú rolu s povolením Microsoft.Support/supportTickets/write, napríklad s prispievateľom v [žiadosti](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)o podporu.
- Nie je možné vytvoriť žiadne ďalšie priradenia rolí **(kód: RoleAssignmentLimitExceeded):** keď sa pokúsite priradiť rolu, pokúste sa znížiť počet priradení rolí priradením rolí k skupinám. Azure podporuje až **2 000 priradení** rolí na jedno predplatné.

Ďalšie informácie o rolách rolí rolí pre roly rolí na základe rolí rolí rolí na základe rolí v službe Azure RBAC nájdete v téme [Roly pre roly na základe rolí rolí na](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)základe

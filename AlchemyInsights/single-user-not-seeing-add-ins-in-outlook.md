---
title: V programe Outlook sa nezobrazujú doplnky pre jedného používateľa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198219"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>V programe Outlook sa nezobrazujú doplnky pre jedného používateľa

Používateľ môže byť súčasťou roly, ktorá nemá správny parameter AppsForOfficeEnabled. Spustite tento cmdlet zistiť, či je k používateľovi priradená správna rola:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegovanie $false | Formát-tabuľka -automatická úloha,RoleAssigneeName,RoleAssigneeType

Ďalšie informácie nájdete v téme [Určenie správcov a používateľov, ktorí môžu inštalovať a spravovať doplnky pre program Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).

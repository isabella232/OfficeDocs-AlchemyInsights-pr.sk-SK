---
title: Viacerí používatelia v programe Outlook nevidia doplnky
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
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198241"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Viacerí používatelia v programe Outlook nevidia doplnky

Ak testujete doplnky programu Outlook a žiadne zobraziť, ako prvý krok riešenia problémov, pomocou rutiny cmdlet prostredia PowerShell **Get-OrganizationConfig** dotaz _AppsForOfficeEnabled_ parameter. Ak dotaz vráti hodnotu **False**, nastavte tento parameter na **hodnotu True** pomocou rutiny cmdlet **Set-OrganizationConfig,** takže doplnky sa zobrazia podľa očakávania.

Neodporúčame, aby bol parameter _AppsForOfficeEnabled_ nastavený na **hodnotu False**. Hodnota **False** prepíše všetky vyššie uvedené nastavenia správcovskej a používateľskej roly a zabraňuje aktivácii všetkých nových aplikácií ktorýmkoľvek používateľom v organizácii.

Ďalšie informácie sa nachádzajú v téme [Určenie správcov a používateľov, ktorí môžu inštalovať a spravovať doplnky pre program Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).
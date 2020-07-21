---
title: Odstránenie osamoteného používateľa z lokálneho servera
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198588"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Odstránenie osamoteného používateľa z lokálneho servera

Ak chcete odstrániť osamoteného používateľa, postupujte nasledovne:

1. Vynútiť synchronizáciu adresárov podľa pokynov v časti [Čo je hybridná identita služby Azure Active Directory?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Ak chcete overiť synchronizáciu adresárov, pozrite si [tému Čo je hybridná identita služby Azure Active Directory?](https://technet.microsoft.com/library/jj151797.aspx).

3. Ak synchronizácia funguje správne, ale odstránenie objektu služby Active Directory nerozšíri Azure AD, manuálne odstrániť osamotený objekt pomocou jedného z nasledujúcich Azure Active Directory modul pre rutiny cmdlet prostredia Windows PowerShell:

    Odstrániť MsolContact  
    Odstrániť MsolGroup  
    Odstrániť MsolUser

    Ak napríklad chcete odstrániť osamotený john.smith@contoso.com identifikácie používateľa, pôvodne vytvorený pomocou synchronizácie adresárov, spustite rutinu cmdlet:

    Odstrániť MsolUser-UserPrincipalName John.Smith@Contoso.com
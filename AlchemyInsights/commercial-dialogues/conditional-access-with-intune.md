---
title: Používanie podmieneného prístupu s Intune
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6700002"
- "7680"
ms.openlocfilehash: 23afea21668191093d612d68ca6e9ab2a844f4a14977631d33f4fd956fc3c4e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005789"
---
# <a name="using-conditional-access-with-intune"></a>Používanie podmieneného prístupu s Intune

Používanie podmieneného prístupu so služby Intune vyžaduje 3 kroky:

- [Vytvorenie politiky dodržiavania súladu na definovanie nastavení, ktoré musia byť splnené skôr, ako sa zariadenie považuje za spĺňajúce súlad. Príklad: Zariadenie musí mať aspoň 6-číselný PIN kód, aby sa zariadenie považovalo za spĺňajúce súlad.](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [Vytvorenie politiky podmieneného prístupu určujúci, aké zdroje sú chránené a aké podmienky musia byť splnené na získanie prístupu k týmto zdrojom. Príklad: Zariadenie musí pred prístupom k podnikovým e-mailom spĺňať súlad.](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [Skontrolujte, či sú politiky dodržiavania súladu aj politiky podmieneného prístupu zamerané na požadované skupiny používateľov. Môže to vyžadovať vytvorenie konkrétnych skupín používateľov v Azure Active Directory.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[Ďalšie informácie...](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)

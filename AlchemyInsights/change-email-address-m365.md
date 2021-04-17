---
title: Zmena e-mailovej adresy skupiny v Microsoft 365 alebo Microsoft Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819095"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Zmena e-mailovej adresy skupiny v Microsoft 365 alebo Microsoft Teams

E-mailovú adresu skupiny v Microsoft 365 alebo Microsoft Teams môžete zmeniť pomocou [Centra spravovania služby Microsoft 365](https://admin.microsoft.com/) Stačí vybrať skupinu a potom položku @upraviť e-mailovú adresu.

Na zmenu primárnej SMTP adresy skupiny v Microsoft 365 alebo Teams môžete použiť aj nasledujúci príkaz EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Príklad:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

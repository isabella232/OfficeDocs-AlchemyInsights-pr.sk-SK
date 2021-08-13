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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995637"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Zmena e-mailovej adresy skupiny v Microsoft 365 alebo Microsoft Teams

E-mailovú adresu skupiny v Microsoft 365 alebo Microsoft Teams môžete zmeniť pomocou [Centra spravovania služby Microsoft 365](https://admin.microsoft.com/) Stačí vybrať skupinu a potom položku @upraviť e-mailovú adresu.

Na zmenu primárnej SMTP adresy skupiny v Microsoft 365 alebo Teams môžete použiť aj nasledujúci príkaz EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Príklad:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

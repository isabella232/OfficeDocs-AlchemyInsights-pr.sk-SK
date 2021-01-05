---
title: Zmena e-mailovej adresy skupiny v Microsoft 365 alebo Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756572"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Zmena e-mailovej adresy skupiny v Microsoft 365 alebo Microsoft Teams

E-mailovú adresu skupiny v Microsoft 365 alebo Microsoft Teams môžete zmeniť pomocou [Centra spravovania služby Microsoft 365](https://admin.microsoft.com/) Stačí vybrať skupinu a potom položku @upraviť e-mailovú adresu.

Na zmenu primárnej SMTP adresy skupiny v Microsoft 365 alebo Teams môžete použiť aj nasledujúci príkaz EXO PowerShell:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Príklad:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`

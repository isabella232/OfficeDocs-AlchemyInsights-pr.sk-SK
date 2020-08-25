---
title: Odoslať ako skupinu Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872150"
---
# <a name="send-as-microsoft-365-group"></a>Odoslať ako skupinu Microsoft 365

Môžete priradiť povolenia Odoslať ako na povolenie konkrétnych používateľov odosielať správy ako skupina Microsoft 365:  

1. Pripojte sa k službe Exchange Online PowerShell.  

2. Spustite nasledujúci príkaz:  

    Add-RecipientPermission `<GroupName>` -správca `<MailboxName>` -AccessRights SendAs

Ďalšie informácie nájdete v téme [povolenie členom odosielať ako alebo odosielať v mene skupiny](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).
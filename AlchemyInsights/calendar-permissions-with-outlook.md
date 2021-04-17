---
title: Povolenia pre kalendár
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819923"
---
# <a name="calendar-permissions"></a>Povolenia pre kalendár

Používatelia môžu zmeniť svoje vlastné povolenia pre kalendár v Outlooku na webe alebo u iných klientov, ale ako správca budete musieť preskúmať aj vy.  
Pomocou rutiny typu cmdlet prostredia Exchange PowerShell získate povolenie pre kalendár používateľa:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Ďalšie informácie nájdete v týchto téme:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Povolenia pre kalendár sa používajú na zdieľanie kalendárov a ďalšie informácie o zdieľaní kalendára Outlooku nájdete v týchto článkoch:

- [Zdieľanie outlookového kalendára s inými osobami](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Zdieľanie kalendára v Outlooku na webe pre podniky](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Na riešenie problémov s povolením kalendára môžete [použiť nástroj Support and Recovery Assistant.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)
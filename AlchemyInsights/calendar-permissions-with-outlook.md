---
title: Povolenia kalendára
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748808"
---
# <a name="calendar-permissions"></a>Povolenia kalendára

Používatelia môžu zmeniť vlastné povolenia kalendára v Outlooku na webe alebo v iných klientoch, ale ako správca budete musieť tiež skúmať.  
Pomocou rutiny typu cmdlet prostredia PowerShell sa vám zobrazí povolenie v kalendári používateľa:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Ďalšie informácie nájdete v týchto témach:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Povolenia kalendára sa používajú pri zdieľaní kalendárov, ak chcete zobraziť ďalšie informácie o zdieľaní outlookového kalendára, prečítajte si tieto články:

- [Zdieľanie outlookového kalendára s inými osobami](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Zdieľanie kalendára v Outlooku na webe pre podniky](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Na riešenie problémov s povolením kalendára môžete použiť nástroj [support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .
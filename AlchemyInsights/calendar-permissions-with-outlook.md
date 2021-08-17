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
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046119"
---
# <a name="calendar-permissions"></a>Povolenia pre kalendár

Používatelia môžu zmeniť svoje vlastné povolenia pre kalendár Outlook na webe alebo iných klientoch, ale ako správca budete musieť preskúmať aj vy.  
Pomocou Exchange rutiny typu cmdlet prostredia PowerShell zobrazíte povolenie pre kalendár používateľa:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Ďalšie informácie nájdete v týchto téme:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Povolenia pre kalendár sa používajú na zdieľanie kalendárov a ďalšie informácie o zdieľaní kalendára Outlook nájdete v týchto článkoch:

- [Zdieľanie outlookového kalendára s inými osobami](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Zdieľanie kalendára v Outlook na webe for business](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Na riešenie problémov s povolením kalendára môžete [použiť nástroj Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) kalendár.
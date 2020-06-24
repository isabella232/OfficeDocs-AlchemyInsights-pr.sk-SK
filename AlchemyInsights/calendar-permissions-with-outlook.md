---
title: Povolenia kalendára
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862168"
---
# <a name="calendar-permissions"></a>Povolenia kalendára

Používatelia môžu zmeniť svoje vlastné povolenia kalendára pomocou programu Outlook na webe alebo iných klientov, ale ako správca možno budete musieť preskúmať tiež.  
Pomocou rutiny cmdlet prostredia Exchange PowerShell sa zobrazí povolenie v kalendári používateľa:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Ďalšie informácie nájdete v nasledujúcich témach:

- [Získať MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Nastaviť MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Pridať MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Povolenia kalendára sa používajú pri zdieľaní kalendárov, ak chcete zobraziť ďalšie informácie o zdieľaní kalendára programu Outlook, pozrite si tieto články:

- [Zdieľanie outlookového kalendára s inými osobami](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Zdieľanie kalendára v Outlooku na webe pre podniky](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Ak chcete riešiť problémy s povolením kalendára, môžete použiť nástroj [Support and Recovery Assistant.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)
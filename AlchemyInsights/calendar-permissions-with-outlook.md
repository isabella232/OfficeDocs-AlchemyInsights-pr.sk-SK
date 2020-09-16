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
# <a name="calendar-permissions"></a><span data-ttu-id="1e37f-102">Povolenia kalendára</span><span class="sxs-lookup"><span data-stu-id="1e37f-102">Calendar Permissions</span></span>

<span data-ttu-id="1e37f-103">Používatelia môžu zmeniť vlastné povolenia kalendára v Outlooku na webe alebo v iných klientoch, ale ako správca budete musieť tiež skúmať.</span><span class="sxs-lookup"><span data-stu-id="1e37f-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="1e37f-104">Pomocou rutiny typu cmdlet prostredia PowerShell sa vám zobrazí povolenie v kalendári používateľa:</span><span class="sxs-lookup"><span data-stu-id="1e37f-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="1e37f-105">Ďalšie informácie nájdete v týchto témach:</span><span class="sxs-lookup"><span data-stu-id="1e37f-105">To see more information see the following:</span></span>

- [<span data-ttu-id="1e37f-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="1e37f-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="1e37f-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="1e37f-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="1e37f-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="1e37f-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="1e37f-109">Povolenia kalendára sa používajú pri zdieľaní kalendárov, ak chcete zobraziť ďalšie informácie o zdieľaní outlookového kalendára, prečítajte si tieto články:</span><span class="sxs-lookup"><span data-stu-id="1e37f-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="1e37f-110">Zdieľanie outlookového kalendára s inými osobami</span><span class="sxs-lookup"><span data-stu-id="1e37f-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="1e37f-111">Zdieľanie kalendára v Outlooku na webe pre podniky</span><span class="sxs-lookup"><span data-stu-id="1e37f-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="1e37f-112">Na riešenie problémov s povolením kalendára môžete použiť nástroj [support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="1e37f-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>
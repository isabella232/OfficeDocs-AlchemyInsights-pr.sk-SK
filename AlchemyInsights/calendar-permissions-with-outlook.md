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
# <a name="calendar-permissions"></a><span data-ttu-id="69b68-102">Povolenia pre kalendár</span><span class="sxs-lookup"><span data-stu-id="69b68-102">Calendar Permissions</span></span>

<span data-ttu-id="69b68-103">Používatelia môžu zmeniť svoje vlastné povolenia pre kalendár v Outlooku na webe alebo u iných klientov, ale ako správca budete musieť preskúmať aj vy.</span><span class="sxs-lookup"><span data-stu-id="69b68-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="69b68-104">Pomocou rutiny typu cmdlet prostredia Exchange PowerShell získate povolenie pre kalendár používateľa:</span><span class="sxs-lookup"><span data-stu-id="69b68-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="69b68-105">Ďalšie informácie nájdete v týchto téme:</span><span class="sxs-lookup"><span data-stu-id="69b68-105">To see more information see the following:</span></span>

- [<span data-ttu-id="69b68-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="69b68-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="69b68-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="69b68-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="69b68-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="69b68-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="69b68-109">Povolenia pre kalendár sa používajú na zdieľanie kalendárov a ďalšie informácie o zdieľaní kalendára Outlooku nájdete v týchto článkoch:</span><span class="sxs-lookup"><span data-stu-id="69b68-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="69b68-110">Zdieľanie outlookového kalendára s inými osobami</span><span class="sxs-lookup"><span data-stu-id="69b68-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="69b68-111">Zdieľanie kalendára v Outlooku na webe pre podniky</span><span class="sxs-lookup"><span data-stu-id="69b68-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="69b68-112">Na riešenie problémov s povolením kalendára môžete [použiť nástroj Support and Recovery Assistant.](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)</span><span class="sxs-lookup"><span data-stu-id="69b68-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>
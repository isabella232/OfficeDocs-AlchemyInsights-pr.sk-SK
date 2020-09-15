---
title: Riešenie problémov s doručovaním e-mailov do verejných priečinkov s podporou e-mailu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: da35ae4bd911fb75f23cc1c99aacbaa2392425dd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677943"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="a622f-102">Riešenie problémov s doručovaním e-mailov do verejných priečinkov s podporou e-mailu</span><span class="sxs-lookup"><span data-stu-id="a622f-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="a622f-103">Ak externí odosielatelia nedokážu odosielať správy do verejných priečinkov s podporou e-mailu a odosielateľom sa zobrazí chyba: **Nepodarilo sa nájsť (550 5.4.1)**, overte, či je doména e-mailu pre verejný priečinok nakonfigurovaná ako doména interného prenosu namiesto smerodajnej domény:</span><span class="sxs-lookup"><span data-stu-id="a622f-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="a622f-104">Otvorte [centrum spravovania pre Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="a622f-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="a622f-105">Prejdite na **Mail flow** položku \> **akceptované domény**toku pošty, vyberte akceptovanú doménu a potom kliknite na položku **Upraviť**.</span><span class="sxs-lookup"><span data-stu-id="a622f-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="a622f-106">Na stránke vlastnosti, ktorá sa otvorí, ak je typ domény nastavený na hodnotu **autoritatívne**, zmeňte hodnotu na **interný prenos** a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="a622f-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="a622f-107">Ak externým odosielateľom sa zobrazí chyba, **ktorú nemáte povolenie (550 5.7.13)**, spustite nasledujúci príkaz v [prostredí Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) a zobrazte povolenia anonymných používateľov vo verejnom priečinku:</span><span class="sxs-lookup"><span data-stu-id="a622f-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="a622f-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Napríklad `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="a622f-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="a622f-109">Ak chcete povoliť externým používateľom odosielať e-maily do tohto verejného priečinka, pridajte CreateItems prístup k používateľovi anonymné.</span><span class="sxs-lookup"><span data-stu-id="a622f-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="a622f-110">Napríklad `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="a622f-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>

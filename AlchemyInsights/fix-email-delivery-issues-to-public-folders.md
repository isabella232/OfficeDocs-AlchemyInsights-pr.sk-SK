---
title: Oprava problémov s doručením e-mailov verejným priečinkom s podporou e-mailu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716367"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="842e4-102">Oprava problémov s doručením e-mailov verejným priečinkom s podporou e-mailu</span><span class="sxs-lookup"><span data-stu-id="842e4-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="842e4-103">Ak externí odosielatelia nemôžu odosielať správy do verejných priečinkov s podporou e-mailu a odosielatelia dostanú chybu: **Nepodarilo sa nájsť (550 5.4.1)**, overte, či je doména e-mailu pre verejný priečinok nakonfigurovaná ako doména interného prenosu namiesto autoritatívnej domény:</span><span class="sxs-lookup"><span data-stu-id="842e4-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="842e4-104">Otvorte [Exchange Admin Center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="842e4-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="842e4-105">Prejsť na **mail flow** \> **akceptované**domény, vyberte akceptovanú doménu, a potom kliknite na tlačidlo **Upraviť**.</span><span class="sxs-lookup"><span data-stu-id="842e4-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="842e4-106">Na stránke vlastnosti, ktorá sa otvorí, ak je typ domény nastavený na **autoritatívny**, zmeňte hodnotu na **interný Relay** a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="842e4-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="842e4-107">Ak externí odosielatelia dostanú chybu nemáte **povolenie (550 5.7.13)**, spustite nasledujúci príkaz v [službe Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) vidieť povolenia pre anonymných používateľov vo verejnom priečinku:</span><span class="sxs-lookup"><span data-stu-id="842e4-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="842e4-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Napríklad `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="842e4-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="842e4-109">Umožniť externým používateľom odosielať e-maily do tohto verejného priečinka, pridajte CreateItems prístup právo na anonymný používateľ.</span><span class="sxs-lookup"><span data-stu-id="842e4-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="842e4-110">Napríklad `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="842e4-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>

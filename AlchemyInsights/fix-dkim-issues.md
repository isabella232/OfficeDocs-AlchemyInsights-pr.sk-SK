---
title: Riešenie problémov s nastavením DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717577"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="b5e78-102">Riešenie problémov s nastavením DKIM</span><span class="sxs-lookup"><span data-stu-id="b5e78-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="b5e78-103">Ak sa vyskytnú problémy umožňujúce DKIM pre vlastnú doménu, použite nasledovný postup:</span><span class="sxs-lookup"><span data-stu-id="b5e78-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="b5e78-104">Väčšina problémov s nastavením DKIM súvisí s nesprávnymi záznamami DNS.</span><span class="sxs-lookup"><span data-stu-id="b5e78-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="b5e78-105">Overte, či záznam DKIM CNAME (**nie** záznam TXT) je správne naformátovaný.</span><span class="sxs-lookup"><span data-stu-id="b5e78-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="b5e78-106">Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="b5e78-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="b5e78-107">Po vytvorení alebo aktualizácii záznamov DNS DKIM na hostiteľskú službu DNS pre vašu doménu (typicky, Registrátor domén), počkajte, kým sa záznamy DNS množiť.</span><span class="sxs-lookup"><span data-stu-id="b5e78-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="b5e78-108">Ak nemôžete vytvoriť DKIM DNS záznamy v admin Center, môžete \<nahradiť customdomain\> s vlastnou doménou (napríklad contoso.com) a spustiť tento príkaz v prostredí [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell):. `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`</span><span class="sxs-lookup"><span data-stu-id="b5e78-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>

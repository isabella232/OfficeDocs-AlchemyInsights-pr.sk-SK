---
title: Riešenie problémov s inštaláciou DKIM
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
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506789"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="470d1-102">Riešenie problémov s inštaláciou DKIM</span><span class="sxs-lookup"><span data-stu-id="470d1-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="470d1-103">Ak sa vyskytnú problémy umožňujúce DKIM pre vlastnú doménu, postupujte nasledovne:</span><span class="sxs-lookup"><span data-stu-id="470d1-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="470d1-104">Väčšina problémov s inštaláciou DKIM súvisí s nesprávnymi záznamami DNS.</span><span class="sxs-lookup"><span data-stu-id="470d1-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="470d1-105">Skontrolujte, či je záznam DKIM CNAME **(nie** TXT záznam) správne naformátovaný.</span><span class="sxs-lookup"><span data-stu-id="470d1-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="470d1-106">Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="470d1-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="470d1-107">Po vytvorení alebo aktualizácii záznamov DKIM DNS v hostiteľskej službe DNS pre vašu doménu (zvyčajne registrátora domén) počkajte na propagáciu záznamov DNS.</span><span class="sxs-lookup"><span data-stu-id="470d1-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="470d1-108">Ak nemôžete vytvoriť záznamy DKIM DNS v Centre spravovania, môžete nahradiť \<CustomDomain\> vlastnou doménou (napríklad contoso.com) a spustiť tento príkaz v [prostredí Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="470d1-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>

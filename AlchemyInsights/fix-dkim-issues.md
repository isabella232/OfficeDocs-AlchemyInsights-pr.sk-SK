---
title: Riešenie problémov s nastavením DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744965"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="fbf8a-102">Riešenie problémov s nastavením DKIM</span><span class="sxs-lookup"><span data-stu-id="fbf8a-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="fbf8a-103">Ak sa vyskytnú problémy s povolením DKIM pre vlastnú doménu, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="fbf8a-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="fbf8a-104">Väčšinu problémov s nastavením DKIM súvisia s nesprávnymi záznamami DNS.</span><span class="sxs-lookup"><span data-stu-id="fbf8a-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="fbf8a-105">Overte, či je záznam CNAME CNAME (**nie** txt záznam) naformátovaný správne.</span><span class="sxs-lookup"><span data-stu-id="fbf8a-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="fbf8a-106">Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="fbf8a-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="fbf8a-107">Po vytvorení alebo aktualizácii DNS záznamov v hostiteľskej službe DNS pre svoju doménu (zvyčajne registrátora domén) počkajte, kým sa DNS záznamy rozšíria.</span><span class="sxs-lookup"><span data-stu-id="fbf8a-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="fbf8a-108">Ak nie je možné vytvoriť DNS záznamy DKIM v centre spravovania, môžete nahradiť \<CustomDomain\> svoju vlastnú doménu (napríklad contoso.com) a spustiť tento príkaz v [prostredí Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="fbf8a-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>

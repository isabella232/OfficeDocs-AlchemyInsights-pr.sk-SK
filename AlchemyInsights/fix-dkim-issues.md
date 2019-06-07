---
title: Opraviť problémy s inštaláciou DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765395"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="4f55b-102">Opraviť problémy s inštaláciou DKIM</span><span class="sxs-lookup"><span data-stu-id="4f55b-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="4f55b-103">Ak sa vyskytnú problémy, umožňujúce DKIM pre vlastnú doménu, použite nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="4f55b-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="4f55b-104">Väčšina problémov s nastavením DKIM súvisia s nesprávne záznamy DNS.</span><span class="sxs-lookup"><span data-stu-id="4f55b-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="4f55b-105">Overte, či záznam DKIM CNAME (**nie** záznam TXT) je správne naformátované.</span><span class="sxs-lookup"><span data-stu-id="4f55b-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="4f55b-106">Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4f55b-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="4f55b-107">Po vytvorení alebo aktualizovať záznamy DKIM DNS v hostiteľskej služby DNS pre vašu doménu (zvyčajne registrátora domény), čakať na DNS záznamy na propagáciu.</span><span class="sxs-lookup"><span data-stu-id="4f55b-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="4f55b-108">Ak nemôžete vytvoriť DKIM DNS záznamy admin Center, môžete nahradiť \<CustomDomain\> s svoje vlastné domény (napríklad contoso.com) a spustite tento príkaz v [Online PowerShell výmeny](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="4f55b-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>

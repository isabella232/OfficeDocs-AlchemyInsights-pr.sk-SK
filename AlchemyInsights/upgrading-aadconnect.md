---
title: 932 inovácia AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766508"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="9d276-102">Inovácia Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="9d276-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="9d276-103">Predvolene je povolená Automatická inovácia pre Azure AD Connect, čo pomáha zabezpečiť, že používate najnovšiu verziu.</span><span class="sxs-lookup"><span data-stu-id="9d276-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="9d276-104">Ak chcete overiť nastavenie automatickej inovácie, použite rutiny cmdlet **Get-ADSyncAutoUpgrade** Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="9d276-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="9d276-105">Rutiny cmdlet vráti jednu z nasledujúcich hodnôt:</span><span class="sxs-lookup"><span data-stu-id="9d276-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="9d276-106">**Povolené**: Automatická inovácia je povolená.</span><span class="sxs-lookup"><span data-stu-id="9d276-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="9d276-107">**Vypnuté**: Automatická inovácia je vypnutá.</span><span class="sxs-lookup"><span data-stu-id="9d276-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="9d276-108">**Pozastavené**: systém už nie je spôsobilý prijímať automatické aktualizácie.</span><span class="sxs-lookup"><span data-stu-id="9d276-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="9d276-109">Túto hodnotu nie je možné nakonfigurovať. je nastavený systémom.</span><span class="sxs-lookup"><span data-stu-id="9d276-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="9d276-110">Ďalšie informácie nájdete v téme [Automatická inovácia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="9d276-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="9d276-111">Ak chcete prevziať najnovšiu verziu Azure AD Connect, prejdite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="9d276-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>

---
title: 932 inovácia AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365926"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="0acff-102">Aktualizácia Azure AD pripojenie</span><span class="sxs-lookup"><span data-stu-id="0acff-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="0acff-103">Podľa predvoleného nastavenia automatické aktualizácie zapnuté Azure AD pripojiť, ktorý pomáha zabezpečiť, že používate najnovšiu verziu.</span><span class="sxs-lookup"><span data-stu-id="0acff-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="0acff-104">Nastavenie automatického upgrade, pomocou Azure AD PowerShell cmdlet **Get-ADSyncAutoUpgrade** .</span><span class="sxs-lookup"><span data-stu-id="0acff-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="0acff-105">Rutiny cmdlet vráti niektorú z nasledujúcich hodnôt:</span><span class="sxs-lookup"><span data-stu-id="0acff-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="0acff-106">**Zapnuté**: Automatické aktualizácie zapnutá.</span><span class="sxs-lookup"><span data-stu-id="0acff-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="0acff-107">**Vypnuté**: Automatické aktualizácie je vypnuté.</span><span class="sxs-lookup"><span data-stu-id="0acff-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="0acff-108">**Zavesené**: systém už nie je oprávnený prijímať automatické aktualizácie.</span><span class="sxs-lookup"><span data-stu-id="0acff-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="0acff-109">Nemôžete konfigurovať túto hodnotu; nachádza sa v systéme.</span><span class="sxs-lookup"><span data-stu-id="0acff-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="0acff-110">Ďalšie informácie nájdete v [Automatické aktualizácie](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="0acff-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="0acff-111">Stiahnuť najnovšiu verziu Azure AD pripojenie, prejdite na [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="0acff-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>

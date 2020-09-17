---
title: 932 inovácia AADConnect
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
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806054"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="c2a64-102">Inovácia služby Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="c2a64-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="c2a64-103">Predvolene je povolená Automatická inovácia pre službu Azure AD Connect, ktorá pomáha zabezpečiť, že máte nainštalovanú najnovšiu verziu.</span><span class="sxs-lookup"><span data-stu-id="c2a64-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="c2a64-104">Ak chcete overiť nastavenia automatickej inovácie, použite rutinu typu cmdlet **Get-ADSyncAutoUpgrade** v prostredí Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="c2a64-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="c2a64-105">Rutina typu cmdlet vráti jednu z nasledujúcich hodnôt:</span><span class="sxs-lookup"><span data-stu-id="c2a64-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="c2a64-106">**Povolené**: Automatická inovácia je povolená.</span><span class="sxs-lookup"><span data-stu-id="c2a64-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="c2a64-107">**Vypnuté**: Automatická inovácia je zakázaná.</span><span class="sxs-lookup"><span data-stu-id="c2a64-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="c2a64-108">**Pozastavené**: systém už nie je oprávnený prijímať automatické inovácie.</span><span class="sxs-lookup"><span data-stu-id="c2a64-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="c2a64-109">Túto hodnotu nie je možné nakonfigurovať. je nastavený systémom.</span><span class="sxs-lookup"><span data-stu-id="c2a64-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="c2a64-110">Ďalšie informácie nájdete v téme [Automatická inovácia](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="c2a64-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="c2a64-111">Ak si chcete stiahnuť najnovšiu verziu služby Azure AD Connect, prejdite na položku [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="c2a64-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>

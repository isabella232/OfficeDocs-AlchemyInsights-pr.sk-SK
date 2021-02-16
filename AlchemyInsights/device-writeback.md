---
title: Zápisom zariadenia
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256967"
---
# <a name="device-writeback"></a><span data-ttu-id="55c63-102">Zápisom zariadenia</span><span class="sxs-lookup"><span data-stu-id="55c63-102">Device Writeback</span></span>

<span data-ttu-id="55c63-103">Zariadenie zápisom sa používa v nasledovných prípadoch:</span><span class="sxs-lookup"><span data-stu-id="55c63-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="55c63-104">Zapnutie [Windows Hello for Business s použitím nasadenia dôvery prostredníctvom hybridného certifikátu](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="55c63-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="55c63-105">Povolenie podmieneného prístupu na základe zariadení na chránené aplikácie ADFS (2012 R2 alebo novšia verzia) (spoliehanie sa na strany trustov)</span><span class="sxs-lookup"><span data-stu-id="55c63-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="55c63-106">Na zápisom zariadenia sa vyžaduje predplatné na Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="55c63-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="55c63-107">Táto akcia poskytuje ďalšie zabezpečenie a istotu, že prístup k aplikáciám sa udelí len pre dôveryhodné zariadenia.</span><span class="sxs-lookup"><span data-stu-id="55c63-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="55c63-108">Ďalšie informácie o podmienenom prístupe nájdete v téme [spravovanie rizika s podmieneným prístupom](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) a [Nastavenie lokálneho podmieneného prístupu pomocou registrácie zariadenia Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview).</span><span class="sxs-lookup"><span data-stu-id="55c63-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="55c63-109">Ďalšie informácie o povolení zariadenia zápisom pre zariadenia nájdete v téme [povolenie zariadenia zápisom](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span><span class="sxs-lookup"><span data-stu-id="55c63-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>

---
title: ;Riešenie problémov s pripojením k službe Hybrid Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401922"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="11c69-102">;Riešenie problémov s pripojením k službe Hybrid Azure AD</span><span class="sxs-lookup"><span data-stu-id="11c69-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="11c69-103">Dôrazne odporúčame zabezpečiť, aby zariadenie malo prístup ku koncovým bodom registrácie zariadenia v rámci systémového konta pomocou skriptu [Test Device Registration Connectivity](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="11c69-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="11c69-104">Ak nastavujete registrácie zariadení po prvýkrát, nezabudnite si prečítať tému [Úvod do správy zariadení v službe Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), v ktorej zistíte, ako kontrolovať zariadenia cez službu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="11c69-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="11c69-105">Ak svoje zariadenia registrujete priamo do služby Azure AD a zaregistrujete ich do služby Intune, uistite sa, že ste [nakonfigurovali službu Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) a máte potrebné [licencie](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="11c69-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="11c69-106">Uistite sa, že máte oprávnenie na vykonávanie operácií v službe Azure AD a lokálnej službe AD.</span><span class="sxs-lookup"><span data-stu-id="11c69-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="11c69-107">Nastavenia registrácií zariadení môže spravovať iba globálny správca v službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="11c69-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="11c69-108">Okrem toho, ak nastavujete automatické registrácie v lokálnej službe Active Directory, budete musieť byť správcom služby Active Directory a AD FS (ak je to potrebné).</span><span class="sxs-lookup"><span data-stu-id="11c69-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="11c69-109">Ďalšie podrobnosti o riešení potenciálnych problémov s pripojením Hybrid nájdete v téme [Riešenie problémov s pripojením Hybrid](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current), kde nájdete informácie o nastavení hybridného nasadenia služby Azure AD. Informácie o spravovaní zariadení pomocou portálu Azure Ad nájdete v témach [Nastavenie zariadení pripojených k službe Hybrid Azure AD (pripojených k lokálnej doméne)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) a [Správa zariadení pomocou portálu Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="11c69-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="11c69-110">Ak chcete vyriešiť bežné problémy s pripojením k službe Hybrid Azure Active Directory (AD), pozrite si tému [Najčastejšie otázky o pripojení k službe Hybrid Azure AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="11c69-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>

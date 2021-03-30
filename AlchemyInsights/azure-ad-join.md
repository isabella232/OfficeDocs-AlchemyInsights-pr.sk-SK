---
title: Pripojenie k službe Azure Active Directory
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405673"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="5057a-102">Pripojenie k službe Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="5057a-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="5057a-103">Ak nastavujete registráciu zariadenia po prvýkrát, uistite sa, že ste si už preskúmali úvodné informácie o riadení zariadení v [Azure Active Directory,](/azure/active-directory/devices/overview) kde nájdete postup, ako získať zariadenia pod kontrolou na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5057a-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="5057a-104">Ak svoje zariadenia zaregistrujete priamo v službe Azure AD a zaregistrujete ich do služby Intune, [](/mem/intune/fundamentals/licenses-assign) musíte sa najskôr ubezpečiť, že ste nakonfigurovali [službu Intune](/mem/intune/enrollment/device-enrollment) a že licencie máte nastavené.</span><span class="sxs-lookup"><span data-stu-id="5057a-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="5057a-105">Uistite sa, že máte oprávnenie vykonávať operácie v službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5057a-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="5057a-106">Nastavenia registrácií zariadenia môže spravovať iba globálny správca v službe Azure AD.</span><span class="sxs-lookup"><span data-stu-id="5057a-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="5057a-107">Informácie o implementácii spojenia so službou Azure AD nájdete v [téme Plánovanie pripájanie k službe Azure AD.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="5057a-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="5057a-108">Ďalšie informácie o riešení bežných problémov s pripojením k službe Azure AD nájdete v téme Najčastejšie otázky o službe [Azure Ad](/azure/active-directory/devices/faq) a pre zariadenie s Windowsom 10 Pro nájdete v téme Nedá sa pripojiť k počítaču [s Windowsom 10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)na Azure AD – je potrebné inovovať na – komunita Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5057a-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>

---
title: Problémy s licenciou Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657291"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="af53b-102">Problémy s licenciou Yammer</span><span class="sxs-lookup"><span data-stu-id="af53b-102">Yammer licensing issues</span></span>

<span data-ttu-id="af53b-103">Všetci používatelia musia mať licenciu na používanie podnikovej služby Yammer, ale predvolene Yammer nevyžaduje, aby mali používatelia licenciu na prístup k službe.</span><span class="sxs-lookup"><span data-stu-id="af53b-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="af53b-104">Keď správca zmení nastavenie tak, aby blokoval používateľov služieb Microsoft 365 bez licencií na Yammer, používatelia, ktorí nemajú priradenú licenciu na Yammer Enterprise, nemôžu získať prístup k službe Yammer.</span><span class="sxs-lookup"><span data-stu-id="af53b-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="af53b-105">Ďalšie informácie nájdete v téme [Správa používateľských licencií yammera v Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="af53b-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="af53b-106">Keď sa licencie odstránia od používateľov, dlaždica Yammer sa už nezobrazuje a ďalšie služby môžu pomocou odstraňovania licencií použiť na skrytie funkcií.</span><span class="sxs-lookup"><span data-stu-id="af53b-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="af53b-107">V iných prípadoch sa funkcie môžu naďalej zobrazovať, ale vyžadujú, aby sa na ňu vyžadovalo nasadenie licencií.</span><span class="sxs-lookup"><span data-stu-id="af53b-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="af53b-108">**Licencia sa používateľovi neaktualizuje**</span><span class="sxs-lookup"><span data-stu-id="af53b-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="af53b-109">Niekedy je používateľovi priradená licencia, ale stále nie je možné získať prístup k Yammeru.</span><span class="sxs-lookup"><span data-stu-id="af53b-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="af53b-110">Oneskorenie je pravdepodobnejšie, keď prebieha pridelenie hromadnej licencie.</span><span class="sxs-lookup"><span data-stu-id="af53b-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="af53b-111">Používatelia yammera sa nemusia aktualizovať v rovnakom poradí, v akom sa licencie zmenia v službe Azure AD, pretože systém funguje asynchrónne.</span><span class="sxs-lookup"><span data-stu-id="af53b-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="af53b-112">Počkajte až 24 hodín, kým sa neotvorí prípad podpory, aby sa nahlásili problémy so synchronizáciou licencií.</span><span class="sxs-lookup"><span data-stu-id="af53b-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="af53b-113">**Priradenie hromadnej licencie**</span><span class="sxs-lookup"><span data-stu-id="af53b-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="af53b-114">Licencie je možné priradiť prostredníctvom centra spravovania alebo skriptovania v prostredí PowerShell.</span><span class="sxs-lookup"><span data-stu-id="af53b-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="af53b-115">Ďalšie informácie nájdete v téme [Priradenie licencií používateľom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a [Priradenie licencií k používateľským kontám v prostredí Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="af53b-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="af53b-116">Technická podpora spoločnosti Microsoft neposkytuje pomoc pri vytváraní skriptov, ale dokumentácia o priradení licencií na Yammer je k dispozícii.</span><span class="sxs-lookup"><span data-stu-id="af53b-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="af53b-117">Ďalšie informácie nájdete v téme [Správa licencií na Yammer pomocou prostredia Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="af53b-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>
---
title: Problémy s licenciami yammera
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148320"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="b1d9c-102">Problémy s licenciami yammera</span><span class="sxs-lookup"><span data-stu-id="b1d9c-102">Yammer licensing issues</span></span>

<span data-ttu-id="b1d9c-103">Všetci používatelia musia mať licenciu na používanie služby Yammer Enterprise, ale v predvolenom nastavení sieť Yammer nevyžaduje, aby používatelia mali licenciu na prístup k službe.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="b1d9c-104">Keď správca zmení nastavenie blokovať Microsoft 365 používateľov bez licencií yammera, používatelia nie je priradená yammer Enterprise licencie nemôže získať prístup k službe Yammer.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="b1d9c-105">Ďalšie informácie nájdete v téme [Správa používateľských licencií Yammera v službách Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="b1d9c-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="b1d9c-106">Keď licencie sú odstránené od používateľov, yammer dlaždice sa už nezobrazuje a iné služby môžete použiť odstránenie licencie skryť funkcie.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="b1d9c-107">V ostatných prípadoch sa funkcie môžu stále zobrazovať, ale vyžadujú, aby licencia priradenie fungovalo.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="b1d9c-108">**Licencia sa neaktualizuje pre používateľa**</span><span class="sxs-lookup"><span data-stu-id="b1d9c-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="b1d9c-109">Niekedy používateľ je priradená licencia, ale stále nie je schopný získať prístup k sieti Yammer.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="b1d9c-110">Oneskorenia sú pravdepodobnejšie, že dôjde, keď prebieha hromadné priradenie licencie.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="b1d9c-111">Používatelia yammera nemusia byť aktualizované v rovnakom poradí ako licencie sa zmenia v Azure AD, pretože systém beží asynchrónne.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="b1d9c-112">Počkajte až 24 hodín pred otvorením prípadu technickej podpory na hlásenie problémov so synchronizáciou licencie.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="b1d9c-113">**Hromadné pridelenie licencie**</span><span class="sxs-lookup"><span data-stu-id="b1d9c-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="b1d9c-114">Licencie je možné priradiť prostredníctvom centra spravovania alebo skriptovania prostredia PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="b1d9c-115">Ďalšie informácie nájdete v [témach Priradenie licencií používateľom](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) a [Priradenie licencií k používateľským kontám pomocou prostredia PowerShell služieb Office 365](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="b1d9c-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="b1d9c-116">Technická podpora spoločnosti Microsoft neposkytuje pomoc pri vytváraní skriptov, ale k dispozícii je dokumentácia o priradení licencie yammera.</span><span class="sxs-lookup"><span data-stu-id="b1d9c-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="b1d9c-117">Ďalšie informácie nájdete v téme [Správa licencií yammera pomocou prostredia Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="b1d9c-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>
---
title: Office sa nedá aktivovať
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812587"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="59473-102">Office sa nedá aktivovať</span><span class="sxs-lookup"><span data-stu-id="59473-102">Unable to activate Office</span></span>

- <span data-ttu-id="59473-103">Skontrolujte, či vám neuplynula platnosť predplatného.</span><span class="sxs-lookup"><span data-stu-id="59473-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="59473-104">Uistite sa, že máte predplatné, ktoré umožňuje klientske licencie ako Office 365 Business alebo Business Premium a [uistite sa, že používateľ má priradenú licenciu](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="59473-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="59473-105">Uistite sa, že používateľ sa prihlasuje do balíka Office s kontom, ktoré má priradenú licenciu.</span><span class="sxs-lookup"><span data-stu-id="59473-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="59473-106">Na [stránke Stav služby Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) skontrolujte, či sa nevyskytujú známe problémy so službou.</span><span class="sxs-lookup"><span data-stu-id="59473-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="59473-107">Skontrolujte nastavenia brány firewall, antivírusového softvéru a nastavení servera proxy a potvrďte, že neblokujú aplikáciám Microsoftu 365 prístup na internet.</span><span class="sxs-lookup"><span data-stu-id="59473-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="59473-108">Pozrite si tému [URL adresy a rozsahy IP adries v balíku Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL adresy a rozsahy IP adries služieb Office 365").</span><span class="sxs-lookup"><span data-stu-id="59473-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="59473-109">**Tip** Na zariadeniach s Windowsom pre vás môžeme diagnostikovať a automaticky opraviť niekoľko bežných problémov s prihlasovaním na do balíka Office.</span><span class="sxs-lookup"><span data-stu-id="59473-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="59473-110">Stiahnite a spustite asistenta **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)**, aby ste mohli používať náš automatický nástroj.</span><span class="sxs-lookup"><span data-stu-id="59473-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="59473-111">Postupujte podľa týchto krokov na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="59473-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="59473-112">Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont.</span><span class="sxs-lookup"><span data-stu-id="59473-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="59473-113">[Odstráňte](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) a [znova priraďte](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licenciu na Office a potom [sa prihláste do balíka Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou ovplyvneného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="59473-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="59473-114">Spustite nástroj [Poradca pri riešení problémov s aktiváciou](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="59473-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="59473-115">Obnovte stav aktivácie balíka Office</span><span class="sxs-lookup"><span data-stu-id="59473-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovte stav aktivácie balíka Office")
- [<span data-ttu-id="59473-116">Vykonanie online opravy balíka Office</span><span class="sxs-lookup"><span data-stu-id="59473-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="59473-117">Ďalšie riešenie problémov nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="59473-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="59473-118">Chyba produktu bez platnej licencie a chyba aktivácie v Office</span><span class="sxs-lookup"><span data-stu-id="59473-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="59473-119">Chyba „Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr“ pri aktivácii balíka Office</span><span class="sxs-lookup"><span data-stu-id="59473-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)
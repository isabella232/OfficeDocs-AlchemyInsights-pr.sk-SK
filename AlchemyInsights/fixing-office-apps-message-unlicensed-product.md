---
title: Balík Office sa nedá aktivovať
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: ee4618bd288e3e8be75dc969af58f921a14f48b0
ms.sourcegitcommit: bf87d91fa60bd961bc6c887c4a4be7a3c7665b38
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/01/2020
ms.locfileid: "44474512"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="d2cac-102">Balík Office sa nedá aktivovať</span><span class="sxs-lookup"><span data-stu-id="d2cac-102">Unable to activate Office</span></span>

- <span data-ttu-id="d2cac-103">Skontrolujte, či vám neuplynula platnosť predplatného.</span><span class="sxs-lookup"><span data-stu-id="d2cac-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="d2cac-104">Uistite sa, že máte predplatné, ktoré umožňuje klientske licencie, napríklad Office 365 Business alebo Business Premium, a [uistite sa, že používateľ má priradenú licenciu](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="d2cac-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="d2cac-105">Uistite sa, že používateľ sa prihlasuje do balíka Office s tým istým kontom, ktoré má priradenú licenciu.</span><span class="sxs-lookup"><span data-stu-id="d2cac-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="d2cac-106">Na [stránke Stav služby Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) skontrolujte, či sa nevyskytujú známe problémy so službou.</span><span class="sxs-lookup"><span data-stu-id="d2cac-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="d2cac-107">Skontrolujte nastavenia brány firewall, antivírusového softvéru a nastavení servera proxy a potvrďte, že neblokujú aplikáciám balíka Office prístup na internet.</span><span class="sxs-lookup"><span data-stu-id="d2cac-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Office apps access to the internet.</span></span> <span data-ttu-id="d2cac-108">Pozrite si tému [URL adresy a rozsahy IP adries v balíku Office 365](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "URL adresy a rozsahy IP adries v Office 365").</span><span class="sxs-lookup"><span data-stu-id="d2cac-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/en-us/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="d2cac-109">Postupujte podľa týchto krokov na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="d2cac-109">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="d2cac-110">Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont.</span><span class="sxs-lookup"><span data-stu-id="d2cac-110">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="d2cac-111">[Odstráňte](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Odstrániť") a [znova priraďte](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "znova priradiť") licenciu na Office a potom [sa prihláste do balíka Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "prihlásenie do balíka Office") pomocou ovplyvneného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="d2cac-111">[Remove](https://docs.microsoft.com/office365/admin/manage/remove-licenses-from-users?view=o365-worldwide "Remove") and [re-assign](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users?view=o365-worldwide "re-assign") Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9 "sign into Office") using the affected user account.</span></span>
- <span data-ttu-id="d2cac-112">Spustite nástroj [Poradca pri riešení problémov s aktiváciou](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="d2cac-112">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="d2cac-113">Obnovte stav aktivácie balíka Office</span><span class="sxs-lookup"><span data-stu-id="d2cac-113">Reset Office activation state</span></span>](https://docs.microsoft.com/en-us/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovenie stavu aktivácie balíka Office")
- [<span data-ttu-id="d2cac-114">Vykonanie online opravy balíka Office</span><span class="sxs-lookup"><span data-stu-id="d2cac-114">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="d2cac-115">Ďalšie riešenie problémov nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="d2cac-115">For additional troubleshooting solutions, see:</span></span>  
[<span data-ttu-id="d2cac-116">Chyba produktu bez platnej licencie a chyba aktivácie v Office</span><span class="sxs-lookup"><span data-stu-id="d2cac-116">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)  
<span data-ttu-id="d2cac-117">["Ľutujeme, nemôžeme sa pripojiť k vášmu kontu.</span><span class="sxs-lookup"><span data-stu-id="d2cac-117">["Sorry, we can't connect to your account.</span></span> <span data-ttu-id="d2cac-118">Skúste to znova neskôr" chyba pri aktivácii balíka Office]( https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 "Ľutujeme, nemôžeme sa pripojiť k vášmu kontu.</span><span class="sxs-lookup"><span data-stu-id="d2cac-118">Please try again later" error when you activate Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365 ""Sorry, we can't connect to your account.</span></span> <span data-ttu-id="d2cac-119">Skúste to znova neskôr" chyba pri aktivácii balíka Office")</span><span class="sxs-lookup"><span data-stu-id="d2cac-119">Please try again later" error when you activate Office")</span></span>
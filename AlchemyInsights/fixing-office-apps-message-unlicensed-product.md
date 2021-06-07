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
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798695"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="b2473-102">Office sa nedá aktivovať</span><span class="sxs-lookup"><span data-stu-id="b2473-102">Unable to activate Office</span></span>

<span data-ttu-id="b2473-103">**Poznámka:** Ak používate staršiu verziu balíka Windows (napríklad Windows 7), uistite sa, že protokol TLS 1.2 je predvolene povolený.</span><span class="sxs-lookup"><span data-stu-id="b2473-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="b2473-104">Ďalšie informácie nájdete v téme Aktualizácia na povolenie [tls 1.1 a TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ako predvolených zabezpečených protokolov vo WinHTTP v Windows.</span><span class="sxs-lookup"><span data-stu-id="b2473-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="b2473-105">Skontrolujte, či vám neuplynula platnosť predplatného.</span><span class="sxs-lookup"><span data-stu-id="b2473-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="b2473-106">Uistite sa, že máte predplatné, ktoré umožňuje klientske licencie ako Office 365 Business alebo Business Premium a [uistite sa, že používateľ má priradenú licenciu](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="b2473-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="b2473-107">Uistite sa, že používateľ sa prihlasuje do balíka Office s kontom, ktoré má priradenú licenciu.</span><span class="sxs-lookup"><span data-stu-id="b2473-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="b2473-108">Na [stránke Stav služby Office 365](/office365/enterprise/view-service-health) skontrolujte, či sa nevyskytujú známe problémy so službou.</span><span class="sxs-lookup"><span data-stu-id="b2473-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="b2473-109">Skontrolujte nastavenia brány firewall, antivírusového softvéru a nastavení servera proxy a potvrďte, že neblokujú aplikáciám Microsoftu 365 prístup na internet.</span><span class="sxs-lookup"><span data-stu-id="b2473-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="b2473-110">Pozrite si tému [URL adresy a rozsahy IP adries v balíku Office 365](/office365/enterprise/urls-and-ip-address-ranges "URL adresy a rozsahy IP adries služieb Office 365").</span><span class="sxs-lookup"><span data-stu-id="b2473-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="b2473-111">**Tip** Na zariadeniach s Windowsom pre vás môžeme diagnostikovať a automaticky opraviť niekoľko bežných problémov s prihlasovaním na do balíka Office.</span><span class="sxs-lookup"><span data-stu-id="b2473-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="b2473-112">Stiahnite a spustite asistenta **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)**, aby ste mohli používať náš automatický nástroj.</span><span class="sxs-lookup"><span data-stu-id="b2473-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="b2473-113">Postupujte podľa týchto krokov na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="b2473-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="b2473-114">Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont.</span><span class="sxs-lookup"><span data-stu-id="b2473-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="b2473-115">[Odstráňte](/microsoft-365/admin/manage/remove-licenses-from-users) a [znova priraďte](/microsoft-365/admin/manage/assign-licenses-to-users) licenciu na Office a potom [sa prihláste do balíka Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou ovplyvneného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="b2473-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="b2473-116">Spustite nástroj [Poradca pri riešení problémov s aktiváciou](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="b2473-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="b2473-117">Obnovte stav aktivácie balíka Office</span><span class="sxs-lookup"><span data-stu-id="b2473-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Obnovte stav aktivácie balíka Office")
- [<span data-ttu-id="b2473-118">Vykonanie online opravy balíka Office</span><span class="sxs-lookup"><span data-stu-id="b2473-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="b2473-119">Ďalšie riešenie problémov nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="b2473-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="b2473-120">Chyba produktu bez platnej licencie a chyba aktivácie v Office</span><span class="sxs-lookup"><span data-stu-id="b2473-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="b2473-121">Chyba „Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr“ pri aktivácii balíka Office</span><span class="sxs-lookup"><span data-stu-id="b2473-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)
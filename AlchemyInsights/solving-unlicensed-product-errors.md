---
title: Riešenie chýb produktu bez kurzívy
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786864"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="1b6b9-102">Návrhy na riešenie chýb produktu bez kurzívy</span><span class="sxs-lookup"><span data-stu-id="1b6b9-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="1b6b9-103">Ak chcete vyriešiť chyby týkajúce sa produktu bez kurzívy, vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="1b6b9-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="1b6b9-104">Skontrolujte, či uplynula platnosť stavu vášho predplatného.</span><span class="sxs-lookup"><span data-stu-id="1b6b9-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="1b6b9-105">Uistite sa, že máte predplatné, ktoré umožňuje klientske licencie, ako sú napríklad aplikácie Microsoft 365 pre podniky alebo Business Premium, a uistite sa, že používateľovi je [priradená licencia.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)</span><span class="sxs-lookup"><span data-stu-id="1b6b9-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="1b6b9-106">Skontrolujte, či sa používateľ prihlasuje do balíka Office s rovnakým kontom, ktoré má priradenú licenciu.</span><span class="sxs-lookup"><span data-stu-id="1b6b9-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="1b6b9-107">Skontrolujte stránku [Stav služby a](https://docs.microsoft.com/office365/enterprise/view-service-health) zistite, či sa v službe vyskytnú nejaké známe problémy.</span><span class="sxs-lookup"><span data-stu-id="1b6b9-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="1b6b9-108">Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy a overte, či aplikácie služby Microsoft 365 neblokujú prístup na internet.</span><span class="sxs-lookup"><span data-stu-id="1b6b9-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="1b6b9-109">Pozrite [si časť URL adresy a rozsahy IP adries.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="1b6b9-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="1b6b9-110">Môžete skúsiť aj tieto akcie na riešenie problémov:</span><span class="sxs-lookup"><span data-stu-id="1b6b9-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="1b6b9-111">Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont.</span><span class="sxs-lookup"><span data-stu-id="1b6b9-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="1b6b9-112">[Odstráňte](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) a [znova priraďte](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licenciu na Office a potom sa [prihláste do balíka Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou príslušného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="1b6b9-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="1b6b9-113">Spustite Poradcu [pri riešení problémov s aktiváciou.](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="1b6b9-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="1b6b9-114">[Obnovte stav aktivácie balíka Office.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="1b6b9-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="1b6b9-115">[Vykonanie online opravy balíka Office.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)</span><span class="sxs-lookup"><span data-stu-id="1b6b9-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="1b6b9-116">Ďalšie riešenie problémov nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="1b6b9-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="1b6b9-117">Chyba produktu bez platnej licencie a chyba aktivácie v Office</span><span class="sxs-lookup"><span data-stu-id="1b6b9-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="1b6b9-118">Chyba „Ľutujeme, nemôžeme sa pripojiť k vášmu kontu. Skúste to znova neskôr“ pri aktivácii balíka Office</span><span class="sxs-lookup"><span data-stu-id="1b6b9-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)
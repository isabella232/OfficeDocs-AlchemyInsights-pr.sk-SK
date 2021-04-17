---
title: Oprava hlásenia o oprave aplikácií služby Microsoft 365 Nepodarilo sa nájsť licencie balíka Office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816503"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="b3a0c-102">Oprava hlásenia o oprave aplikácií služby Microsoft 365 "Nepodarilo sa nájsť licencie balíka Office priradené"</span><span class="sxs-lookup"><span data-stu-id="b3a0c-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="b3a0c-103">Ak sa zobrazí toto hlásenie, skúste toto:</span><span class="sxs-lookup"><span data-stu-id="b3a0c-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="b3a0c-104">Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy a overte, či neblokujú prístup na internet k aplikáciám služby Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b3a0c-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="b3a0c-105">Pozrite si časť URL adresy a rozsahy IP adries v [Microsoft 365.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="b3a0c-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="b3a0c-106">Odobrať [a zmeniť priradenie licencie na Office pre](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) príslušného používateľa.</span><span class="sxs-lookup"><span data-stu-id="b3a0c-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="b3a0c-107">Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont.</span><span class="sxs-lookup"><span data-stu-id="b3a0c-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="b3a0c-108">Prejdite na nastavenia Windowsu > **Kontá**  >  **e-& kontá a** odstráňte všetky pracovné kontá okrem príslušného konta.</span><span class="sxs-lookup"><span data-stu-id="b3a0c-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="b3a0c-109">Prejdite na nastavenia Windowsu > **Kontá**  >  **prístup k pracovnému alebo školskému** a odpojte všetky pracovné kontá okrem príslušného konta.</span><span class="sxs-lookup"><span data-stu-id="b3a0c-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="b3a0c-110">Obnovte stav aktivácie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="b3a0c-110">Reset the Office activation state.</span></span> <span data-ttu-id="b3a0c-111">[Zistite, ako na to.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="b3a0c-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="b3a0c-112">[Prihláste sa](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou príslušného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="b3a0c-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="b3a0c-113">Ďalšie riešenia problémov nájdete v téme Chyba [produktu bez licencie a chyba aktivácie v Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="b3a0c-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
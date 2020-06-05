---
title: Oprava aplikácií microsoft 365 Nepodarilo sa nájsť office licencie priradené správy
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 65ffae1a784f841cb08a5df52b02671a4526d9d4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580456"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="052bb-102">Oprava správy aplikácie Microsoft 365 "Nepodarilo sa nájsť priradené licencie balíka Office"</span><span class="sxs-lookup"><span data-stu-id="052bb-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="052bb-103">Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúci postup:</span><span class="sxs-lookup"><span data-stu-id="052bb-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="052bb-104">Skontrolujte nastavenia brány firewall, antivírusového softvéru a servera proxy, aby ste potvrdili, že neblokujú prístup na Internet k aplikáciám Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="052bb-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="052bb-105">Pozrite si [článok Adresy URL a rozsahy adries IP od spoločnosti Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="052bb-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="052bb-106">Odstráňte a [znova priraďte licenciu balíka Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pre príslušného používateľa.</span><span class="sxs-lookup"><span data-stu-id="052bb-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="052bb-107">Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z existujúcich používateľských kont.</span><span class="sxs-lookup"><span data-stu-id="052bb-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="052bb-108">Prejdite do časti Nastavenie systému Windows > **kontá**  >  **E-mailové & kontá**a odstráňte všetky pracovné kontá okrem príslušného konta.</span><span class="sxs-lookup"><span data-stu-id="052bb-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="052bb-109">Prejdite do časti Nastavenie systému Windows > **kontá**  >  **Prístup k práci alebo škole**a odpojte všetky pracovné kontá okrem príslušného konta.</span><span class="sxs-lookup"><span data-stu-id="052bb-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="052bb-110">Obnovte stav aktivácie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="052bb-110">Reset the Office activation state.</span></span> <span data-ttu-id="052bb-111">[Prečítajte si, ako](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="052bb-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="052bb-112">[Prihláste sa](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomocou príslušného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="052bb-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="052bb-113">Ďalšie riešenia problémov nájdete v téme [Chyby produktu bez platnej licencie a aktivácie v balíku Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="052bb-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
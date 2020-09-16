---
title: Oprava aplikácií Microsoft 365 nenašiel priradené správy o licenciách balíka Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747710"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="f265a-102">Oprava aplikácií Microsoft 365 sa nepodarilo nájsť priradenú licenciu na Office</span><span class="sxs-lookup"><span data-stu-id="f265a-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="f265a-103">Ak sa zobrazí toto hlásenie, vyskúšajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="f265a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f265a-104">Skontrolujte bránu firewall, antivírusový softvér a nastavenia servera proxy a potvrďte, že neblokujú prístup na internet k aplikáciám Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f265a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="f265a-105">Pozrite si tému [URL adresy a rozsahy IP adries pre Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f265a-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="f265a-106">Odstránenie a opätovné [Priradenie licencie na Office](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) pre príslušného používateľa.</span><span class="sxs-lookup"><span data-stu-id="f265a-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="f265a-107">Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) zo všetkých existujúcich používateľských kont.</span><span class="sxs-lookup"><span data-stu-id="f265a-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="f265a-108">Prejdite na položky Nastavenie systému Windows > **kontá**  >  **e-mailové & kontá**a odstráňte všetky pracovné kontá okrem príslušného konta.</span><span class="sxs-lookup"><span data-stu-id="f265a-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="f265a-109">Prejdite na položky Nastavenie systému Windows > prístup k **kontám**v  >  **práci alebo škole**a odpojte všetky pracovné kontá okrem príslušného konta.</span><span class="sxs-lookup"><span data-stu-id="f265a-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="f265a-110">Obnovte stav aktivácie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="f265a-110">Reset the Office activation state.</span></span> <span data-ttu-id="f265a-111">[Zistite, ako](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)na to.</span><span class="sxs-lookup"><span data-stu-id="f265a-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="f265a-112">[Prihláste](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sa pomocou príslušného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="f265a-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="f265a-113">Ďalšie riešenia na riešenie problémov nájdete v téme chyby týkajúce sa produktu bez platnej [licencie a aktivácie balíka Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="f265a-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
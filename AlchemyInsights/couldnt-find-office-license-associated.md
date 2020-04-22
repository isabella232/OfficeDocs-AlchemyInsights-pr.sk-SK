---
title: Oprava aplikácií balíka Office nemohla nájsť priradenú správu licencií balíka Office
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
ms.openlocfilehash: 565df0a05baa974a6cbac58ac6be8d78470dbc5d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715647"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="30770-102">Oprava aplikácií balíka Office "Nepodarilo sa nájsť Office licencie súvisiace" správa</span><span class="sxs-lookup"><span data-stu-id="30770-102">Fixing the Office apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="30770-103">Ak sa zobrazí toto hlásenie, vyskúšajte nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="30770-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="30770-104">Skontrolujte, či brána firewall, antivírusový softvér a nastavenia servera proxy potvrdia, že neblokujú prístup na internet k aplikáciám balíka Office.</span><span class="sxs-lookup"><span data-stu-id="30770-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="30770-105">Pozrite si [Microsoft 365 URL a rozsahy adries IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="30770-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="30770-106">Odstráňte a [priraďte licenciu balíka Office](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) pre príslušného používateľa.</span><span class="sxs-lookup"><span data-stu-id="30770-106">Remove and [reassign the Office license](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="30770-107">Otvorte aplikáciu balíka Office a [odhláste sa](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) z existujúcich používateľských kont.</span><span class="sxs-lookup"><span data-stu-id="30770-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="30770-108">Prejdite na nastavenia systému Windows > **kontá** > **e-mailové & kontá**a odstráňte všetky pracovné kontá okrem príslušného konta.</span><span class="sxs-lookup"><span data-stu-id="30770-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="30770-109">Prejdite na nastavenia systému Windows > **kontá** > **prístup k práci alebo škole**, a odpojte všetky pracovné účty okrem príslušného konta.</span><span class="sxs-lookup"><span data-stu-id="30770-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="30770-110">Obnoviť stav aktivácie balíka Office.</span><span class="sxs-lookup"><span data-stu-id="30770-110">Reset the Office activation state.</span></span> <span data-ttu-id="30770-111">[Prečítajte si, ako](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="30770-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="30770-112">[Prihláste](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sa pomocou príslušného používateľského konta.</span><span class="sxs-lookup"><span data-stu-id="30770-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="30770-113">Ďalšie riešenia na riešenie problémov nájdete [v téme nelicencované produkty a chyby aktivácie v balíku Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="30770-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
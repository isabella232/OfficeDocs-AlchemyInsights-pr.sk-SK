---
title: Určiť adresy IP a klient v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752074"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="75550-102">Určiť adresy IP a klient v denníkoch auditu</span><span class="sxs-lookup"><span data-stu-id="75550-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="75550-103">Adresu IP, ktorá zodpovedá činnosť používateľa alebo správcu sa zobrazí denníky auditu.</span><span class="sxs-lookup"><span data-stu-id="75550-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="75550-104">Informácie o klientovi je tiež prihlásený.</span><span class="sxs-lookup"><span data-stu-id="75550-104">The client information is also logged.</span></span> <span data-ttu-id="75550-105">Tu sú kroky na identifikáciu takýchto informácií</span><span class="sxs-lookup"><span data-stu-id="75550-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="75550-106">Prihláste sa do [Centrum Office 365 zabezpečenia & súlad](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="75550-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="75550-107">Kliknite na položku **vyhľadávanie a vyšetrovanie** a vyberte **Vyhľadávanie denník auditu**.</span><span class="sxs-lookup"><span data-stu-id="75550-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="75550-108">Ak máte záujem v konkrétnej činnosti, vyberte ho zo zoznamu **činností** .</span><span class="sxs-lookup"><span data-stu-id="75550-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="75550-109">Ak nie, vrátia všetky aktivity pre vybratého používateľa (predvolené nastavenie).</span><span class="sxs-lookup"><span data-stu-id="75550-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="75550-110">**Poznámka**: niektoré činnosti nemusia byť dostupné v menu **aktivity** ; však o audite položky budú vrátené Ak **Ukázať výsledky všetkých činností** je (predvolené nastavenie).</span><span class="sxs-lookup"><span data-stu-id="75550-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="75550-111">V poli **Používatelia** zadať užívateľské meno, vyberte príslušný rozsah dátumov pre aktivitu a kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="75550-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="75550-112">Vo výsledkoch zobrazí adresu IP pre túto činnosť v table výsledky.</span><span class="sxs-lookup"><span data-stu-id="75550-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="75550-113">Vyberte auditný záznam zobrazíte podrobné informácie v **Podrobnosti** Nadjazd (napríklad klient, používateľ, ktorý vykonáva akcie, atď.).</span><span class="sxs-lookup"><span data-stu-id="75550-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="75550-114">Ďalšie informácie nájdete v téme [Lokalizovanie adresu IP počítača používa na prístup k ohrozeným kontom](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="75550-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>

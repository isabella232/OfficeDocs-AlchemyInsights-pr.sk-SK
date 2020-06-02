---
title: Identifikácia adresy IP a klienta v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508931"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="fdee2-102">Identifikácia adresy IP a klienta v denníkoch auditu</span><span class="sxs-lookup"><span data-stu-id="fdee2-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="fdee2-103">Adresa IP, ktorá zodpovedá aktivite používateľa alebo správcu služby Microsoft 365, sa zobrazuje v denníkoch auditu.</span><span class="sxs-lookup"><span data-stu-id="fdee2-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="fdee2-104">Informácie o klientovi sa tiež zaznamená.</span><span class="sxs-lookup"><span data-stu-id="fdee2-104">The client information is also logged.</span></span> <span data-ttu-id="fdee2-105">Tu sú kroky na identifikáciu týchto informácií</span><span class="sxs-lookup"><span data-stu-id="fdee2-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="fdee2-106">Prihláste sa do Centra [& zabezpečenia spoločnosti Microsoft 365](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="fdee2-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="fdee2-107">Prejdite na stránku **vyhľadávania**  >  **v denníku auditu.**</span><span class="sxs-lookup"><span data-stu-id="fdee2-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="fdee2-108">Ak máte záujem o konkrétnu aktivitu, vyberte ju zo zoznamu **Aktivity.**</span><span class="sxs-lookup"><span data-stu-id="fdee2-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="fdee2-109">Ak nie, všetky aktivity sa vrátia pre vybratého používateľa (predvolené nastavenie).</span><span class="sxs-lookup"><span data-stu-id="fdee2-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="fdee2-110">**Poznámka:** Niektoré činnosti nemusia byť k dispozícii v menu **Aktivity;** Tieto položky auditu sa však vrátia, ak je vybratá možnosť **Zobraziť výsledky pre všetky aktivity** (predvolené nastavenie).</span><span class="sxs-lookup"><span data-stu-id="fdee2-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="fdee2-111">Zadajte meno používateľa do poľa **Používatelia,** vyberte príslušný rozsah dátumov pre aktivitu a potom kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="fdee2-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="fdee2-112">Vo výsledkoch sa na table s výsledkami zobrazuje adresa IP pre danú aktivitu.</span><span class="sxs-lookup"><span data-stu-id="fdee2-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="fdee2-113">Vyberte záznam auditu a zobrazia sa podrobné informácie v rozbaľovacom zozname **Podrobnosti** (napríklad Klient, Používateľ, ktorý vykonal akciu atď.).</span><span class="sxs-lookup"><span data-stu-id="fdee2-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="fdee2-114">Ďalšie informácie sa nachádzajú v téme [Vyhľadanie adresy IP počítača používaného na prístup k ohrozenému kontu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="fdee2-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>

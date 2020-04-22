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
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716403"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="bbb40-102">Identifikácia adresy IP a klienta v denníkoch auditu</span><span class="sxs-lookup"><span data-stu-id="bbb40-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="bbb40-103">Adresa IP, ktorá zodpovedá aktivite používateľa alebo správcu spoločnosti Microsoft 365, sa zobrazí v denníkoch auditu.</span><span class="sxs-lookup"><span data-stu-id="bbb40-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="bbb40-104">Informácie o klientovi je tiež prihlásený.</span><span class="sxs-lookup"><span data-stu-id="bbb40-104">The client information is also logged.</span></span> <span data-ttu-id="bbb40-105">Tu sú kroky na identifikáciu týchto informácií</span><span class="sxs-lookup"><span data-stu-id="bbb40-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="bbb40-106">Prihláste sa do [Microsoft 365 Security & centrum súladu](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="bbb40-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="bbb40-107">Prejdite na stránku vyhľadávania**denníka auditu** **vyhľadávania** > .</span><span class="sxs-lookup"><span data-stu-id="bbb40-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="bbb40-108">Ak máte záujem o konkrétnu aktivitu, vyberte ju zo zoznamu **aktivity** .</span><span class="sxs-lookup"><span data-stu-id="bbb40-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="bbb40-109">Ak nie, všetky aktivity sa vrátia pre vybratého používateľa (predvolené nastavenie).</span><span class="sxs-lookup"><span data-stu-id="bbb40-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="bbb40-110">**Poznámka**: niektoré aktivity nemusia byť k dispozícii v ponuke **aktivity** ; Tieto položky auditu sa však vrátia, ak je vybratá možnosť **Zobraziť výsledky pre všetky aktivity** (predvolené nastavenie).</span><span class="sxs-lookup"><span data-stu-id="bbb40-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="bbb40-111">Zadajte meno používateľa v poli **Používatelia** , vyberte príslušný rozsah dátumov pre aktivitu a potom kliknite na tlačidlo **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="bbb40-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="bbb40-112">Vo výsledkoch môžete vidieť adresu IP danej aktivity na table s výsledkami.</span><span class="sxs-lookup"><span data-stu-id="bbb40-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="bbb40-113">Vyberte záznam auditu a zobrazia sa podrobné informácie v rozbaľovacom zozname **Podrobnosti** (napríklad klient, používateľ, ktorý vykonal akciu atď.).</span><span class="sxs-lookup"><span data-stu-id="bbb40-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="bbb40-114">Ďalšie informácie nájdete v téme [vyhľadanie adresy IP počítača používaného na prístup k ohrozeným účtom](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="bbb40-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>

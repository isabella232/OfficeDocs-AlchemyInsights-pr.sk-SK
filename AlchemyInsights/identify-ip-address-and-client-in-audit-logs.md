---
title: Identifikácia IP adresy a klienta v denníkoch auditu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668325"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="95138-102">Identifikácia IP adresy a klienta v denníkoch auditu</span><span class="sxs-lookup"><span data-stu-id="95138-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="95138-103">IP adresa, ktorá zodpovedá aktivite používateľa alebo správcu Microsoft 365, sa zobrazí v denníkoch auditu.</span><span class="sxs-lookup"><span data-stu-id="95138-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="95138-104">Informácie o klientovi sa tiež zaznamenávajú.</span><span class="sxs-lookup"><span data-stu-id="95138-104">The client information is also logged.</span></span> <span data-ttu-id="95138-105">Tu sú kroky na identifikáciu týchto informácií</span><span class="sxs-lookup"><span data-stu-id="95138-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="95138-106">Prihláste sa do [Centra zabezpečenia dodržiavania súladu so službou Microsoft 365 Security &](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="95138-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="95138-107">Prejdite na stránku **Search**  >  **vyhľadávania denníka auditu** vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="95138-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="95138-108">Ak máte záujem o konkrétnu aktivitu, vyberte ju zo zoznamu **aktivity** .</span><span class="sxs-lookup"><span data-stu-id="95138-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="95138-109">Ak nie, pre vybratého používateľa sa vrátia všetky aktivity (predvolené nastavenie).</span><span class="sxs-lookup"><span data-stu-id="95138-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="95138-110">**Poznámka**: niektoré aktivity nemusia byť v ponuke **aktivity** k dispozícii. Tieto položky auditu sa však vrátia, ak je vybratá možnosť **Zobraziť výsledky pre všetky aktivity** (predvolené nastavenie).</span><span class="sxs-lookup"><span data-stu-id="95138-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="95138-111">Zadajte meno používateľa v poli **Používatelia** , vyberte príslušný rozsah dátumov pre aktivitu a potom kliknite na položku **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="95138-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="95138-112">Vo výsledkoch môžete na table Výsledky Zobraziť IP adresu danej aktivity.</span><span class="sxs-lookup"><span data-stu-id="95138-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="95138-113">Vyberte záznam auditu, aby sa zobrazili podrobné informácie v rozbaľovacom zozname **podrobností** (napríklad klient, používateľ, ktorý vykonal akciu atď.).</span><span class="sxs-lookup"><span data-stu-id="95138-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="95138-114">Ďalšie informácie nájdete v téme [Vyhľadanie IP adresy počítača, ktorý sa používa na prístup k ohrozenému kontu](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="95138-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>

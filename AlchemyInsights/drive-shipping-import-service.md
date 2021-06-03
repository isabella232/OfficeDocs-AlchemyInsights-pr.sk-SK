---
title: Odoslanie disku v službe Microsoft 365 Import Service
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731947"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="bf0e2-102">Odoslanie disku v službe Microsoft 365 Import Service</span><span class="sxs-lookup"><span data-stu-id="bf0e2-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="bf0e2-103">Pomocou odosielania disku skopírujte súbory PSTs na pevný disk a potom pevný disk odovedzte spoločnosti Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bf0e2-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="bf0e2-104">Začatie úlohy:</span><span class="sxs-lookup"><span data-stu-id="bf0e2-104">To start the job:</span></span>

1. <span data-ttu-id="bf0e2-105">V centre Microsoft 365 dodržiavania súladu v časti **Riadenie informácií** vyberte položku **Importovať**.</span><span class="sxs-lookup"><span data-stu-id="bf0e2-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="bf0e2-106">Vyberte **položku Vyberte typ úlohy importu** a potom vyberte položku **Ďalej**.</span><span class="sxs-lookup"><span data-stu-id="bf0e2-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="bf0e2-107">Ak chcete zobraziť postup pre túto možnosť importu, vyberte **položku Pevný disk do niektorého z našich fyzických umiestnení.**</span><span class="sxs-lookup"><span data-stu-id="bf0e2-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="bf0e2-108">Tu je niekoľko vecí, na ktoré je potrebné pamätať:</span><span class="sxs-lookup"><span data-stu-id="bf0e2-108">Here are some things to remember:</span></span>

- <span data-ttu-id="bf0e2-109">Ak chcete v poštovej schránke importovať súbory PST do poštových schránok, Exchange Online mať priradenú rolu importu a exportu Microsoft 365 poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="bf0e2-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="bf0e2-110">Výkon môže ovplyvniť viac ako 20 GB v prípade PT, ktoré sú väčšie.</span><span class="sxs-lookup"><span data-stu-id="bf0e2-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="bf0e2-111">Podporované sú len 2,5-palcové SSD disky alebo 2,5-palcové alebo 3,5-palcové interné pevné disky SATA II/III.</span><span class="sxs-lookup"><span data-stu-id="bf0e2-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="bf0e2-112">Pevný disk obsahujúci súbory PST musí byť zašifrovaný šifrovanie BitLocker.</span><span class="sxs-lookup"><span data-stu-id="bf0e2-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="bf0e2-113">Poplatok za importovanie súborov PST do Microsoft 365 poštových schránok pomocou odosielania disku je 2 USD za každý GB údajov.</span><span class="sxs-lookup"><span data-stu-id="bf0e2-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="bf0e2-114">Ďalšie informácie o používaní spôsobu odosielania disku na importovanie súborov PST nájdete v téme Importovanie súborov PST organizácie [pomocou odosielania disku.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="bf0e2-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>
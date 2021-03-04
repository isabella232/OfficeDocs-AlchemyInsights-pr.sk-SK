---
title: Vyhľadanie IP adresy v denníku auditu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429790"
---
# <a name="find-the-ip-address-in-audit-log"></a><span data-ttu-id="97e0d-102">Vyhľadanie IP adresy v denníku auditu</span><span class="sxs-lookup"><span data-stu-id="97e0d-102">Find the IP address in audit log</span></span>

1. <span data-ttu-id="97e0d-103">IP adresa, ktorá zodpovedá aktivite vykonanej používateľom alebo správcom, sa zobrazuje v denníkoch auditu.</span><span class="sxs-lookup"><span data-stu-id="97e0d-103">The IP address that corresponds to an activity performed by a user or administrator is shown in the audit logs.</span></span> <span data-ttu-id="97e0d-104">Informácie o klientovi sa tiež zaznamenávajú.</span><span class="sxs-lookup"><span data-stu-id="97e0d-104">The client information is also logged.</span></span> <span data-ttu-id="97e0d-105">Tu je návod na identifikáciu IP adresy:</span><span class="sxs-lookup"><span data-stu-id="97e0d-105">Here's how to identify the IP address:</span></span>

1. <span data-ttu-id="97e0d-106">Prejdite na [centrum dodržiavania súladu & zabezpečenia služieb Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="97e0d-106">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="97e0d-107">Vyberte položku  >  **[vyhľadávanie denníkov auditu](https://go.microsoft.com/fwlink/?linkid=2103759)** vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="97e0d-107">Select **Search** > **[Audit log search](https://go.microsoft.com/fwlink/?linkid=2103759)**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="97e0d-108">Ak sa zobrazí oznámenie o tom, že je potrebné zapnúť auditovanie, pokračujte a teraz ho zapnite.</span><span class="sxs-lookup"><span data-stu-id="97e0d-108">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="97e0d-109">Ak táto funkcia nie je povolená, výsledky hľadania nebudú môcť vytiahnuť údaje z predchádzajúcich dátumov.</span><span class="sxs-lookup"><span data-stu-id="97e0d-109">If this feature isn't enabled, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="97e0d-110">Ak máte záujem o konkrétnu aktivitu, vyberte ju v zozname **aktivity** . v opačnom prípade sa predvolene vrátia všetky aktivity vybratého používateľa.</span><span class="sxs-lookup"><span data-stu-id="97e0d-110">If you're interested in a specific activity, select it from the **Activities** list; otherwise, by default, all activities will be returned for the selected user.</span></span> <span data-ttu-id="97e0d-111">Všimnite si, že niektoré aktivity nemusia byť v ponuke **aktivity** k dispozícii na výber. Tieto položky auditu sa však vrátia, ak je vybratá možnosť **Zobraziť výsledky pre všetky aktivity** (predvolené nastavenie).</span><span class="sxs-lookup"><span data-stu-id="97e0d-111">Note that certain activities might not be available for selection from the **Activities** menu; however, those audit items will be returned if **Show results for all activities** is selected (default setting).</span></span>
1. <span data-ttu-id="97e0d-112">Zadajte rozsah dátumov a v poli **Používatelia** vyberte meno používateľa, ktorého chcete preskúmať.</span><span class="sxs-lookup"><span data-stu-id="97e0d-112">Specify the date range, and in the **Users** field, select the username for the user you want to investigate.</span></span>
1. <span data-ttu-id="97e0d-113">Vyberte položku **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="97e0d-113">Select **Search**.</span></span> <span data-ttu-id="97e0d-114">Aktivity sa zobrazia v časti **výsledky**.</span><span class="sxs-lookup"><span data-stu-id="97e0d-114">The activities appear under **Results**.</span></span> <span data-ttu-id="97e0d-115">Môžete zobraziť IP adresu pre každú aktivitu.</span><span class="sxs-lookup"><span data-stu-id="97e0d-115">You can see the IP address for each activity.</span></span>
1. <span data-ttu-id="97e0d-116">Ak chcete zobraziť podrobnosti, vyberte aktivitu a potom vyberte položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="97e0d-116">To view details, select an activity, and then select **More Information**.</span></span>

<span data-ttu-id="97e0d-117">Ďalšie informácie nájdete v téme Vyhľadávanie v [denníku auditu služieb Office 365 na riešenie bežných scenárov](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="97e0d-117">To learn more, see Search the [Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
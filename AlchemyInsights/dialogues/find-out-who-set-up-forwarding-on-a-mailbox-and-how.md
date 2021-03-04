---
title: Zistite, kto nastavuje preposielanie v poštovej schránke a ako
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429994"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a><span data-ttu-id="d5a03-102">Zistite, kto nastavuje preposielanie v poštovej schránke a ako</span><span class="sxs-lookup"><span data-stu-id="d5a03-102">Find out who set up forwarding on a mailbox, and how</span></span>

<span data-ttu-id="d5a03-103">Ak bol v poštovej schránke nastavený externý preposielanie, aktivita sa Audituje ako súčasť rutiny typu cmdlet Set-Mailbox.</span><span class="sxs-lookup"><span data-stu-id="d5a03-103">If external forwarding was set on a mailbox, the activity is audited as part of the Set-Mailbox cmdlet.</span></span> <span data-ttu-id="d5a03-104">Tu je návod na nájdenie aktivity v denníku auditu:</span><span class="sxs-lookup"><span data-stu-id="d5a03-104">Here's how to find the activity in the audit log:</span></span>

1. <span data-ttu-id="d5a03-105">Prejdite na [centrum dodržiavania súladu & zabezpečenia služieb Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="d5a03-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="d5a03-106">Vyberte položku >  **vyhľadávanie denníkov auditu** vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="d5a03-106">Select **Search**> **Audit log search**.</span></span>
    > [!NOTE]
    > <span data-ttu-id="d5a03-107">Ak sa zobrazí oznámenie o tom, že je potrebné zapnúť auditovanie, pokračujte a teraz ho zapnite.</span><span class="sxs-lookup"><span data-stu-id="d5a03-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="d5a03-108">Ak táto funkcia nie je zapnutá, výsledky hľadania nebudú môcť vytiahnuť údaje z predchádzajúcich dátumov.</span><span class="sxs-lookup"><span data-stu-id="d5a03-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="d5a03-109">Uistite sa, že pole **aktivity** je nastavené na možnosť **Zobraziť výsledky pre všetky aktivity** (predvolené).</span><span class="sxs-lookup"><span data-stu-id="d5a03-109">Make sure the **Activities** field is set to **Show results for all activities** (the default).</span></span> <span data-ttu-id="d5a03-110">Zadajte rozsah dátumov.</span><span class="sxs-lookup"><span data-stu-id="d5a03-110">Specify the date range.</span></span> <span data-ttu-id="d5a03-111">Nemusíte špecifikovať meno používateľa.</span><span class="sxs-lookup"><span data-stu-id="d5a03-111">You don't need to specify a username.</span></span>
1. <span data-ttu-id="d5a03-112">Vyberte položku **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="d5a03-112">Select **Search**.</span></span> <span data-ttu-id="d5a03-113">Aktivity sa zobrazia v časti **výsledky**.</span><span class="sxs-lookup"><span data-stu-id="d5a03-113">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="d5a03-114">Vyberte položku **výsledky filtrovania** a potom do poľa Filter **aktivity** zadajte položku **množina poštových schránok** .</span><span class="sxs-lookup"><span data-stu-id="d5a03-114">Select **Filter Results**, and then enter **Set-mailbox** in the **Activity** filter field.</span></span> <span data-ttu-id="d5a03-115">Tým sa vrátia všetky aktivity v **nastaveniach poštovej schránky** .</span><span class="sxs-lookup"><span data-stu-id="d5a03-115">This returns all **Set-Mailbox** activities.</span></span>
1. <span data-ttu-id="d5a03-116">Ak chcete zobraziť podrobnosti, vyberte aktivitu a potom vyberte položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="d5a03-116">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="d5a03-117">V časti **parametre** môžete zobraziť e-mailovú adresu preposielania, ktorá bola nastavená v poštovej schránke.</span><span class="sxs-lookup"><span data-stu-id="d5a03-117">Under **Parameters** you can see the forwarding email address that was set on the mailbox.</span></span> <span data-ttu-id="d5a03-118">**Userid** označuje používateľa, ktorý v poštovej schránke nastavil externý preposielanie.</span><span class="sxs-lookup"><span data-stu-id="d5a03-118">The **UserID** represents the user who set up external forwarding on the mailbox.</span></span>
<span data-ttu-id="d5a03-119">Ďalšie informácie nájdete v téme [vyhľadávanie v denníku auditu služieb Office 365 na riešenie bežných scenárov](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="d5a03-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
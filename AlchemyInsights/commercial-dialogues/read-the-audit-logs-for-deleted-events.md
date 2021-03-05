---
title: Prečítajte si denníky auditu odstránených udalostí
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
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483317"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="1ce9b-102">Prečítajte si denníky auditu odstránených udalostí</span><span class="sxs-lookup"><span data-stu-id="1ce9b-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="1ce9b-103">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="1ce9b-103">Here's how to do this:</span></span>

1. <span data-ttu-id="1ce9b-104">Prejdite na [centrum dodržiavania súladu & zabezpečenia služieb Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="1ce9b-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="1ce9b-105">Vyberte položku  >  [**vyhľadávanie denníkov auditu**](https://go.microsoft.com/fwlink/?linkid=2103759)vyhľadávania.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="1ce9b-106">Ak sa zobrazí upozornenie, že je potrebné túto funkciu zapnúť, pokračujte a zapnite ju teraz.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="1ce9b-107">Ak funkcia nie je zapnutá, výsledky hľadania nebudú môcť vytiahnuť údaje z predchádzajúcich dátumov.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="1ce9b-108">Vyberte položku **aktivity** a potom vyhľadajte položku **aktivity poštovej schránky servera Exchange**.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="1ce9b-109">Vyberte priečinok Odstránené **správy z priečinka Odstránené položky** a **premiestnili sa správy do možností priečinka Odstránené položky** .</span><span class="sxs-lookup"><span data-stu-id="1ce9b-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="1ce9b-110">Po dokončení kliknite mimo tably na minimalizovanie tably **aktivity** .</span><span class="sxs-lookup"><span data-stu-id="1ce9b-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="1ce9b-111">Zadajte rozsah dátumov a potom v poli **Používatelia** vyberte meno používateľa, ktorého chcete preskúmať.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="1ce9b-112">Naraz môžete vybrať viac ako jedného používateľa.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="1ce9b-113">Vyberte položku **Hľadať**.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-113">Select **Search**.</span></span> <span data-ttu-id="1ce9b-114">Aktivity sa zobrazia v časti **výsledky**.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="1ce9b-115">Ak chcete zobraziť podrobnosti, vyberte aktivitu a potom vyberte položku **Ďalšie informácie**.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="1ce9b-116">Ďalšie informácie o odstránenej položke, ako je napríklad riadok predmetu a umiestnenie položky pri odstránení, sa zobrazia v poli **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="1ce9b-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="1ce9b-117">Odstránené položky nie je možné obnoviť pomocou funkcie denník auditu.</span><span class="sxs-lookup"><span data-stu-id="1ce9b-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="1ce9b-118">Ak chcete obnoviť odstránené položky, pozrite si tému [Obnovenie odstránených položiek alebo e-mailu v aplikácii Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="1ce9b-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="1ce9b-119">Ďalšie informácie nájdete v téme [vyhľadávanie v denníku auditu služieb Office 365 na riešenie bežných scenárov](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="1ce9b-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>

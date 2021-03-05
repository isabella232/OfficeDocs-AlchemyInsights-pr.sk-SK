---
title: Vyhľadanie udalostí vykonaných na základe pravidiel pre doručenú poštu
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483703"
---
# <a name="find-events-performed-on-inbox-rules"></a><span data-ttu-id="0b8e3-102">Vyhľadanie udalostí vykonaných na základe pravidiel pre doručenú poštu</span><span class="sxs-lookup"><span data-stu-id="0b8e3-102">Find events performed on inbox rules</span></span>

<span data-ttu-id="0b8e3-103">Keď sa pravidlá pre doručenú poštu vytvoria, zmenia alebo odstránia, udalosti sa zaznamenávajú do denníka auditu.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-103">When inbox rules are created, changed, or deleted, the events are recorded in the audit log.</span></span> <span data-ttu-id="0b8e3-104">Tu je návod na ich preskúmanie:</span><span class="sxs-lookup"><span data-stu-id="0b8e3-104">Here's how to review them:</span></span>

1. <span data-ttu-id="0b8e3-105">Prejdite na [centrum dodržiavania súladu & zabezpečenia služieb Office 365](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="0b8e3-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="0b8e3-106">Vyberte položku Hľadať > denník auditu.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-106">Select Search > Audit log search.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0b8e3-107">Ak sa zobrazí oznámenie o tom, že je potrebné zapnúť auditovanie, pokračujte a teraz ho zapnite.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-107">If you see a notice that you need to turn on auditing, go ahead and turn it on now.</span></span> <span data-ttu-id="0b8e3-108">Ak táto funkcia nie je zapnutá, výsledky hľadania nebudú môcť vytiahnuť údaje z predchádzajúcich dátumov.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-108">If this feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="0b8e3-109">Vyberte pole aktivity a vyhľadajte položku aktivity poštovej schránky servera Exchange a potom vyberte položku New-InboxRule vytvoriť pravidlo pre doručenú poštu z aplikácie Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-109">Select the Activities field and find Exchange mailbox activities, and then select New-InboxRule Create inbox rule from Outlook Web App.</span></span> <span data-ttu-id="0b8e3-110">Po dokončení kliknite mimo tably na minimalizovanie tably aktivity.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-110">When you're done, click outside of the pane to minimize the Activities pane.</span></span>
1. <span data-ttu-id="0b8e3-111">Zadajte rozsah dátumov a potom v poli používatelia vyberte meno používateľa, ktorého chcete preskúmať.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-111">Specify the date range, and then in the Users field, select the username for the user you want to investigate.</span></span> <span data-ttu-id="0b8e3-112">Naraz môžete vybrať viac ako jedného používateľa.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="0b8e3-113">Vyberte položku Hľadať.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-113">Select Search.</span></span> <span data-ttu-id="0b8e3-114">Aktivity sa zobrazia v časti výsledky.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-114">The activities appear under Results.</span></span>
1. <span data-ttu-id="0b8e3-115">Ak chcete zobraziť podrobnosti, vyberte aktivitu a potom vyberte položku Ďalšie informácie.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-115">To view details, select an activity, and then select More Information.</span></span> <span data-ttu-id="0b8e3-116">V časti parametre sa zobrazuje názov pravidla, podmienky a akcie, ktoré bude mať pravidlo.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-116">Under the Parameters section you can see the name of the rule, conditions set, and the actions that the rule will take.</span></span>

<span data-ttu-id="0b8e3-117">Ďalšie informácie nájdete v téme Vyhľadávanie v denníku auditu služieb Office 365 na riešenie bežných scenárov.</span><span class="sxs-lookup"><span data-stu-id="0b8e3-117">To learn more, see Search the Office 365 audit log to troubleshoot common scenarios.</span></span>
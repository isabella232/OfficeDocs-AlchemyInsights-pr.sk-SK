---
title: Blokovanie e-mailových podpisov vytvorených používateľmi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483366"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="647d1-102">Blokovanie e-mailových podpisov vytvorených používateľmi</span><span class="sxs-lookup"><span data-stu-id="647d1-102">Block user-made email signatures</span></span>

<span data-ttu-id="647d1-103">Nasledujúce riešenie sa vzťahuje len na podpisy e-mailov vytvorené v Outlooku na webe.</span><span class="sxs-lookup"><span data-stu-id="647d1-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="647d1-104">Podpis môžete blokovať len v aplikácii Outlook, ak máte lokálny Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="647d1-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="647d1-105">V centre spravovania vyberte položku **Exchange centra spravovania**  >  .</span><span class="sxs-lookup"><span data-stu-id="647d1-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="647d1-106">Kliknite na položku **povolenia**  >  **politiky aplikácie Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="647d1-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="647d1-107">Vyberte politiku a potom kliknite na ikonu ceruzky, ktorú chcete upraviť.</span><span class="sxs-lookup"><span data-stu-id="647d1-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="647d1-108">Kliknite na položku **funkcie**  >  **Ďalšie možnosti**.</span><span class="sxs-lookup"><span data-stu-id="647d1-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="647d1-109">V časti **používateľské prostredie** zrušte začiarknutie políčka **podpis e-mailu** a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="647d1-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="647d1-110">**Dôležité:** Ak ste pred zrušením začiarknutia tohto políčka pridali podpis, používateľ ho bude môcť naďalej používať.</span><span class="sxs-lookup"><span data-stu-id="647d1-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="647d1-111">Požiadajte ich, aby ho odstránili.</span><span class="sxs-lookup"><span data-stu-id="647d1-111">Ask them to remove it.</span></span>

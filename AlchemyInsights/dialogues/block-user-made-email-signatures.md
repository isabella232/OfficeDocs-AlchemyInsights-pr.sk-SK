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
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243634"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="bd8ea-102">Blokovanie e-mailových podpisov vytvorených používateľmi</span><span class="sxs-lookup"><span data-stu-id="bd8ea-102">Block user-made email signatures</span></span>

<span data-ttu-id="bd8ea-103">Nasledujúce riešenie sa vzťahuje len na podpisy e-mailov vytvorené v Outlooku na webe.</span><span class="sxs-lookup"><span data-stu-id="bd8ea-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="bd8ea-104">Podpis môžete blokovať len v aplikácii Outlook, ak máte lokálny Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="bd8ea-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="bd8ea-105">V centre spravovania vyberte položku **Exchange centra spravovania**  >  .</span><span class="sxs-lookup"><span data-stu-id="bd8ea-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="bd8ea-106">Kliknite na položku **povolenia**  >  **politiky aplikácie Outlook Web App**.</span><span class="sxs-lookup"><span data-stu-id="bd8ea-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="bd8ea-107">Vyberte politiku a potom kliknite na ikonu ceruzky, ktorú chcete upraviť.</span><span class="sxs-lookup"><span data-stu-id="bd8ea-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="bd8ea-108">Kliknite na položku **funkcie**  >  **Ďalšie možnosti**.</span><span class="sxs-lookup"><span data-stu-id="bd8ea-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="bd8ea-109">V časti **používateľské prostredie** zrušte začiarknutie políčka **podpis e-mailu** a potom kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="bd8ea-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="bd8ea-110">**Dôležité:** Ak ste pred zrušením začiarknutia tohto políčka pridali podpis, používateľ ho bude môcť naďalej používať.</span><span class="sxs-lookup"><span data-stu-id="bd8ea-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="bd8ea-111">Požiadajte ich, aby ho odstránili.</span><span class="sxs-lookup"><span data-stu-id="bd8ea-111">Ask them to remove it.</span></span>

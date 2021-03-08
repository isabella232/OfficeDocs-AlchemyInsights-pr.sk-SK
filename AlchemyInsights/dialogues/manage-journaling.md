---
title: Spravovanie denníkov
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: 2fcd0f386d2da8cad19fcc9872482bb75fe00dd2
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526145"
---
# <a name="manage-journaling"></a><span data-ttu-id="c1b92-102">Spravovanie denníkov</span><span class="sxs-lookup"><span data-stu-id="c1b92-102">Manage journaling</span></span>

<span data-ttu-id="c1b92-103">Denníky môžu pomôcť vašej organizácii reagovať na právne, regulačné a organizačné požiadavky na dodržiavanie súladu nahrávaním oznámení o prichádzajúcich a odchádzajúcich e-mailoch.</span><span class="sxs-lookup"><span data-stu-id="c1b92-103">Journaling can help your organization respond to legal, regulatory, and organizational compliance requirements by recording inbound and outbound email communications.</span></span> <span data-ttu-id="c1b92-104">Majte na pamäti:</span><span class="sxs-lookup"><span data-stu-id="c1b92-104">Keep in mind:</span></span>

* <span data-ttu-id="c1b92-105">Skôr ako budete môcť spravovať denníky, musíte mať povolenia na správu [organizácie](https://go.microsoft.com/fwlink/?linkid=2115259) a [správy záznamov](https://go.microsoft.com/fwlink/?linkid=2115469) .</span><span class="sxs-lookup"><span data-stu-id="c1b92-105">You need to have [Organization Management](https://go.microsoft.com/fwlink/?linkid=2115259) and [Records Management](https://go.microsoft.com/fwlink/?linkid=2115469) permissions before you can manage journaling.</span></span>
* <span data-ttu-id="c1b92-106">Musíte mať poštovú schránku denníka a (voliteľne) nakonfigurovanú poštovú schránku s alternatívnymi denníkmi.</span><span class="sxs-lookup"><span data-stu-id="c1b92-106">You need to have a journal mailbox and (optionally) an alternate journaling mailbox configured.</span></span> <span data-ttu-id="c1b92-107">Ďalšie informácie nájdete v téme [Konfigurácia denníkov v službe Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span><span class="sxs-lookup"><span data-stu-id="c1b92-107">To learn more, see [Configure Journaling in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2115260).</span></span>
* <span data-ttu-id="c1b92-108">V službe Exchange Online je k dispozícii obmedzenie počtu pravidiel denníkov, ktoré môžete vytvoriť.</span><span class="sxs-lookup"><span data-stu-id="c1b92-108">In Exchange Online, there's a limit to the number of journal rules that you can create.</span></span> <span data-ttu-id="c1b92-109">Podrobnosti nájdete v téme [Denník, doprava a obmedzenia pravidiel pre doručenú poštu](https://go.microsoft.com/fwlink/?linkid=2115261).</span><span class="sxs-lookup"><span data-stu-id="c1b92-109">For details, see [Journal, transport, and inbox rule limits](https://go.microsoft.com/fwlink/?linkid=2115261).</span></span>
* <span data-ttu-id="c1b92-110">Exchange Online nepodporuje doručovanie zostáv denníka do poštovej schránky služby Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="c1b92-110">Exchange Online doesn't support delivering journal reports to an Exchange Online mailbox.</span></span> <span data-ttu-id="c1b92-111">Je nutné zadať e-mailovú adresu lokálneho systému archivácie alebo služby archivácie tretích strán ako poštovej schránky denníkov.</span><span class="sxs-lookup"><span data-stu-id="c1b92-111">You must specify the email address of an on-premises archiving system or a third-party archiving service as the journaling mailbox.</span></span>

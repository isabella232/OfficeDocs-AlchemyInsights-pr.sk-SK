---
title: Príklad Microsoft Defendera pre politiku bezpečného pripojenia služieb Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749197"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="7af8f-102">Príklad Microsoft Defendera pre politiku bezpečného pripojenia služieb Office 365</span><span class="sxs-lookup"><span data-stu-id="7af8f-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="7af8f-103">Tieto nastavenia umožňujú politiku s názvom *žiadne oneskorenia* , ktoré okamžite doručujú správy a potom po ich naskenovaní opätovne priloží prílohy:</span><span class="sxs-lookup"><span data-stu-id="7af8f-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="7af8f-104">**Názov**: žiadne oneskorenia</span><span class="sxs-lookup"><span data-stu-id="7af8f-104">**Name**: No delays</span></span>
- <span data-ttu-id="7af8f-105">**Popis**: doručí správy okamžite a opätovne priloží prílohy po kontrole.</span><span class="sxs-lookup"><span data-stu-id="7af8f-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="7af8f-106">**Odpoveď**: vyberte možnosť **dynamické doručenie** .</span><span class="sxs-lookup"><span data-stu-id="7af8f-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="7af8f-107">Ďalšie informácie nájdete v téme [dynamické doručenie v zásadách bezpečných príloh](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="7af8f-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="7af8f-108">Sekcia **presmerovať prílohu** : vyberte možnosť na **povolenie presmerovania** a potom zadajte e-mailovú adresu globálneho správcu služieb Microsoft 365, správcu zabezpečenia alebo bezpečnostného analytika, ktorý bude skúmať nebezpečné prílohy.</span><span class="sxs-lookup"><span data-stu-id="7af8f-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="7af8f-109">**Použiť na** sekciu: vyberte **doménu príjemcu** a potom vyberte svoju doménu.</span><span class="sxs-lookup"><span data-stu-id="7af8f-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="7af8f-110">Vyberte položku **Pridať** a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="7af8f-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="7af8f-111">Po dokončení vyberte položku **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="7af8f-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="7af8f-112">Ďalšie informácie nájdete v téme [bezpečné prílohy v programe Microsoft Defender pre Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="7af8f-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>

---
title: Oprava politiky nájomníka (prepísanie akcie)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748989"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="76bba-102">Oprava politiky nájomníka (prepísanie akcie)</span><span class="sxs-lookup"><span data-stu-id="76bba-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="76bba-103">Táto správa ovplyvnila politiku ochrany pred nevyžiadanou poštou v nájomníkovi.</span><span class="sxs-lookup"><span data-stu-id="76bba-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="76bba-104">Ak chcete skontrolovať politiku, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="76bba-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="76bba-105">Prejdite na [centrum dodržiavania súladu pre Office 365 Security &](https://go.microsoft.com/fwlink/p/?linkid=2077143)a potom **prejdite do časti**  >    >  [Ochrana pred nevyžiadanou poštou](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="76bba-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="76bba-106">Ak chcete zistiť, či **zdroj politiky** označuje nasledovné:  **Pridať-XHeader/ModifySubject/redirect/Delete/žiadna akcia/skrytá správa**</span><span class="sxs-lookup"><span data-stu-id="76bba-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="76bba-107">Ak áno, na karte **vlastné** skontrolujte nastavenie politiky, ktorá ovplyvnila správu.</span><span class="sxs-lookup"><span data-stu-id="76bba-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="76bba-108">Je možné, že **štandardné nastavenia** aplikované na všetkých zákazníkov služby Exchange Online Protection ovplyvnili správu.</span><span class="sxs-lookup"><span data-stu-id="76bba-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="76bba-109">Ďalšie informácie o konfigurácii politiky filtrovania nevyžiadanej pošty nájdete v téme [Konfigurácia politiky filtrovania nevyžiadanej pošty](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="76bba-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>

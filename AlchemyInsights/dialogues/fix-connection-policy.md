---
title: Oprava politiky pripojenia
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695887"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="50bde-102">Oprava politiky pripojenia</span><span class="sxs-lookup"><span data-stu-id="50bde-102">Fix connection policy</span></span>

<span data-ttu-id="50bde-103">E-mail bol označený ako bezpečný a doručený do priečinka doručenej pošty používateľa, pretože odosielajúca IP adresa bola v politike filtra pripojenia označená ako bezpečná.</span><span class="sxs-lookup"><span data-stu-id="50bde-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="50bde-104">Ak chcete skontrolovať politiku, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="50bde-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="50bde-105">Prejdite na [centrum dodržiavania súladu pre Office 365 Security &](https://go.microsoft.com/fwlink/p/?linkid=2077143)a potom **prejdite do časti**  >    >  [Ochrana pred nevyžiadanou poštou](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="50bde-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="50bde-106">Na karte **vlastné** vyberte **politiku filtrovania pripojenia** a potom vyberte položku **upraviť politiku**.</span><span class="sxs-lookup"><span data-stu-id="50bde-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="50bde-107">Pozrite si zoznam **povolených IP adries** .</span><span class="sxs-lookup"><span data-stu-id="50bde-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="50bde-108">Skontrolujte, či je povolený **bezpečný zoznam** .</span><span class="sxs-lookup"><span data-stu-id="50bde-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="50bde-109">Spoločnosť Microsoft sa prihlási k zdrojom tretích strán dôveryhodných odosielateľov.</span><span class="sxs-lookup"><span data-stu-id="50bde-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="50bde-110">Ak je povolený **bezpečný zoznam** , títo Dôveryhodní odosielatelia nie sú omylom označení ako nevyžiadaná pošta.</span><span class="sxs-lookup"><span data-stu-id="50bde-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="50bde-111">Odporúčam vybrať túto možnosť, pretože zníži počet falošných poplachov (dobrá pošta klasifikovaná ako nevyžiadaná pošta), ktorá sa zobrazí.</span><span class="sxs-lookup"><span data-stu-id="50bde-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>

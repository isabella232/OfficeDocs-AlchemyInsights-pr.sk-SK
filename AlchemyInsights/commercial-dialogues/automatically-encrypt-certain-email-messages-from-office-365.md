---
title: Automatické šifrovanie niektorých e-mailových správ z balíka Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749457"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="24a6e-102">Automatické šifrovanie niektorých e-mailových správ z balíka Office 365</span><span class="sxs-lookup"><span data-stu-id="24a6e-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="24a6e-103">V [centre spravovania pre Exchange](https://outlook.office365.com/ecp/)vyberte položku **pravidlá toku pošty >**.</span><span class="sxs-lookup"><span data-stu-id="24a6e-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="24a6e-104">Kliknite na **novú ikonu (+)** a potom kliknite na položku **použiť šifrovanie správ v Office 365 a ochranu práv na správy**.</span><span class="sxs-lookup"><span data-stu-id="24a6e-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="24a6e-105">Do poľa **názov** zadajte názov pravidla, napríklad *šifrovať všetky správy*.</span><span class="sxs-lookup"><span data-stu-id="24a6e-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="24a6e-106">**Ak chcete použiť toto pravidlo**, vyberte možnosť **[použiť na všetky správy]**.</span><span class="sxs-lookup"><span data-stu-id="24a6e-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="24a6e-107">Vedľa poľa **vykonať** toto políčko kliknite na položku **vybrať jeden**.</span><span class="sxs-lookup"><span data-stu-id="24a6e-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="24a6e-108">V rozbaľovacej ponuke **Šablóna RMS** vyberte položku **šifrovať** a potom kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="24a6e-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="24a6e-109">(Ak sa táto možnosť nezobrazuje, znamená to, že váš plán nezahŕňa automatické šifrovanie.</span><span class="sxs-lookup"><span data-stu-id="24a6e-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="24a6e-110">Môžete ju však pridať!)</span><span class="sxs-lookup"><span data-stu-id="24a6e-110">But you can add it!)</span></span>
7. <span data-ttu-id="24a6e-111">Začiarknite políčko **Auditovať Toto pravidlo s úrovňou závažnosti** a potom vyberte požadovanú úroveň.</span><span class="sxs-lookup"><span data-stu-id="24a6e-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="24a6e-112">Ak vaša spoločnosť disponuje zmluvnými povinnosťami na odoslanie všetkých zašifrovaných e-mailov, odporúčam nastaviť úroveň na hodnotu **vysoká**.</span><span class="sxs-lookup"><span data-stu-id="24a6e-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="24a6e-113">V časti **Vyberte model pre toto pravidlo** kliknite na položku **vynútiť**.</span><span class="sxs-lookup"><span data-stu-id="24a6e-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="24a6e-114">Vyberte ľubovoľný voliteľný výber (zo zoznamu voliteľných výberov, ktoré môžete vykonať v tomto bode, pričom mnohé z nich možno ponechať s predvoleným nastavením pre jednoduchosť).</span><span class="sxs-lookup"><span data-stu-id="24a6e-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="24a6e-115">Kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="24a6e-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="24a6e-116">Vždy sa môžete vrátiť a upraviť toto pravidlo neskôr.</span><span class="sxs-lookup"><span data-stu-id="24a6e-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="24a6e-117">Ďalšie informácie o vytváraní pravidiel šifrovania nájdete v téme [definovanie pravidiel toku pošty na šifrovanie e-mailových správ v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="24a6e-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>


---
title: Automatické šifrovanie niektorých e-mailových správ v Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50526741"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="f5a1b-102">Automatické šifrovanie niektorých e-mailových správ v Office 365</span><span class="sxs-lookup"><span data-stu-id="f5a1b-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="f5a1b-103">Správy, ktoré používatelia odosielajú určitým externým osobám alebo organizáciám, môžete automaticky šifrovať.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="f5a1b-104">Ak to chcete urobiť, vykonajte tieto kroky:</span><span class="sxs-lookup"><span data-stu-id="f5a1b-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="f5a1b-105">V [centre spravovania pre Exchange](https://outlook.office365.com/ecp/)vyberte položku **pravidlá toku pošty >**.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="f5a1b-106">Kliknite na **novú ikonu (+)** a potom kliknite na položku **použiť šifrovanie správ v Office 365 a ochranu práv na správy**.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="f5a1b-107">Do poľa **názov** zadajte názov pravidla, napríklad *šifrovanie správ odoslaných do DrToniRamos@gmail.com*.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="f5a1b-108">**Ak chcete použiť toto pravidlo**, vyberte položku **príjemca > je touto osobou**.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="f5a1b-109">V okne **Výber členov** vyberte meno osoby, s ktorou chcete použiť pravidlo šifrovania, a potom kliknite na položku **Pridať**.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="f5a1b-110">Po dokončení pridávania používateľov kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="f5a1b-111">Vedľa poľa **vykonať** toto políčko kliknite na položku **vybrať jeden**.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="f5a1b-112">V rozbaľovacej ponuke **Šablóna RMS** vyberte položku **šifrovať** a potom kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="f5a1b-113">(Ak sa táto možnosť nezobrazuje, znamená to, že váš plán nezahŕňa automatické šifrovanie.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="f5a1b-114">Môžete ju však pridať!)</span><span class="sxs-lookup"><span data-stu-id="f5a1b-114">But you can add it!)</span></span>
9. <span data-ttu-id="f5a1b-115">Vyberte ľubovoľný voliteľný výber (zo zoznamu voliteľných výberov, ktoré môžete vykonať v tomto bode, pričom mnohé z nich možno ponechať s predvoleným nastavením pre jednoduchosť).</span><span class="sxs-lookup"><span data-stu-id="f5a1b-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="f5a1b-116">Kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f5a1b-117">Vždy sa môžete vrátiť a upraviť toto pravidlo neskôr.</span><span class="sxs-lookup"><span data-stu-id="f5a1b-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="f5a1b-118">Ďalšie informácie o vytváraní pravidiel šifrovania nájdete v téme [definovanie pravidiel toku pošty na šifrovanie e-mailových správ v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="f5a1b-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>


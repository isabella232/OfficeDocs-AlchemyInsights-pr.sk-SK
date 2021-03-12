---
title: Automatické šifrovanie e-mailových správ v Office 365 odoslaných do určitých domén
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749301"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="21164-102">Automatické šifrovanie e-mailových správ v Office 365 odoslaných do určitých domén</span><span class="sxs-lookup"><span data-stu-id="21164-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="21164-103">V [centre spravovania pre Exchange](https://outlook.office365.com/ecp/)vyberte položku **pravidlá toku pošty >**.</span><span class="sxs-lookup"><span data-stu-id="21164-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="21164-104">Kliknite na **novú ikonu (+)** a potom kliknite na položku **použiť šifrovanie správ v Office 365 a ochranu práv na správy**.</span><span class="sxs-lookup"><span data-stu-id="21164-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="21164-105">Do poľa **názov** zadajte názov pravidla, napríklad *šifrovanie správ odoslaných do contoso.com*.</span><span class="sxs-lookup"><span data-stu-id="21164-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="21164-106">**Ak chcete použiť toto pravidlo**, vyberte položku **príjemca > doména**.</span><span class="sxs-lookup"><span data-stu-id="21164-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="21164-107">Zadajte názov domény, napríklad **contoso.com**.</span><span class="sxs-lookup"><span data-stu-id="21164-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="21164-108">Kliknite na ikonu **Pridať (+)** a potom kliknite na **tlačidlo OK**.</span><span class="sxs-lookup"><span data-stu-id="21164-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="21164-109">Vedľa poľa **vykonať** toto políčko kliknite na položku **vybrať jeden**.</span><span class="sxs-lookup"><span data-stu-id="21164-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="21164-110">V rozbaľovacej ponuke **Šablóna RMS** vyberte položku **šifrovať** a potom kliknite na tlačidlo **OK**.</span><span class="sxs-lookup"><span data-stu-id="21164-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="21164-111">(Ak sa táto možnosť nezobrazuje, znamená to, že váš plán nezahŕňa automatické šifrovanie.</span><span class="sxs-lookup"><span data-stu-id="21164-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="21164-112">Môžete ju však pridať!)</span><span class="sxs-lookup"><span data-stu-id="21164-112">But you can add it!)</span></span>
9. <span data-ttu-id="21164-113">Vyberte ľubovoľný voliteľný výber (zo zoznamu voliteľných výberov, ktoré môžete vykonať v tomto bode, pričom mnohé z nich možno ponechať s predvoleným nastavením pre jednoduchosť).</span><span class="sxs-lookup"><span data-stu-id="21164-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="21164-114">Kliknite na tlačidlo **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="21164-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="21164-115">Vždy sa môžete vrátiť a upraviť toto pravidlo neskôr.</span><span class="sxs-lookup"><span data-stu-id="21164-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="21164-116">Ďalšie informácie o vytváraní pravidiel šifrovania nájdete v téme [definovanie pravidiel toku pošty na šifrovanie e-mailových správ v Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="21164-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>
---
title: Ako zakázať externé skupiny
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 11/15/2019
ms.locfileid: "36739508"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="6e2c2-102">Ako zakázať externé skupiny</span><span class="sxs-lookup"><span data-stu-id="6e2c2-102">How to disable External Groups</span></span>

<span data-ttu-id="6e2c2-103">Yammer externé správy používa pravidlá prenosu Exchange (ETRs), súbor proaktívne kontroly, aby sa zabránilo zdieľanie informácií spoločnosti.</span><span class="sxs-lookup"><span data-stu-id="6e2c2-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="6e2c2-104">S cieľom obmedziť používateľom vytvárať externé skupiny, musíte nakonfigurovať pravidlo prenosu Exchange (ETR) a potom nakonfigurovať sieť Yammer použiť pravidlo prenosu Exchange blokovať externé správy.</span><span class="sxs-lookup"><span data-stu-id="6e2c2-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="6e2c2-105">Po vytvorení pravidla Exchange Online admin Center, postupujte nasledovne nastaviť ETR použiť v nariekanie:</span><span class="sxs-lookup"><span data-stu-id="6e2c2-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="6e2c2-106">Prihláste sa na sieť Yammer ako overený správca a v **centre spravovania siete Yammer**prejdite na položku C **obsah a zabezpečenie zabezpečenia \> .**</span><span class="sxs-lookup"><span data-stu-id="6e2c2-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="6e2c2-107">V časti **externé správy**vyberte **vynútenie pravidiel Exchange Online Exchange Transport (ETRs) v nariekanie.**</span><span class="sxs-lookup"><span data-stu-id="6e2c2-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="6e2c2-108">Vyberte položku **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="6e2c2-108">Choose **Save**.</span></span>

<span data-ttu-id="6e2c2-109">Ďalšie informácie nájdete v téme [zakázanie externých správ v sieti Yammer siete](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="6e2c2-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  
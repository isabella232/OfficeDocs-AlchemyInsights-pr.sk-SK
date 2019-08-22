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
ms.openlocfilehash: 4683a71438ec31f9e9211404a9c66c4e45e0e1df
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/22/2019
ms.locfileid: "36540916"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="e3bf9-102">Ako zakázať externé skupiny</span><span class="sxs-lookup"><span data-stu-id="e3bf9-102">How to disable External Groups</span></span>

<span data-ttu-id="e3bf9-103">Yammer externých správ sa uplatňuje Exchange Transport pravidlá (Red), sadu aktívne kontroly na zabrániť zdieľaniu informácií spoločnosti.</span><span class="sxs-lookup"><span data-stu-id="e3bf9-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="e3bf9-104">S cieľom obmedziť používateľov od vytvorenia externé skupiny, musíte nakonfigurovať výmena pravidlo prenosu (ETR), a potom nakonfigurovať sieť Yammer používať Exchange dopravné pravidlo blokovať externých správ.</span><span class="sxs-lookup"><span data-stu-id="e3bf9-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="e3bf9-105">Akonáhle ste vytvorili pravidlo Exchange Online admin Center, postupujte nasledovne nastaviť ETR použiť v sieť Yammer:</span><span class="sxs-lookup"><span data-stu-id="e3bf9-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="e3bf9-106">Prihlásenie na sieť Yammer len overené a **Yammer admin center**, prejdite na C **obsahu a zabezpečenia \> nastavenia zabezpečenia.**</span><span class="sxs-lookup"><span data-stu-id="e3bf9-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="e3bf9-107">Podľa **Externých správ**, vyberte **presadiť vaše Exchange Online Exchange Transport pravidlá (Red) v nariekanie.**</span><span class="sxs-lookup"><span data-stu-id="e3bf9-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="e3bf9-108">Vyberte položku **Uložiť**.</span><span class="sxs-lookup"><span data-stu-id="e3bf9-108">Choose **Save**.</span></span>

<span data-ttu-id="e3bf9-109">Ďalšie informácie nájdete v téme [kontroly externých správ v sieti sieť Yammer s Exchange Transport pravidlá](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="e3bf9-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  
---
title: 'Riešenie problémov s hlasovou schránkou '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7564"
ms.openlocfilehash: a2d26da512838ae112c352fe21366074b69fa224
ms.sourcegitcommit: 3802f2f4db4f53a408a360187db67f2296448c21
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679103"
---
# <a name="troubleshooting-voicemail"></a><span data-ttu-id="d48a0-102">Riešenie problémov s hlasovou schránkou</span><span class="sxs-lookup"><span data-stu-id="d48a0-102">Troubleshooting Voicemail</span></span>

<span data-ttu-id="d48a0-103">Presvedčte sa, či je funkcia obsadené na obsadenie zámerná.</span><span class="sxs-lookup"><span data-stu-id="d48a0-103">Ensure that the Busy on Busy feature is intentional.</span></span>

<span data-ttu-id="d48a0-104">Ak táto funkcia nie je pre tohto používateľa potrebná:</span><span class="sxs-lookup"><span data-stu-id="d48a0-104">If this feature is not needed on this user:</span></span>

1. <span data-ttu-id="d48a0-105">Prejdite do [centra spravovania pre teams](https://admin.teams.microsoft.com/policies/calling).</span><span class="sxs-lookup"><span data-stu-id="d48a0-105">Go to [Teams Admin center](https://admin.teams.microsoft.com/policies/calling).</span></span>
1. <span data-ttu-id="d48a0-106">Na ľavej strane železnice navigácia politiky **hlasového**  >  **hovoru**  >  **spravovať politiky** na **volanie politiky**.</span><span class="sxs-lookup"><span data-stu-id="d48a0-106">On the left rail navigate **Voice** > **Calling policies** > **Manage Policies** on the **Calling Policy**.</span></span>
1. <span data-ttu-id="d48a0-107">Vyberte položku **Spravovať používateľov**.</span><span class="sxs-lookup"><span data-stu-id="d48a0-107">Select **Manage Users**.</span></span>
1. <span data-ttu-id="d48a0-108">Vyhľadanie používateľa a zmena volacej politiky na takú, ktorá je pri zaneprázdnení zaneprázdnená, **je k dispozícii, keď je hovor k dispozícii** **.**</span><span class="sxs-lookup"><span data-stu-id="d48a0-108">Search for user and change the Calling Policy to one that has **Busy on Busy is available when in a call** to **Off**.</span></span>
1. <span data-ttu-id="d48a0-109">Kliknite na tlačidlo **Použiť**.</span><span class="sxs-lookup"><span data-stu-id="d48a0-109">Click **Apply**.</span></span>
> [!NOTE]
> <span data-ttu-id="d48a0-110">Zmeny politiky môžu trvať až 24 hodín, kým sa replikujú.</span><span class="sxs-lookup"><span data-stu-id="d48a0-110">Changes to policies can take up to 24 hours to replicate.</span></span>

<span data-ttu-id="d48a0-111">Ďalšie informácie o tejto funkcii nájdete v téme: [zaneprázdnený pri obsadení je k dispozícii počas hovoru](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span><span class="sxs-lookup"><span data-stu-id="d48a0-111">For more information on this feature refer to: [Busy on Busy is available while in a call](https://docs.microsoft.com/microsoftteams/teams-calling-policy#busy-on-busy-is-available-while-in-a-call).</span></span>

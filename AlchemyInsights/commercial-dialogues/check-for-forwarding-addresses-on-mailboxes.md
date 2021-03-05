---
title: Kontrola preposielania adries v poštových schránkach
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483923"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="c5296-102">Kontrola preposielania adries v poštových schránkach</span><span class="sxs-lookup"><span data-stu-id="c5296-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="c5296-103">Niekedy hakeri presmerujú e-mailové správy používateľov, preto najprv skontrolujeme, či preposielate adresy a pravidlá poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="c5296-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="c5296-104">Potom skontrolujeme denníky auditu.</span><span class="sxs-lookup"><span data-stu-id="c5296-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="c5296-105">Tu je návod na kontrolu preposielania adries:</span><span class="sxs-lookup"><span data-stu-id="c5296-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="c5296-106">Vyberte položku **Používatelia**  >  **aktívni používatelia**.</span><span class="sxs-lookup"><span data-stu-id="c5296-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="c5296-107">Vyberte používateľa, ktorého konto bolo ohrozené.</span><span class="sxs-lookup"><span data-stu-id="c5296-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="c5296-108">V zobrazenom rozbaľovacom zozname rozbaľte položku **Nastavenie pošty** a potom kliknite na položku **Upraviť** na **preposielanie e-mailov**.</span><span class="sxs-lookup"><span data-stu-id="c5296-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="c5296-109">Odstráňte všetky preposielané adresy, ktoré nepoznáte.</span><span class="sxs-lookup"><span data-stu-id="c5296-109">Remove any forwarding addresses you don't recognize.</span></span>
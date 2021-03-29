---
title: Kontrola adries na preposielanie v poštových schránkach
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403326"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="e2e89-102">Kontrola adries na preposielanie v poštových schránkach</span><span class="sxs-lookup"><span data-stu-id="e2e89-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="e2e89-103">Niekedy hakeri preposielajú e-mailové správy používateľov sebe, preto najskôr skontrolujeme preposielanie adries a pravidiel v poštovej schránke.</span><span class="sxs-lookup"><span data-stu-id="e2e89-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="e2e89-104">Potom skontrolujeme denníky auditu.</span><span class="sxs-lookup"><span data-stu-id="e2e89-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="e2e89-105">Tu je postup kontroly adries na preposielanie:</span><span class="sxs-lookup"><span data-stu-id="e2e89-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="e2e89-106">Vyberte **položku Používatelia**  >  **Aktívni používatelia.**</span><span class="sxs-lookup"><span data-stu-id="e2e89-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="e2e89-107">Vyberte používateľa, ktorého konto bolo zneužiné.</span><span class="sxs-lookup"><span data-stu-id="e2e89-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="e2e89-108">V zobrazenom rozbaľovacom zozname rozbaľte položku Nastavenia pošty a **potom kliknite** na položku Upraviť pre **preposielanie** **e-mailov.**</span><span class="sxs-lookup"><span data-stu-id="e2e89-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="e2e89-109">Odstráňte všetky adresy na preposielanie, ktoré nepoznáte.</span><span class="sxs-lookup"><span data-stu-id="e2e89-109">Remove any forwarding addresses you don't recognize.</span></span>
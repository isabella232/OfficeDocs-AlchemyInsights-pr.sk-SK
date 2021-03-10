---
title: Oprava nastavení politiky používateľa alebo poštovej schránky
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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/09/2021
ms.locfileid: "50695902"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="a1200-102">Oprava nastavení politiky používateľa alebo poštovej schránky</span><span class="sxs-lookup"><span data-stu-id="a1200-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="a1200-103">Nastavenia nevyžiadanej pošty v poštovej schránke ovplyvnili túto správu.</span><span class="sxs-lookup"><span data-stu-id="a1200-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="a1200-104">Ak chcete skontrolovať nastavenia, postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="a1200-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="a1200-105">Spustite prostredie Exchange Management Shell.</span><span class="sxs-lookup"><span data-stu-id="a1200-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="a1200-106">Ďalšie informácie nájdete v téme [Otvorenie prostredia Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="a1200-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="a1200-107">Spustite tento príkaz (s použitím e-mailovej adresy používateľa):  **Get-mailboxjunkmailconfiguration-identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="a1200-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="a1200-108">Skontrolujte, či je e-mailová adresa odosielateľa súčasťou **TrustedSendersAndDomains** alebo **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="a1200-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="a1200-109">Ak sa e-mailová adresa nachádza v niektorom zo zoznamov, možno ju budete musieť odstrániť.</span><span class="sxs-lookup"><span data-stu-id="a1200-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="a1200-110">Ďalšie informácie nájdete v téme [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="a1200-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>

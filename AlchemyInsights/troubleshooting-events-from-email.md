---
title: Riešenie problémov s udalosťami z e-mailu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834854"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="4df61-102">Riešenie problémov s udalosťami z e-mailu</span><span class="sxs-lookup"><span data-stu-id="4df61-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="4df61-103">Overenie, či je funkcia pre poštovú schránku povolená: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="4df61-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="4df61-104">Potom si pozrite denníky Udalosti z **e-mailu Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="4df61-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="4df61-105">V denníkoch Udalosti z e-mailu vyhľadajte InternetMessageId, ktorý sa zhoduje s položkou v poštovej schránke.</span><span class="sxs-lookup"><span data-stu-id="4df61-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="4df61-106">Vlastnosť TrustScore určuje, či sa položka pridá alebo nie.</span><span class="sxs-lookup"><span data-stu-id="4df61-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="4df61-107">Udalosti sa pridajú len vtedy, ak sa na hodnotu TrustScore = "Trusted" (Dôveryhodné).</span><span class="sxs-lookup"><span data-stu-id="4df61-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="4df61-108">Vlastnosť TrustScore určuje vlastnosti SPF, Dkim alebo Dmarc, ktoré sa nachádza v hlavičke správy.</span><span class="sxs-lookup"><span data-stu-id="4df61-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="4df61-109">Ak chcete zobraziť tieto vlastnosti:</span><span class="sxs-lookup"><span data-stu-id="4df61-109">To view these properties:</span></span>

<span data-ttu-id="4df61-110">**Počítačová aplikácia Outlook**</span><span class="sxs-lookup"><span data-stu-id="4df61-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="4df61-111">Otvorenie položky</span><span class="sxs-lookup"><span data-stu-id="4df61-111">Open the item</span></span>
- <span data-ttu-id="4df61-112">File -> Properties -> Internet Headers</span><span class="sxs-lookup"><span data-stu-id="4df61-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="4df61-113">alebo</span><span class="sxs-lookup"><span data-stu-id="4df61-113">or</span></span>

<span data-ttu-id="4df61-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="4df61-114">**MFCMapi**</span></span>

- <span data-ttu-id="4df61-115">Prechod na položku v priečinku doručenej pošty</span><span class="sxs-lookup"><span data-stu-id="4df61-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="4df61-116">Vyhľadajte PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="4df61-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="4df61-117">Tieto vlastnosti sa určia a zaznamenajú počas prenosu a smerovania.</span><span class="sxs-lookup"><span data-stu-id="4df61-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="4df61-118">Ak chcete vyriešiť ďalšie problémy, možno bude potrebné pokračovať s podporou prenosu v oblasti zlyhania pri SPF, DKIM a.alebo DMARC.</span><span class="sxs-lookup"><span data-stu-id="4df61-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>
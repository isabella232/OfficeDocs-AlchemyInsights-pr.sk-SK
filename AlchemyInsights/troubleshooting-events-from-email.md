---
title: Riešenie problémov s udalosťami z e-mailu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658749"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="8b283-102">Riešenie problémov s udalosťami z e-mailu</span><span class="sxs-lookup"><span data-stu-id="8b283-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="8b283-103">Overenie funkcie je povolená pre poštovú schránku: **Get-EventsFromEmailConfiguration- <mailbox> identity**</span><span class="sxs-lookup"><span data-stu-id="8b283-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="8b283-104">Potom sa pozrite na denníky udalostí z e-mailov **export-MailboxDiagnosticLogs <mailbox> -zložka TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="8b283-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="8b283-105">V denníkoch udalostí z e-mailu vyhľadajte InternetMessageId, ktoré sa zhoduje s položkou v poštovej schránke.</span><span class="sxs-lookup"><span data-stu-id="8b283-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="8b283-106">Vlastnosť TrustScore určuje, či sa položka pridá alebo nie.</span><span class="sxs-lookup"><span data-stu-id="8b283-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="8b283-107">Udalosti sa pridajú iba v prípade, že TrustScore = "dôveryhodný".</span><span class="sxs-lookup"><span data-stu-id="8b283-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="8b283-108">TrustScore je určený vlastnosťami SPF, dkim alebo DMARC, ktoré sa nachádzajú v hlavičke správy.</span><span class="sxs-lookup"><span data-stu-id="8b283-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="8b283-109">Ak chcete zobraziť tieto vlastnosti:</span><span class="sxs-lookup"><span data-stu-id="8b283-109">To view these properties:</span></span>

<span data-ttu-id="8b283-110">**Počítačová verzia Outlooku**</span><span class="sxs-lookup"><span data-stu-id="8b283-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="8b283-111">Otvorenie položky</span><span class="sxs-lookup"><span data-stu-id="8b283-111">Open the item</span></span>
- <span data-ttu-id="8b283-112">Súbor – > vlastnosti – > internetové hlavičky</span><span class="sxs-lookup"><span data-stu-id="8b283-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="8b283-113">alebo</span><span class="sxs-lookup"><span data-stu-id="8b283-113">or</span></span>

<span data-ttu-id="8b283-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="8b283-114">**MFCMapi**</span></span>

- <span data-ttu-id="8b283-115">Prechod na položku v priečinku Doručená pošta</span><span class="sxs-lookup"><span data-stu-id="8b283-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="8b283-116">Vyhľadanie PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="8b283-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="8b283-117">Tieto vlastnosti sa určia a zaznamenávajú počas prepravy a smerovania.</span><span class="sxs-lookup"><span data-stu-id="8b283-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="8b283-118">Ďalšie riešenie problémov možno budete musieť spracovať prostredníctvom podpory prenosu informácií o zlyhaniach v SPF, DKIM a. alebo DMARC.</span><span class="sxs-lookup"><span data-stu-id="8b283-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>
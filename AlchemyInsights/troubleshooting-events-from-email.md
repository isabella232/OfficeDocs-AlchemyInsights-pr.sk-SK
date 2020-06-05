---
title: Riešenie problémov s udalosťami z e-mailu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569404"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="555d4-102">Riešenie problémov s udalosťami z e-mailu</span><span class="sxs-lookup"><span data-stu-id="555d4-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="555d4-103">Overte, či je zapnutá funkcia pre poštovú schránku: \*\*Get-EventsFromEmailConfiguration -Identity <mailbox> \*\*</span><span class="sxs-lookup"><span data-stu-id="555d4-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="555d4-104">Potom sa pozrite na "Udalosti z e-mailu" prihlási **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="555d4-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="555d4-105">V denníkoch "Udalosti z e-mailu" vyhľadajte InternetMessageId, ktorý zodpovedá položke v poštovej schránke.</span><span class="sxs-lookup"><span data-stu-id="555d4-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="555d4-106">TrustScore určuje, či je položka pridaná alebo nie.</span><span class="sxs-lookup"><span data-stu-id="555d4-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="555d4-107">Udalosti sa pridajú iba v prípade, že trustscore = "Dôveryhodný".</span><span class="sxs-lookup"><span data-stu-id="555d4-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="555d4-108">TrustScore je určený SPF, Dkim alebo Dmarc vlastnosti, ktoré sú v hlavičke správy.</span><span class="sxs-lookup"><span data-stu-id="555d4-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="555d4-109">Ak chcete zobraziť tieto vlastnosti:</span><span class="sxs-lookup"><span data-stu-id="555d4-109">To view these properties:</span></span>

<span data-ttu-id="555d4-110">**Výhľad na pracovnú plochu**</span><span class="sxs-lookup"><span data-stu-id="555d4-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="555d4-111">Otvorenie položky</span><span class="sxs-lookup"><span data-stu-id="555d4-111">Open the item</span></span>
- <span data-ttu-id="555d4-112">Súbor -> Vlastnosti -> Internetové hlavičky</span><span class="sxs-lookup"><span data-stu-id="555d4-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="555d4-113">Alebo</span><span class="sxs-lookup"><span data-stu-id="555d4-113">or</span></span>

<span data-ttu-id="555d4-114">**Mfcmapi**</span><span class="sxs-lookup"><span data-stu-id="555d4-114">**MFCMapi**</span></span>

- <span data-ttu-id="555d4-115">Prechod na položku v doručenej pošte</span><span class="sxs-lookup"><span data-stu-id="555d4-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="555d4-116">Hľadajte PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="555d4-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="555d4-117">Tieto vlastnosti sa určujú a zaznamenávajú počas prepravy a smerovania.</span><span class="sxs-lookup"><span data-stu-id="555d4-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="555d4-118">Pre ďalšie riešenie problémov, budete musieť nadviazať s podporou prenosu o zlyhania sPF, DKIM a.alebo DMARC.</span><span class="sxs-lookup"><span data-stu-id="555d4-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>
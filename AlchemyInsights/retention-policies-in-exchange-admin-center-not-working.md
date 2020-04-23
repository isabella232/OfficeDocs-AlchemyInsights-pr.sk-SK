---
title: Politiky uchovávania údajov v Exchange Admin Center nepracuje
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742448"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="a5ae2-102">Politiky uchovávania údajov v stredisku Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="a5ae2-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="a5ae2-103">**Problém:** Novovytvorené alebo aktualizované politiky uchovávania údajov Exchange Admin Center sa nevzťahujú na poštové schránky alebo položky sa nepremiestnia do archívnej poštovej schránky alebo odstránené.</span><span class="sxs-lookup"><span data-stu-id="a5ae2-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="a5ae2-104">**Príčiny:**</span><span class="sxs-lookup"><span data-stu-id="a5ae2-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="a5ae2-105">Môže to byť spôsobené tým, že **asistent pre spravované priečinky** nespracoval poštovú schránku používateľa.</span><span class="sxs-lookup"><span data-stu-id="a5ae2-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="a5ae2-106">Asistent pre spravované priečinky sa pokúša spracovať každú poštovú schránku v organizácii typu cloud raz za sedem dní.</span><span class="sxs-lookup"><span data-stu-id="a5ae2-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="a5ae2-107">Ak zmeníte značku uchovávania údajov alebo použijete inú politiku uchovávania údajov pre poštovú schránku, môžete počkať, kým asistent spravovaných priečinkov spracuje poštovú schránku, alebo môžete spustiť rutinu cmdlet Start-ManagedFolderAssistant na spustenie Asistenta pre spravované priečinky na spracovanie konkrétnej poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="a5ae2-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="a5ae2-108">Spustenie tejto rutiny cmdlet je užitočné pre testovanie alebo riešenie problémov politiky uchovávania údajov alebo nastavenia značky uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="a5ae2-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="a5ae2-109">Ďalšie informácie nájdete v téme [Spustenie Asistenta pre spravované priečinky](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="a5ae2-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="a5ae2-110">**Riešenie:** Spustite nasledovný príkaz na spustenie Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:</span><span class="sxs-lookup"><span data-stu-id="a5ae2-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="a5ae2-111">To môže nastať aj ak **RetentionHold** bola **povolená** v poštovej schránke.</span><span class="sxs-lookup"><span data-stu-id="a5ae2-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="a5ae2-112">Ak poštová schránka bola umiestnená na RetentionHold, politika uchovávania údajov v poštovej schránke nebude spracovaná počas tohto času.</span><span class="sxs-lookup"><span data-stu-id="a5ae2-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="a5ae2-113">Ďalšie informácie o nastavení RetentionHold nájdete: [zadržanie poštovej schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="a5ae2-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="a5ae2-114">**Riešenie:**</span><span class="sxs-lookup"><span data-stu-id="a5ae2-114">**Solution:**</span></span>
    
  - <span data-ttu-id="a5ae2-115">Skontrolujte stav RetentionHold nastavenie na konkrétnu poštovú schránku v [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="a5ae2-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="a5ae2-116">Spustite nasledovný príkaz na **Vypnutie** RetentionHold na konkrétnu poštovú schránku:</span><span class="sxs-lookup"><span data-stu-id="a5ae2-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="a5ae2-117">Teraz znova spustite Asistenta pre spravované priečinky:</span><span class="sxs-lookup"><span data-stu-id="a5ae2-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="a5ae2-118">**Poznámka:** Ak je poštová schránka menšia ako 10 MB, Asistent pre spravované priečinky nebude automaticky spracovávať poštovú schránku.</span><span class="sxs-lookup"><span data-stu-id="a5ae2-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="a5ae2-119">Ďalšie informácie o politikách uchovávania údajov v centre spravovania servera Exchange nájdete v téme:</span><span class="sxs-lookup"><span data-stu-id="a5ae2-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="a5ae2-120">Značky uchovávania údajov a politiky uchovávania údajov</span><span class="sxs-lookup"><span data-stu-id="a5ae2-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="a5ae2-121">Použitie politiky uchovávania údajov pre poštové schránky</span><span class="sxs-lookup"><span data-stu-id="a5ae2-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="a5ae2-122">Pridanie alebo odstránenie značiek uchovávania údajov</span><span class="sxs-lookup"><span data-stu-id="a5ae2-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="a5ae2-123">Ako identifikovať typ hold umiestnené v poštovej schránke</span><span class="sxs-lookup"><span data-stu-id="a5ae2-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)

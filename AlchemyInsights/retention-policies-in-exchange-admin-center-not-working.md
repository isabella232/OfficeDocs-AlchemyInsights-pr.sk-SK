---
title: Politiky uchovávania údajov v centre spravovania pre Exchange nefunguje
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740525"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="ffdc4-102">Politiky uchovávania údajov v centre spravovania pre Exchange</span><span class="sxs-lookup"><span data-stu-id="ffdc4-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="ffdc4-103">Ak chcete, aby sme spustili automatizované kontroly nižšie uvedených nastavení, vyberte tlačidlo späť < – v hornej časti tejto stránky a potom zadajte e-mailovú adresu používateľa, ktorý má problémy s politikami uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="ffdc4-104">**Problém:** Novo vytvorené alebo aktualizované politiky uchovávania údajov v centre spravovania pre Exchange sa nevzťahujú na poštové schránky ani položky, ktoré nie sú presunuté do archívnej poštovej schránky alebo odstránené.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="ffdc4-105">**Hlavné príčiny:**</span><span class="sxs-lookup"><span data-stu-id="ffdc4-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="ffdc4-106">Môže to byť spôsobené tým, že **asistent pre spravované priečinky** nespracoval poštovú schránku používateľa.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="ffdc4-107">Asistent pre spravované priečinky sa po každých siedmich dňoch pokúsi spracovať každú poštovú schránku v organizácii využívajúcej cloud.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="ffdc4-108">Ak zmeníte značku uchovávania údajov alebo použijete inú politiku uchovávania údajov pre poštovú schránku, môžete počkať, kým spravovaný priečinok spracuje poštovú schránku, alebo môžete spustiť rutinu typu cmdlet Start-ManagedFolderAssistant a spustiť Asistenta pre spravované priečinky na spracovanie konkrétnej poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="ffdc4-109">Spustenie tejto rutiny typu cmdlet je užitočné pri testovaní alebo riešení problémov s nastaveniami politiky uchovávania údajov alebo značky uchovávania údajov.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="ffdc4-110">Ďalšie informácie nájdete v téme [Spustenie Asistenta pre spravované priečinky](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="ffdc4-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="ffdc4-111">**Riešenie:** Spustite nasledujúci príkaz na spustenie Asistenta pre spravované priečinky pre konkrétnu poštovú schránku:</span><span class="sxs-lookup"><span data-stu-id="ffdc4-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="ffdc4-112">Môže sa to vyskytnúť aj v prípade, ak je **RetentionHold** **zapnutá** v poštovej schránke.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="ffdc4-113">Ak je poštová schránka umiestnená na RetentionHold, politika uchovávania údajov v poštovej schránke sa počas tohto času nespracuje.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="ffdc4-114">Ďalšie informácie o inštalácii v nastaveniach RetentionHold nájdete v téme: [uchovanie poštovej schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="ffdc4-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="ffdc4-115">**Riešenie**</span><span class="sxs-lookup"><span data-stu-id="ffdc4-115">**Solution:**</span></span>
    
  - <span data-ttu-id="ffdc4-116">Skontrolujte stav nastavenia RetentionHold v konkrétnej poštovej schránke v [prostredí EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="ffdc4-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="ffdc4-117">Spustite tento príkaz na **Vypnutie** RetentionHold v konkrétnej poštovej schránke:</span><span class="sxs-lookup"><span data-stu-id="ffdc4-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="ffdc4-118">Teraz znova spustite Asistenta pre spravované priečinky:</span><span class="sxs-lookup"><span data-stu-id="ffdc4-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="ffdc4-119">**Poznámka:** Ak je poštová schránka menšia než 10 MB, Asistent pre spravované priečinky automaticky nespracuje poštovú schránku.</span><span class="sxs-lookup"><span data-stu-id="ffdc4-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="ffdc4-120">Ďalšie informácie o politikách uchovávania údajov v centre spravovania pre Exchange nájdete v témach:</span><span class="sxs-lookup"><span data-stu-id="ffdc4-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="ffdc4-121">Značky uchovávania údajov a politiky uchovávania údajov</span><span class="sxs-lookup"><span data-stu-id="ffdc4-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="ffdc4-122">Použitie politiky uchovávania údajov v poštových schránkach</span><span class="sxs-lookup"><span data-stu-id="ffdc4-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="ffdc4-123">Pridanie alebo odstránenie značiek uchovávania údajov</span><span class="sxs-lookup"><span data-stu-id="ffdc4-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="ffdc4-124">Ako identifikovať typ zadržania umiestneného v poštovej schránke</span><span class="sxs-lookup"><span data-stu-id="ffdc4-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)

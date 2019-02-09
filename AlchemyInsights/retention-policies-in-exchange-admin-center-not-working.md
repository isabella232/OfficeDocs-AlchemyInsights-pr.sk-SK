---
title: Politiky uchovávania údajov v Exchange Admin Center nefunguje
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786785"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="9e36f-102">Politiky uchovávania údajov v Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="9e36f-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="9e36f-103">**Problém:** Novo vytvorené alebo aktualizované Retenčná politika v centre výmenu Admin nie sú uplatnenie k poštovým schránkam alebo položky nie sú presunuté do archívnej poštovej schránky alebo odstránené.</span><span class="sxs-lookup"><span data-stu-id="9e36f-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="9e36f-104">**Príčiny:**</span><span class="sxs-lookup"><span data-stu-id="9e36f-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="9e36f-p101">To môže byť, pretože **Asistent spravovaných priečinkov** nebola spracovaná poštovej schránky používateľa. Asistent pre spravované priečinky snaží spracovať každú poštovú schránku organizácii cloud raz za každých sedem dní. Ak zmeníte značku uchovávania údajov alebo použijete pre poštovú schránku inú politiku uchovávania údajov, môžete počkať, kým riadené priečinok Assist spracuje údaje poštovej schránky, alebo môžete spustiť Štart-ManagedFolderAssistant cmdlet spustiť Asistenta pre spravované priečinky spracovať konkrétne Poštová schránka. Spustenie tejto rutiny cmdlet je užitočné pri testovaní politiky uchovávania údajov a nastavení značky uchovávania údajov pri riešení problémov. Pre viac informácií, navštívte [Spustenie Asistenta pre spravované priečinky](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="9e36f-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="9e36f-110">**Riešenie:** Spustite nasledovný príkaz na spustenie Asistenta pre spravované priečinky v konkrétnej poštovej schránke:</span><span class="sxs-lookup"><span data-stu-id="9e36f-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="9e36f-p102">To môže nastať aj ak **RetentionHold** bolo **zapnuté** poštovej schránky. Ak poštovú schránku bol kladený na RetentionHold, politiku uchovávania údajov poštovej schránky nebudú spracované počas tejto doby. Pre ďalšie informácie pozri Nastavenie RetentionHold: [Zadržania uchovávania údajov poštovej schránky](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="9e36f-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="9e36f-114">**Riešenie:**</span><span class="sxs-lookup"><span data-stu-id="9e36f-114">**Solution:**</span></span>
    
  - <span data-ttu-id="9e36f-115">Skontrolujte stav RetentionHold nastavenia špecifické schránky v [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="9e36f-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="9e36f-116">Spustite nasledujúci príkaz **vypnúť** RetentionHold na špecifické schránky:</span><span class="sxs-lookup"><span data-stu-id="9e36f-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="9e36f-117">Teraz znova spustiť spravované priečinok asistent:</span><span class="sxs-lookup"><span data-stu-id="9e36f-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="9e36f-118">**Poznámka:** Ak poštová schránka je menšie ako 10 MB, Asistent pre spravované priečinky automaticky nespracováva poštovú schránku.</span><span class="sxs-lookup"><span data-stu-id="9e36f-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  


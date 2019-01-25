---
title: Presunúť e-mailových správ do archívnej poštovej schránky
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 01/24/2019
ms.locfileid: "29488813"
---
<span data-ttu-id="475f1-p101">Problémy pri archivácii sa položky do archívnej poštovej schránky. Uistite sa, že ste vykonali nasledujúce kroky:</span><span class="sxs-lookup"><span data-stu-id="475f1-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="475f1-p102">Potvrdiť, že bola povolená **archivácia poštovej schránky** . Ak nie, použite kroky v [tomto článku](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) na zapnutie archívnej poštovej schránky.</span><span class="sxs-lookup"><span data-stu-id="475f1-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="475f1-106">V službe Exchange Admin Center, vyberte **Značky uchovávania údajov** podľa **Riadenia dodržiavania súladu**, vytvoriť **značku uchovávania údajov** s **premiestniť do archívu** akcie obsahujúce požadované **Obmedzenie veku uchovávania**.</span><span class="sxs-lookup"><span data-stu-id="475f1-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="475f1-107">Exchange Admin Center, vyberte **Politiky uchovávania údajov**, vytvoriť **Politiku uchovávania údajov** a pridať vaše **premiestniť do archívu** značky uchovávania údajov do tejto politiky.</span><span class="sxs-lookup"><span data-stu-id="475f1-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="475f1-p103">[Priradenie politiky uchovávania údajov](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštovej schránky špecifické používateľa. **Primárnej** a **archívnej** poštovej schránky sa použije rovnakú politiku.</span><span class="sxs-lookup"><span data-stu-id="475f1-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="475f1-p104">Poštová schránka používateľa teraz mali mať politiku archivácie premiestnite položky do archívnej poštovej schránky. Môže byť potrebné prinútiť podarilo priečinka asistent (MFA) spustiť a použiť nové nastavenia do poštovej schránky používateľa. Spustite nasledujúci príkaz zároveň [pripojený k EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) spustiť Asistenta pre spravované priečinky v konkrétnej poštovej schránke:</span><span class="sxs-lookup"><span data-stu-id="475f1-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="475f1-113">Chcete sa dozvedieť viac o nastavení politiku archivácie, pozri [nastaviť Archív a odstránenie politiky poštových schránok](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="475f1-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  


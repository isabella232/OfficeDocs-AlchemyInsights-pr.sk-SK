---
title: Nastaviť alebo zmeniť povolenia pre verejný priečinok
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 8/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: cffdf9bf-34ce-40f6-a69e-d02f17d9caef
ms.openlocfilehash: e4e98ba3e7dff2bd86be4667d7262c9544f9c9cb
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/12/2019
ms.locfileid: "29899223"
---
# <a name="permissions-and-public-folders"></a><span data-ttu-id="ab58e-102">Povolenia a verejné priečinky</span><span class="sxs-lookup"><span data-stu-id="ab58e-102">Permissions and Public Folders</span></span>

<span data-ttu-id="ab58e-103">Môžete zmeniť povolenia na verejné priečinky pomocou programu Outlook, Exchange admin center (EAC) alebo prostredie PowerShell:</span><span class="sxs-lookup"><span data-stu-id="ab58e-103">You can change the permissions on your Public Folders using Outlook, the Exchange admin center (EAC), or PowerShell:</span></span>
  
- <span data-ttu-id="ab58e-104">Outlook návod, [kliknite sem](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span><span class="sxs-lookup"><span data-stu-id="ab58e-104">For Outlook instructions, [click here](https://support.office.com/article/Set-or-change-permissions-for-a-public-folder-b2e0440c-7873-48ec-9ff2-b1a20b723005.aspx).</span></span>
    
- <span data-ttu-id="ab58e-p101">EAC, nájdete v [tomto článku](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) pre pokyny. Kliknutím [sem](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) prejdete do EAC.</span><span class="sxs-lookup"><span data-stu-id="ab58e-p101">For EAC, refer to [this article](https://technet.microsoft.com/library/jj651147%28v=exchg.150%29.aspx.aspx#Anchor_1) for instructions. You can click [here](https://support.office.com/article/ https://outlook.office365.com/ecp/.aspx) to navigate to EAC.</span></span> 
    
- <span data-ttu-id="ab58e-p102">Powershell, nájdete [Tento článok](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) pokyny pre používanie rutiny prostredia Add-PublicFolderClientPermission. Ak potrebujete pokyny na pripojenie k Exchange Powershell, kliknite [tu](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span><span class="sxs-lookup"><span data-stu-id="ab58e-p102">For Powershell, refer to [this article](https://technet.microsoft.com/library/bb124743%28v=exchg.160%29.aspx.aspx) for instructions on using the Add-PublicFolderClientPermission commandlet. If you need instructions to connect to Exchange Powershell, click [here](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx.aspx).</span></span>
    
<span data-ttu-id="ab58e-p103">Ak sa **Externí používatelia nemôžete posielať e-mailov do e-mailu verejných priečinkov**, dôvodom môže byť verejný priečinok chýba povolenia potrebné pre externý e-mail doručenie. Môžete opraviť pomocou Outlook návod [tu](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), alebo pokynov PowerShell [tu](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span><span class="sxs-lookup"><span data-stu-id="ab58e-p103">If **external users can't send emails to a mail-enabled Public Folder**, the reason might be that the public folder is missing permissions required for external email delivery. You can fix this using the Outlook instructions [here](https://technet.microsoft.com/library/aa997560%28v=exchg.150%29.aspx.aspx#Anchor_1), or the PowerShell instructions [here](https://support.microsoft.com/help/2984402/-5.7.1-smtp-550-5.7.1-resolver.rst.authrequired-nondelivery-report-when-external-users-try-to-send-mail-to-mail-enabled-public-folders-in-office-365.aspx).</span></span>
  


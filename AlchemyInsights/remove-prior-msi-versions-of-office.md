---
title: Odstrániť predchádzajúce verzie MSI balíka Office
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680732"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="b2c72-102">Odstrániť predchádzajúce verzie MSI balíka Office</span><span class="sxs-lookup"><span data-stu-id="b2c72-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="b2c72-103">Pred inštaláciou balíka Office 365 ProPlus odporúčame odstrániť predchádzajúce verzie balíka Office s Inštalátorom systému Windows (MSI).</span><span class="sxs-lookup"><span data-stu-id="b2c72-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="b2c72-104">Postupujte takto:</span><span class="sxs-lookup"><span data-stu-id="b2c72-104">Here's how to do this:</span></span>

1. <span data-ttu-id="b2c72-105">Ak ste použili inštalátor MSI na inštaláciu balíka Office, môžete na odinštalovanie balíka Office použiť nástroj na nasadenie balíka Office (ODT).</span><span class="sxs-lookup"><span data-stu-id="b2c72-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="b2c72-106">V súbore **configuration.xml** môžete použiť prvok RemoveMSI.</span><span class="sxs-lookup"><span data-stu-id="b2c72-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="b2c72-107">Postupujte podľa pokynov v tomto článku: [centrum dodržiavania súladu & zabezpečenia balíka Office 365.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="b2c72-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>
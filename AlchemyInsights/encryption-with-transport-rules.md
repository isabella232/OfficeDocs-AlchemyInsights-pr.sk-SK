---
title: Šifrovanie s pravidlami prenosu
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
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813883"
---
# <a name="encryption-with-transport-rules"></a><span data-ttu-id="ce8bd-102">Šifrovanie s pravidlami prenosu</span><span class="sxs-lookup"><span data-stu-id="ce8bd-102">Encryption with transport rules</span></span>

<span data-ttu-id="ce8bd-103">V centre [spravovania pre Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) môžete používať funkcie šifrovanie správ v Office (OME) v pravidlách toku pošty na spustenie šifrovania správ.</span><span class="sxs-lookup"><span data-stu-id="ce8bd-103">In the [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC), you can use Office Message Encryption(OME) capabilities in your mail flow rules to trigger message encryption.</span></span> <span data-ttu-id="ce8bd-104">V podmienke pravidla prenosu vyberte možnosť **Použiť šifrovanie správ v Office 365 a ochranu práv**.</span><span class="sxs-lookup"><span data-stu-id="ce8bd-104">Choose the **Apply Office 365 Message Encryption and rights protection** option on the Transport Rule condition.</span></span>

- <span data-ttu-id="ce8bd-105">Ďalšie informácie nájdete v téme [Definovanie pravidla toku pošty na šifrovanie](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span><span class="sxs-lookup"><span data-stu-id="ce8bd-105">For more information, see [Define Mail flow rule to encrypt](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

- <span data-ttu-id="ce8bd-106">V prostredí PowerShell použite rutinu typu cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) a nastavte parameter *ApplyOME* na možnosť $true.</span><span class="sxs-lookup"><span data-stu-id="ce8bd-106">In Powershell, use the [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet and set the *ApplyOME* parameter to $true.</span></span>

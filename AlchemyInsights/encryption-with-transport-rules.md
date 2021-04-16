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
# <a name="encryption-with-transport-rules"></a>Šifrovanie s pravidlami prenosu

V centre [spravovania pre Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) môžete používať funkcie šifrovanie správ v Office (OME) v pravidlách toku pošty na spustenie šifrovania správ. V podmienke pravidla prenosu vyberte možnosť **Použiť šifrovanie správ v Office 365 a ochranu práv**.

- Ďalšie informácie nájdete v téme [Definovanie pravidla toku pošty na šifrovanie](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- V prostredí PowerShell použite rutinu typu cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) a nastavte parameter *ApplyOME* na možnosť $true.

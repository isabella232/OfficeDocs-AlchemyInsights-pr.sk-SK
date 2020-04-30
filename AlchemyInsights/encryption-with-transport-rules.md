---
title: Šifrovanie s pravidlami prenosu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 3f16c7e7be99a50cd57f47ea2801b3022c4aec95
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915290"
---
# <a name="encryption-with-transport-rules"></a>Šifrovanie s pravidlami prenosu

V centre [spravovania pre Exchange](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) môžete používať funkcie šifrovanie správ v Office (OME) v pravidlách toku pošty na spustenie šifrovania správ. V podmienke pravidla prenosu vyberte možnosť **Použiť šifrovanie správ v Office 365 a ochranu práv**.

- Ďalšie informácie nájdete v téme [Definovanie pravidla toku pošty na šifrovanie](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- V prostredí PowerShell použite rutinu typu cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) a nastavte parameter *ApplyOME* na možnosť $true.

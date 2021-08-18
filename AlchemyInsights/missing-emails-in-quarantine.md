---
title: Chýbajúce e-maily v karanténe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: c77da6716c0755d6ed4911f490e000bd74d08f92
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329677"
---
# <a name="missing-emails-in-quarantine"></a>Chýbajúce e-maily v karanténe

Správcovia [môžu tieto správy zobraziť, uvoľniť alebo odstrániť](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Na portáli Microsoft 365 Defender prejdite na <https://security.microsoft.com> položku Skontrolovať  \> **karanténu**. Ak chcete prejsť priamo na stránku **Karanténa,** použite <https://security.microsoft.com/quarantine> .  

Ďalšie informácie o hodnotách vyhľadávania a filtrovania, ktoré môžete použiť, nájdete v téme Správa správ v karanténe a súborov [ako správca v rámci služby EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Rutiny typu cmdlet, ktoré používate na zobrazenie a spravovanie správ a súborov v karanténe, sú:

- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Táto rutina typu cmdlet je len pre správy, nie pre Trezor prílohy pre SharePoint, OneDrive alebo Microsoft Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)

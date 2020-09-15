---
title: Chýbajúce e-maily v karanténe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673729"
---
# <a name="missing-emails-in-quarantine"></a>Chýbajúce e-maily v karanténe

Správcovia môžu [tieto správy zobrazovať, uvoľňovať alebo odstraňovať.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Ak chcete otvoriť centrum zabezpečenia & dodržiavania súladu, prejdite na [https://protection.office.com](https://protection.office.com/) . Ak chcete otvoriť stránku karantény priamo, prejdite na položku [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Môžete vyhľadávať podľa nasledujúcich hodnôt:  

- **ID správy**: globálny jedinečný identifikátor správy. Ak v zozname vyberiete správu, na zobrazenej table s **podrobnosťami** sa zobrazí hodnota **ID správy** . Správcovia môžu použiť [sledovanie](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) správ na vyhľadanie správ a príslušných hodnôt identifikácie správ.
- **E-mailová adresa odosielateľa**: e-mailová adresa jedného odosielateľa.
- **E-mailová adresa príjemcu**: e-mailová adresa jedného príjemcu.
- **Predmet**: použite celý predmet správy. Vyhľadávanie nerozlišuje veľké a malé písmená.

Po zadaní kritérií vyhľadávania kliknite na položku Obnoviť ![ tlačidlo ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **obnoviť** a výsledky sa filtrujú.  

Rutiny typu cmdlet, ktoré používate na zobrazenie a spravovanie správ a súborov v karanténe, sú:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Ukážka – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Táto rutina typu cmdlet je len pre správy, nie malvérové súbory z ATP pre SharePoint Online, OneDrive for Business alebo teams.
- [Vydanie – QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
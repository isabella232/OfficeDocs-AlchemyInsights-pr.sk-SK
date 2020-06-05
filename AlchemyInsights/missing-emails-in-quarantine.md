---
title: Chýbajúce e-maily v karanténe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569559"
---
# <a name="missing-emails-in-quarantine"></a>Chýbajúce e-maily v karanténe"

Správcovia môžu [tieto správy zobraziť, uvoľniť alebo odstrániť.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Ak chcete otvoriť Centrum zabezpečenia & súladu, prejdite na položku [https://protection.office.com](https://protection.office.com/) . Ak chcete otvoriť stránku Karanténa priamo, prejdite na položku [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Môžete vyhľadávať podľa nasledujúcich hodnôt:  

- **Identifikácia správy:** Globálne jedinečný identifikátor správy. Ak vyberiete správu v zozname, hodnota **Id správy** sa zobrazí na table **Podrobnosti** rozbaľovacieho zoznamu, ktorá sa zobrazí. Správcovia môžu použiť [sledovanie správ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) na vyhľadanie správ a zodpovedajúcich hodnôt identifikácie správy.
- **E-mailová adresa odosielateľa**: E-mailová adresa jedného odosielateľa.
- **E-mailová adresa príjemcu:** e-mailová adresa jedného príjemcu.
- **Predmet**: Použite celý predmet správy. Pri vyhľadávaní sa nerozlišujú veľké a malé písmená.

Po zadaní kritérií vyhľadávania kliknutím na ![ tlačidlo Obnoviť kliknite na tlačidlo ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Obnoviť** a výsledky môžete filtrovať.  

Rutiny cmdlet, ktoré používate na zobrazenie a správu správ a súborov v karanténe, sú:
- [Odstrániť karanténuMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Získajte karanténuMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Všimnite si, že táto rutina cmdlet je len pre správy, nie malware súbory z ATP pre SharePoint Online, OneDrive pre podniky alebo tímy.
- [Správa o vydaní karantény](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
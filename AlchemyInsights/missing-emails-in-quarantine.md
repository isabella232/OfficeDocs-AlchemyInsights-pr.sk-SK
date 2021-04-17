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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831749"
---
# <a name="missing-emails-in-quarantine"></a>Chýbajúce e-maily v karanténe"

Správcovia [môžu tieto správy zobraziť, uvoľniť alebo odstrániť.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Ak chcete otvoriť Centrum zabezpečenia & zabezpečenia, prejdite na položku [https://protection.office.com](https://protection.office.com/) . Ak chcete stránku karantény otvoriť priamo, prejdite do ponuky [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Vyhľadávať môžete podľa nasledujúcich hodnôt:  

- **ID správy:** globálny jedinečný identifikátor správy. Ak vyberiete správu v zozname, na  **zobrazenej**  table Podrobnosti sa  **zobrazí**  hodnota ID správy. Správcovia môžu pomocou [sledovania správ](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) vyhľadať správy a ich zodpovedajúce hodnoty ID správy.
- **E-mailová adresa** odosielateľa: E-mailová adresa jedného odosielateľa.
- **E-mailová** adresa príjemcu: E-mailová adresa jedného príjemcu.
- **Predmet**: Použite celý predmet správy. Pri vyhľadávaní sa rozlišujú malé a veľké písmená.

Po zadaní kritérií vyhľadávania kliknite na tlačidlo Obnoviť a ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **vyfiltrujte** výsledky.  

Rutiny typu cmdlet, ktoré používate na zobrazenie a spravovanie správ a súborov v karanténe, sú:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)Táto rutina typu cmdlet je len pre správy, nie pre malvérové súbory z ATP pre SharePoint Online, OneDrive for Business alebo Teams.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)
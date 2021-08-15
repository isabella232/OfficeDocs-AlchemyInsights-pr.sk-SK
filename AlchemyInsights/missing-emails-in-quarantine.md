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
ms.openlocfilehash: 900d5f250846e9a7046f72156c150f4970d91d5ad94cb7fc054952228f4bf257
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026237"
---
# <a name="missing-emails-in-quarantine"></a>Chýbajúce e-maily v karanténe"

Správcovia [môžu tieto správy zobraziť, uvoľniť alebo odstrániť.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Ak chcete otvoriť Centrum zabezpečenia & zabezpečenia, prejdite na položku [https://protection.office.com](https://protection.office.com/) . Ak chcete stránku karantény otvoriť priamo, prejdite do ponuky [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Vyhľadávať môžete podľa nasledujúcich hodnôt:  

- **ID správy:** globálny jedinečný identifikátor správy. Ak vyberiete správu v zozname, na  **zobrazenej**  table Podrobnosti sa  **zobrazí**  hodnota ID správy. Správcovia môžu pomocou [sledovania správ](/microsoft-365/security/office-365-security/message-trace-scc) vyhľadať správy a ich zodpovedajúce hodnoty ID správy.
- **E-mailová adresa** odosielateľa: E-mailová adresa jedného odosielateľa.
- **E-mailová** adresa príjemcu: E-mailová adresa jedného príjemcu.
- **Predmet**: Použite celý predmet správy. Pri vyhľadávaní sa rozlišujú malé a veľké písmená.

Po zadaní kritérií vyhľadávania kliknite na tlačidlo Obnoviť a ![ ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **vyfiltrujte** výsledky.

Rutiny typu cmdlet, ktoré používate na zobrazenie a spravovanie správ a súborov v karanténe, sú:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage:](/powershell/module/exchange/preview-quarantinemessage)Táto rutina typu cmdlet je len pre správy, nie pre malvérové súbory z programu Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive for Business alebo Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)
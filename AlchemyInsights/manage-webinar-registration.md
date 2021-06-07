---
title: Správa registrácie webového seminára
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794148"
---
# <a name="manage-webinar-registration"></a>Správa registrácie webového seminára

Môžete spravovať, kto sa môže zaregistrovať Teams Webinári pomocou príkazov Teams PowerShell. Ak chcete nainštalovať Teams PowerShell, pozrite si [Teams PowerShell.](/microsoftteams/teams-powershell-install) 

Predvolene je funkcia *WhoCanRegister povolená* a nastavená na možnosť **EveryoneInCompany.** Ak chcete povoliť, aby sa ktokoľvek vrátane anonymných používateľov zaregistroval, pomocou príkazu Powershell **nastavte** politiku schôdze na možnosť Všetci:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Poznámka:** Ak je v nastaveniach schôdze vypnuté anonymné spojenie, anonymní používatelia sa môžu pripojiť k webovým seminárom. Ďalšie informácie a povolenie tohto nastavenia nájdete v téme [Správa nastavení schôdze v Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

Ak chcete vypnúť registráciu schôdze, nastavte položku *AllowMeetingRegistration na hodnotu* **False**.

Ďalšie informácie o konfigurácii toho, kto sa môže zaregistrovať pre webináry, nájdete v téme Konfigurácia, [kto sa môže zaregistrovať pre webové semináre.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Ďalšie informácie o nastaveniach pre Microsoft Lists nájdete v téme [Ovládanie nastavení pre zoznamy Microsoft.](/sharepoint/control-lists)

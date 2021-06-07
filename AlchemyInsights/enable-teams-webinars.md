---
title: Povolenie Teams webových seminárov
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/04/2021
ms.locfileid: "52794040"
---
# <a name="enable-teams-webinars"></a>Povolenie Teams webových seminárov

Webové semináre sú predvolene povolené. Pomocou príkazov prostredia PowerShell môžete spravovať, kto Teams a zaregistrovať pre Teams Teams Webinári.

- Všetci používatelia, ktorí môžu vytvoriť schôdzu, môžu tiež vytvoriť schôdzu z webového seminára. Ak chcete spravovať, kto môže plánovať Teams Webináre, použite *funkciu AllowMeetingRegistration*. 
- Predvolene je funkcia *WhoCanRegister povolená* a nastavená na možnosť **Všetci.** Ak chcete vypnúť registráciu schôdze, nastavte položku *AllowMeetingRegistration na hodnotu* **False**.

Ak chcete tieto nastavenia zmeniť, musíte nainštalovať [Teams prostredia PowerShell.](/microsoftteams/teams-powershell-install) Politiky schôdzí sa tiež vynútijú na Teams Webinári. Ak je napríklad v nastaveniach schôdze vypnuté anonymné spojenie, anonymní používatelia sa môžu pripojiť k webovým seminárom.

Ďalšie informácie o konfigurácii toho, kto sa môže zaregistrovať pre webináry, nájdete v téme Konfigurácia, [kto sa môže zaregistrovať pre webové semináre.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Ďalšie informácie o nastaveniach pre Microsoft Lists nájdete v téme [Ovládanie nastavení pre zoznamy Microsoft.](/sharepoint/control-lists)
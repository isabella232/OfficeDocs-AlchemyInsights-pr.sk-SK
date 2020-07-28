---
title: Ovládanie automatických aktualizácií aplikácií balíka Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439924"
---
# <a name="control-automatic-updates-for-office-apps"></a>Ovládanie automatických aktualizácií aplikácií balíka Office

V predvolenom nastavení sa aktualizácie aplikácií balíka Office preberajú automaticky a použijú na pozadí bez akéhokoľvek zásahu používateľa. Správcovia však môžu ovládať spôsob, akým sa používajú aktualizácie pomocou nastavenia služby Office Update. Nastavenia aktualizácie umožňujú správcom povoliť alebo zakázať automatické aktualizácie, zobraziť alebo skryť **tlačidlo Aktualizovať v** balíku Office, nastaviť termíny aktualizácií a ďalšie. Podrobné informácie nájdete v téme:

- [Konfigurácia nastavenia aktualizácie balíka Office](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [Automatické aktualizácie balíka Office nie je povolená](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [Definovanie spôsobu aktualizácie balíka Office po jeho nainštalovaní](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

Ak chcete skontrolovať existujúce nastavenia aktualizácií použité na klientskom počítači, postupujte nasledovne:

1. Otvorte Editor databázy Registry tým, že **pôjdete**  >  **na Štart Spustiť**  >  **regedit**.
2. Prepnite sa do nasledujúceho umiestnenia a skontrolujte nastavenia služby Office Update:  
    a. HKEY_LOCAL_MACHINE SOFTWARE\Microsoft\Office\  
    b. Kliknite na tlačidloToRun\Konfigurácia

**Upozornenie:**  Ak je nastavený kľúč OfficeMgmtCOM, môže sa zobraziť hlásenie "Aktualizácie spravuje správca systému" v **aktualizáciách balíka Office**  >  **Account**  >  **Account Office**. Ďalšie informácie nájdete v téme [Správa aktualizácií aplikácií Microsoft 365 pomocou programu Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).  
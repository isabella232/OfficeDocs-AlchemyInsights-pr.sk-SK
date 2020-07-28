---
title: Zmena aktualizačných kanálov pre aplikácie balíka Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440020"
---
# <a name="change-update-channels-for-office-apps"></a>Zmena aktualizačných kanálov pre aplikácie balíka Office

V prípade nových inštalácií balíka Office vyberte požadovaný kanál aktualizácie pomocou nastavení na prevzatie softvéru balíka Office a potom nainštalujte (alebo znova nainštalujte) aplikácie balíka Office. Ďalšie informácie nájdete v téme [Správa nastavení preberania softvéru v službách Office 365](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Upozornenie:** Kanál aktualizácie vybratý pomocou nastavenia na prevzatie softvéru balíka Office sa vzťahuje na všetkých používateľov vykonávajúcich nové inštalácie pomocou portálu O365. Ďalšie informácie nájdete v téme [Prevzatie a inštalácia alebo preinštalovanie Microsoft 365 alebo Office 2019 v PC alebo Macu](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Pre existujúce inštalácie balíka Office, použite Nástroj office Deployment Tool (ODT) prepnúť na iný kanál aktualizácie:  

1. Prevezmite najnovšiu verziu nástroja Office Deployment Tool (setup.exe) zo [Strediska pre prevzatie softvéru spoločnosti Microsoft](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Identifikujte názov kanála, na ktorý chcete prepnúť. Ďalšie informácie nájdete v téme [Možnosti konfigurácie nástroja na nasadenie balíka Office](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Vytvorte konfiguračný súbor XML určujúci príslušný názov kanála, napríklad update.xml.  
    a. <Configuration>  
    b. <aktualizácie **kanála ="Mesačne"** />  
    c. </Configuration>
4. Z príkazového riadka s právami správcu prepnite do umiestnenia priečinka, v ktorom setup.exe nachádza, a spustite nasledujúci príkaz:  
    a. setup.exe /configure update.xml
5. Spustite aplikáciu balíka Office (napríklad Excel) a potom vyberte **položku Konto**  >  **súboru**. V časti Informácie o produkte vyberte **položku Aktualizovať**  >  **možnosti aktualizácie**.

Ďalšie informácie nájdete v téme [Prepínanie kanálov aktualizácie pre existujúce aplikácie balíka Office](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Prepínanie aktualizačných kanálov pre vybratú skupinu používateľov alebo pomocou Configuration Manager (SCCM), nakonfigurujte nastavenie aktualizácie kanála pomocou objektu gpo. Ďalšie informácie nájdete v téme [Prehľad aktualizačných kanálov pre aplikácie Microsoft 365](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Podrobnosti nájdete v téme [Správa kanálov služieb Office 365 ProPlus pre profesionálov z oblasti IT](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) a správa [aktualizácií aplikácií Microsoft 365 pomocou programu Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).
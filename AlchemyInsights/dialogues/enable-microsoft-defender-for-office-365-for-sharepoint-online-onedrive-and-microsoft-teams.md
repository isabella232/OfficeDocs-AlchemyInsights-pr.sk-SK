---
title: Povolenie programu Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695653"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povolenie programu Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft teams

1. Pomocou poverení globálneho správcu alebo správcu zabezpečenia sa prihláste do [Centra zabezpečenia a dodržiavania súladu pre Office 365](https://protection.office.com/).
2. Na ľavej table vyberte položku **Správa hrozieb** a potom vyberte položku   >  [bezpečnostné prílohy](https://protection.office.com/safeattachment)politiky.
3. Vyberte položku **Zapnúť Microsoft Defender pre Office 365 pre SharePoint, OneDrive a Microsoft teams** a potom vyberte položku **Uložiť**.
    > [!TIP]
    >
    > - Ako globálny správca alebo správca SharePointu Online spustite nasledujúcu rutinu typu cmdlet prostredia PowerShell s parametrom **DisallowInfectedFileDownload** nastaveným na *hodnotu True*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Nastavenie upozornení na zistené súbory](https://go.microsoft.com/fwlink/?linkid=2092110)

Ďalšie informácie nájdete v téme [Microsoft Defender pre Office 365 pre SharePoint, OneDrive a Microsoft teams](https://go.microsoft.com/fwlink/?linkid=2092041).

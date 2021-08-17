---
title: Povoľte Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft Teams
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
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058881"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povoľte Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft Teams

1. Pomocou poverení globálneho správcu alebo správcu zabezpečenia sa prihláste do Centra [Office 365 zabezpečenia a dodržiavania súladu.](https://protection.office.com/)
2. Na **ľavej table** vyberte položku Spravovanie hrozieb a potom vyberte **položku**  >  [Trezor prílohy](https://protection.office.com/safeattachment).
3. Vyberte **položku Zapnúť Microsoft Defender pre Office 365 pre SharePoint, OneDrive a Microsoft Teams** a potom vyberte položku **Uložiť**.
    > [!TIP]
    >
    > - Ako globálny správca alebo správca služby SharePoint Online spustite nasledujúcu rutinu typu cmdlet prostredia PowerShell s **parametrom DisallowInfectedFileDownload** nastaveným na *hodnotu true:* [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Nastavenie upozornení pre zistené súbory](https://go.microsoft.com/fwlink/?linkid=2092110)

Ďalšie informácie nájdete v téme [Microsoft Defender pre Office 365 pre SharePoint, OneDrive a Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)

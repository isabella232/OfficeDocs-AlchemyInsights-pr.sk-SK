---
title: Povoliť Office 365 ATP pre SharePoint, OneDrive a Microsoft teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703441"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povoliť Office 365 pokročilé ohrozenia ochrany SharePoint Online, OneDrive a Microsoft teams

1. Prejdite na https://protection.office.com a prihláste sa.
2. Vyberte položku**politika** >  **správy** > hrozieb**bezpečné prílohy**.
3. Vyberte možnosť **Zapnúť ATP pre SharePoint, OneDrive a Microsoft teams**a potom kliknite na tlačidlo **Uložiť**.
4. Odporúča Ako globálny správca alebo SharePoint Online správca, spustite rutinu cmdlet [set-Sponájomcu](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **Disallowinfectedfiledownload** nastavená na *hodnotu True*.
5. Odporúča [Nastavte výstrahy pre rozpoznané](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) súbory.

> [!NOTE]
> ATP bude nAk chcete skenovať každý súbor v SharePointe Online, OneDrive alebo Microsoft teams. Súbory sa skenujú asynchrónne, a to prostredníctvom procesu, ktorý používa akcie zdieľania a hosťovskej aktivity spolu s inteligentnými heuristami a signálmi hrozieb na identifikáciu škodlivých súborov. Vidieť [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
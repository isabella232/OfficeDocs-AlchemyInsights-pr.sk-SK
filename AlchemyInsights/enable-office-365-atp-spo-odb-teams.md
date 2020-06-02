---
title: Povolenie protokolu ATP služieb Office 365 pre SharePoint, OneDrive a Microsoft Teams
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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506933"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povolenie rozšírenej ochrany pred hrozbami služieb Office 365 pre SharePoint Online, OneDrive a Microsoft Teams

1. Choď te https://protection.office.com do a prihláste sa.
2. Vyberte položku **Threat management**Policy Safe Attachments (Bezpečné prílohy politiky správy  >  **Policy**  >  **hrozieb).**
3. Vyberte položku **Zapnúť atp pre SharePoint, OneDrive a Microsoft Teams a**potom kliknite na tlačidlo **Uložiť**.
4. (Odporúča sa) Ako globálny správca alebo správca SharePointu Online spustite rutinu cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** nastaveným na *hodnotu true*.
5. (Odporúča sa) [Nastavte upozornenia](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) na zistené súbory.

> [!NOTE]
> ATP bude skenovať každý jeden súbor v SharePointE Online, OneDrive alebo Microsoft Teams. Súbory sa kontrolujú asynchrónne prostredníctvom procesu, ktorý používa udalosti zdieľania a aktivity hostí spolu s inteligentnou heuristikou a signálmi hrozieb na identifikáciu škodlivých súborov. Pozrite [si tému ATP pre SharePoint, OneDrive a Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
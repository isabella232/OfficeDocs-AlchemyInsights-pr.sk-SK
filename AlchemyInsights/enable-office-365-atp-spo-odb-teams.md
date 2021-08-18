---
title: Povoľte Office 365 ATP pre SharePoint, OneDrive a Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332174"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povoľte Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft Teams

1. Prejdite na https://protection.office.com položku a prihláste sa.
2. Vyberte **položku Politika správy**  >  **hrozieb** Trezor  >  **prílohy**.
3. Vyberte **položku Zapnúť Defender pre Office 365 pre SharePoint, OneDrive a Microsoft Teams** a potom kliknite na položku **Uložiť**.
4. (Odporúča sa) Ako globálny správca alebo správca služby SharePoint Online spustite rutinu typu cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s **parametrom DisallowInfectedFileDownload** nastaveným na *hodnotu true.*
5. (Odporúča sa) [Nastavenie upozornení pre](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) zistené súbory.

**Poznámka:** Microsoft Defender pre Office 365 nebude skenovať každý jeden súbor vo SharePoint Online, OneDrive alebo Microsoft Teams. Súbory sa naskenujú asynchrónne, a to procesom, ktorý využíva udalosti zdieľania a aktivity hostí, ako aj inteligentné heuštie a signály hrozieb na identifikáciu škodlivých súborov. Pozrite si Office 365 Microsoft [Defender pre SharePoint, OneDrive a Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).

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
ms.openlocfilehash: 4a29fdf1b61dd51b85793a1346bea193c67f70d32344470cb5449cf767da4a24
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896618"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povoľte Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft Teams

1. Prejdite na https://protection.office.com položku a prihláste sa.
2. Vyberte **položku Politika správy**  >  **hrozieb** Trezor  >  **prílohy**.
3. Vyberte **položku Zapnúť Defender for Office 365 pre SharePoint, OneDrive a Microsoft Teams** a potom kliknite na položku **Uložiť**.
4. (Odporúča sa) Ako globálny správca alebo správca služby SharePoint Online spustite rutinu typu cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** nastaveným na *hodnotu true.*
5. (Odporúča sa) [Nastavenie upozornení pre](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) zistené súbory.

> [!NOTE]
> Microsoft Defender pre Office 365 nebude kontrolovať každý súbor vo SharePoint Online, OneDrive alebo Microsoft Teams. Súbory sa naskenujú asynchrónne, a to procesom, ktorý využíva udalosti zdieľania a aktivity hostí, ako aj inteligentné heuštie a signály hrozieb na identifikáciu škodlivých súborov. Pozrite [si téme Microsoft Defender Office 365 pre SharePoint, OneDrive a Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
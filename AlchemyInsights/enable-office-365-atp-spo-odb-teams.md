---
title: Povoliť Office 365 ATP pre SharePoint a OneDrive Microsoft tímy
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403048"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Zapnutie ochrany Office 365 pokročilé hrozby pre SharePoint Online, OneDrive a Microsoft tímy

1. Prejsť na https://protection.office.com a prihláste sa.
2. Vybrať **Threat management** > **politika** > **Bezpečnými prílohami**.
3. Vyberte **Zapnúť ATP pre SharePoint, OneDrive, a tímy spoločnosti Microsoft**a potom kliknite na tlačidlo **Uložiť**.
4. (Odporúča sa) Ako globálny správca alebo správca SharePoint Online, spustite rutinu cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s **DisallowInfectedFileDownload** parameter nastavený na *hodnotu true*.
5. (Odporúča sa) [Nastaviť upozornenia](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) pre rozpoznaných súborov.

> [!NOTE]
> ATP sa nto scan každý súbor SharePoint Online, OneDrive alebo Microsoft Teams. Súbory sú kontrolované asynchrónne, cez proces, ktorý využíva zdieľanie a hodnotenie činnosti udalosti, spolu s smart heuristiky a hrozba signály na identifikáciu škodlivého súborov. Pozrite si [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
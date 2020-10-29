---
title: Povolenie služieb Office 365 ATP pre SharePoint, OneDrive a Microsoft teams
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801090"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Povolenie programu Microsoft Defender pre Office 365 pre SharePoint Online, OneDrive a Microsoft teams

1. Prejdite na https://protection.office.com a prihláste sa.
2. Vyberte **Threat management**  >  **Policy**  >  **bezpečné prílohy** politiky správy hrozieb.
3. Vyberte položku **Zapnúť ATP pre SharePoint, OneDrive a Microsoft teams** a potom kliknite na tlačidlo **Uložiť** .
4. Odporúča Ako globálny správca alebo správca SharePointu Online spustite rutinu typu cmdlet [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) s parametrom **DisallowInfectedFileDownload** nastavený na *hodnotu True* .
5. Odporúča [Nastavte upozornenia](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) na zistené súbory.

> [!NOTE]
> ATP bude NAK kontrolovať každý jeden súbor v SharePointe Online, vo OneDrive alebo v aplikácii Microsoft teams. Súbory sa naskenujú asynchrónne, a to prostredníctvom procesu, ktorý používa akcie zdieľania a aktivity hosťujúcich, spolu s inteligentnou heuristikou a signálmi hrozby na identifikáciu škodlivých súborov. Pozrite si tému [ATP pre SharePoint, OneDrive a Microsoft teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).
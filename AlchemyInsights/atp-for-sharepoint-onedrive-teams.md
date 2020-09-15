---
title: ATP pre SharePoint, OneDrive a Microsoft teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715576"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP pre SharePoint, OneDrive a Microsoft teams

Ak chcete povoliť rozšírenú ochranu pred hrozbami, postupujte podľa týchto krokov:

1. Prejdite na [https://protection.office.com](https://protection.office.com) globálneho správcu alebo konto správcu zabezpečenia a prihláste sa.

2. Na ľavej navigačnej table v časti **Správa hrozieb**vyberte položku **Policy** \> **bezpečnostné prílohy**politiky.

3. Vyberte položku **Zapnúť ATP pre SharePoint, OneDrive a Microsoft teams**.

4. Pri zisťovaní škodlivých súborov [vytvorte politiku upozornenia o aktivite](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) na prijímanie oznámení.

Podrobné pokyny nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).

**Poznámka**: zámerom je, že ATP neskenuje každý jeden súbor v SharePointe Online, OneDrive for Business alebo v aplikácii Microsoft teams. Súbory sa kontrolujú asynchrónne procesom, ktorý používa aktivitu zdieľania, aktivitu hostí a signály hrozby na identifikáciu škodlivých súborov. Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).

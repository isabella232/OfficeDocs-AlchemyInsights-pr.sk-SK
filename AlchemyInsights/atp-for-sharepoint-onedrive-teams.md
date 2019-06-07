---
title: ATP pre SharePoint a OneDrive Microsoft tímy
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765388"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP pre SharePoint a OneDrive Microsoft tímy

Postupujte nasledovne umožniť rozšírenú ochranu:

1. Prejsť na [https://protection.office.com](https://protection.office.com) a prihláste sa pomocou globálny správca alebo správca konto zabezpečenia.

2. Na ľavej navigačnej table pod **Threat management**vyberte **politika** \> **Bezpečnými prílohami**.

3. Vyberte **Zapnúť ATP pre SharePoint, OneDrive, a tímy Microsoft**.

4. [Vytvorenie aktivity alert politiky](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) dostávať upozornenia, keď sme odhaliť škodlivé súbory.

Kompletné pokyny nájdete v časti tejto [témy](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).

**Poznámka**: predvolene ATP neprehľadáva každý súbor v službe SharePoint Online, OneDrive for Business alebo Microsoft Teams. Súbory sú načítané asynchrónne proces, ktorý využíva zdieľanie činností, hodnotenie a hrozba signály na identifikáciu škodlivého súborov. Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).

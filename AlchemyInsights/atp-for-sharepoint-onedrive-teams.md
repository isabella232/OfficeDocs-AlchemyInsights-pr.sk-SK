---
title: ATP pre SharePoint, OneDrive a Microsoft teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712473"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a>ATP pre SharePoint, OneDrive a Microsoft teams

Ak chcete povoliť rozšírenú ochranu pred hrozbami, postupujte podľa týchto krokov:

1. Prejdite na [https://protection.office.com](https://protection.office.com) a prihláste sa pomocou globálneho správcu alebo konta správcu zabezpečenia.

2. Na ľavej navigačnej table v časti **Správa hrozieb**vyberte položku **Policy** \> **bezpečné prílohy**politiky.

3. Vyberte možnosť **Zapnúť ATP pre SharePoint, OneDrive a Microsoft teams**.

4. [Vytvorenie politiky výstrahy aktivity](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) na prijímanie upozornení pri detekcii škodlivých súborov.

Úplné pokyny nájdete v tejto [téme](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).

**Poznámka**: podľa návrhu, ATP neskenuje každý jednotlivý súbor SharePoint Online, OneDrive pre podniky alebo Microsoft teams. Súbory sú naskenované asynchrónne procesom, ktorý používa zdieľanie aktivity, hodnotenie aktivity a hrozby signály identifikovať škodlivé súbory. Ďalšie informácie nájdete v tejto [téme](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).

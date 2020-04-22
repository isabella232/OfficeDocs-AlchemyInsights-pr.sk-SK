---
title: Klasické zostavy denníka auditu služby SharePoint
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741980"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Denníky auditu služby SharePoint a OneDrive

## <a name="sharepoint-classic-audit-logs"></a>Denníky auditu služby SharePoint Classic

Auditovanie SPO Legacy bolo presunuté do zjednoteného denníka auditu (UAL). Všetky SPO staršie audítorské správy budú teraz napájané prostredníctvom UAL a staršie audítorské signály boli migrované na UAL.

Kľúčové zmeny:

* Orezávanie nie je k dispozícii ako schopnosť.
* Výber konkrétnych udalostí na audit nie je k dispozícii. Úplný zoznam auditovaných udalostí, ktoré sú predvolene k dispozícii, nájdete [v tomto dokumente](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) .
* Možnosť **umiestnenie** v časti **prispôsobené prehľady** nie je k dispozícii.
* Možnosť **otváranie alebo preberanie dokumentov** nie je k dispozícii.

[Konfigurácia nastavení auditovania pre kolekciu lokalít](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint a OneDrive moderné Unified audit denníky z súladu

* [Zapnutie/vypnutie zapisovania do denníka zjednoteného auditu](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

V SharePointe alebo OneDrive sa nevyžaduje žiadna dodatočná konfigurácia.

Použite auditovanie zapisovania do denníka na kontrolu aktivity súborov, priečinkov, používateľov, povolení:

* [Aktivity súborov a strán](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [Aktivity priečinkov](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktivity zdieľania a prístupu k žiadosti o prístup](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synchronizačné aktivity](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Činnosti správy lokality](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Ďalšie informácie o možnostiach získania týchto udalostí nájdete [v téme Vyhľadávanie v denníku auditu](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

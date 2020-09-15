---
title: Klasické zostavy denníkov auditu SharePointu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662223"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>Denníky auditu SharePointu a OneDrivu

## <a name="sharepoint-classic-audit-logs"></a>Klasické denníky auditu SharePointu

Audity SPO Legacy sa sťahovali do jednotného denníka auditu (UAL). Všetky staršie správy o audite SPO budú teraz poháňané prostredníctvom funkcie UAL a staršie audítorské signály sa migrujú do funkcie UAL.

Kľúčové zmeny:

* Orezávanie nie je k dispozícii ako možnosť.
* Výber konkrétnych udalostí na audit nie je k dispozícii. Ak chcete zobraziť celý zoznam auditovaných udalostí, ktoré sú k dispozícii na základe predvoleného nastavenia, pozrite si [Tento dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) .
* Možnosť **umiestnenie** v časti **prispôsobené zostavy** nie je k dispozícii.
* Možnosť **Otvoriť alebo stiahnuť dokumenty** nie je k dispozícii.

[Konfigurácia nastavenia auditu pre kolekciu lokalít](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Moderné zjednotené denníky auditu SharePointu a OneDrivu z dodržiavania súladu

* [Zapnutie a vypnutie zjednoteného zapisovania do denníka auditu](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

V rámci SharePointu alebo OneDrivu sa nevyžaduje žiadna ďalšia konfigurácia.

Použite vyhľadávanie zapisovanie do denníka auditu na kontrolu aktivity súborov, priečinkov, používateľov, povolení:

* [Aktivity týkajúce sa súborov a stránok](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Aktivity priečinka](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Aktivity týkajúce sa zdieľania a žiadosti o prístup](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Aktivity synchronizácie](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Aktivity týkajúce sa správy lokality](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Ďalšie informácie o tom, ako získať tieto udalosti, nájdete [v téme Vyhľadávanie v denníku auditu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).

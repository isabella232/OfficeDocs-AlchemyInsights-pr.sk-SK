---
title: Microsoft Edge nastavenia ochrany osobných údajov
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114187"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge nastavenia ochrany osobných údajov

Ak je služba Microsoft Edge nasadená na platformách iných ako Windows, diagnostické údaje a informácie o lokalite sa spoločnosti Microsoft odosielajú. Ak je však Microsoft Edge nasadené na lokalite Windows 10, diagnostické údaje a informácie o lokalite sa odosielajú podľa nastavení [diagnostických Windows používateľov.](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)

Ak chcete konfigurovať Microsoft Edge spracovanie zhromažďovania údajov pre vašu organizáciu, použite tieto skupinové politiky:
- [MetricsReportingEnabled:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)Táto politika umožňuje vykazovanie údajov o používaní a údajoch súvisiacich s zlyhaním.
- [SendSiteInfoToImproveServices:](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)Táto politika odosiela informácie o lokalite, ktoré sa používajú na služby Microsoft.

Ďalšie informácie nájdete v téme [Konfigurácia nastavenia politiky.](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)
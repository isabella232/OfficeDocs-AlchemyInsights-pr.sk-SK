---
title: Konfigurácia nastavenia ochrany osobných údajov v prehliadači Microsoft Edge
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
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678859"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Konfigurácia nastavenia ochrany osobných údajov v prehliadači Microsoft Edge

Ak je Microsoft Edge nasadený na platformách iných ako Windows, diagnostické údaje a informácie o lokalite sa na základe predvoleného nastavenia neodosielajú spoločnosti Microsoft. Ak je však Microsoft Edge nasadený vo Windowse 10, diagnostické údaje a informácie o lokalite sa odosielajú v závislosti od [nastavení diagnostických údajov používateľov systému Windows](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization).

Ak chcete nakonfigurovať spôsob, akým Microsoft Edge spracuje zhromažďovanie údajov pre vašu organizáciu, použite tieto skupinové politiky:
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled): Táto politika umožňuje vytváranie hlásení o používaní a údajoch súvisiacich s haváriami.
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices): Táto politika odošle informácie o lokalite, ktoré sa používajú na zlepšenie služieb spoločnosti Microsoft.

Ďalšie informácie nájdete v téme [Konfigurácia nastavenia politiky](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings).
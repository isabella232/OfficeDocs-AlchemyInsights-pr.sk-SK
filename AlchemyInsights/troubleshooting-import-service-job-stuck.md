---
title: Riešenie problémov s úlohami služby Import Service sú zaseknuté
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/27/2021
ms.locfileid: "52125493"
---
# <a name="troubleshooting-import-service-job-stuck"></a>Riešenie problémov s úlohami služby Import Service sú zaseknuté

Ak sa vyskytnú problémy s uviaznutým alebo zlyhávaním úloh služby Import, preskúmajte a vyskúšajte tento postup:

- Skontrolujte veľkosť súboru PST. Maximálna odporúčaná veľkosť súboru PST na import je 20 GB.

- Ak máte podozrenie, že ste vynechali položky z dôvodu poškodenia, spustite Scanpst.exe a opravte chyby v súboroch PST.

- Ak sa počas importu zobrazí chyba MapiExceptionShutoffQuotaExceeded, skontrolujte, či cieľová poštová schránka má dostatočnú kapacitu na importovanie požadovaných súborov PST.

Ďalšie informácie o riešení problémov s úlohami importu PST nájdete v téme [Riešenie problémov s úlohami importu PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)

Informácie o riešení problémov pri importovaní súborov PST do služieb Outlook nájdete v téme Riešenie problémov s importom súboru [.Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).
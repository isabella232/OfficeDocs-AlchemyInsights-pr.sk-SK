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
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="2c3dc-102">Riešenie problémov s úlohami služby Import Service sú zaseknuté</span><span class="sxs-lookup"><span data-stu-id="2c3dc-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="2c3dc-103">Ak sa vyskytnú problémy s uviaznutým alebo zlyhávaním úloh služby Import, preskúmajte a vyskúšajte tento postup:</span><span class="sxs-lookup"><span data-stu-id="2c3dc-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="2c3dc-104">Skontrolujte veľkosť súboru PST.</span><span class="sxs-lookup"><span data-stu-id="2c3dc-104">Review the size of of the PST file.</span></span> <span data-ttu-id="2c3dc-105">Maximálna odporúčaná veľkosť súboru PST na import je 20 GB.</span><span class="sxs-lookup"><span data-stu-id="2c3dc-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="2c3dc-106">Ak máte podozrenie, že ste vynechali položky z dôvodu poškodenia, spustite Scanpst.exe a opravte chyby v súboroch PST.</span><span class="sxs-lookup"><span data-stu-id="2c3dc-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="2c3dc-107">Ak sa počas importu zobrazí chyba MapiExceptionShutoffQuotaExceeded, skontrolujte, či cieľová poštová schránka má dostatočnú kapacitu na importovanie požadovaných súborov PST.</span><span class="sxs-lookup"><span data-stu-id="2c3dc-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="2c3dc-108">Ďalšie informácie o riešení problémov s úlohami importu PST nájdete v téme [Riešenie problémov s úlohami importu PST.](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job)</span><span class="sxs-lookup"><span data-stu-id="2c3dc-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="2c3dc-109">Informácie o riešení problémov pri importovaní súborov PST do služieb Outlook nájdete v téme Riešenie problémov s importom súboru [.Outlook (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="2c3dc-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>
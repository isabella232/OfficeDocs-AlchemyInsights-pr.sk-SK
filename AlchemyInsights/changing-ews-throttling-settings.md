---
title: Zmena nastavení obmedzovania EWS
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818051"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="bc11f-102">Zmena nastavení obmedzovania EWS</span><span class="sxs-lookup"><span data-stu-id="bc11f-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="bc11f-103">Spustite náš automatický test, ktorý vám umožní upraviť politiku obmedzovania EWS počas trvania migrácie.</span><span class="sxs-lookup"><span data-stu-id="bc11f-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="bc11f-104">Všimnite si, že aj po spustení bude import EWS obmedzený na 150 MB na 5 minút na poštovú schránku. Ak chcete dosiahnuť vyššiu priepustnosť migrácie, migrujte viacerých používateľov súčasne.</span><span class="sxs-lookup"><span data-stu-id="bc11f-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="bc11f-105">Zmeny politiky obmedzovania EWS nemajú žiadny vplyv na nasledujúce typy migrácie (pomocou nástrojov od spoločnosti Microsoft): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Verejný priečinok alebo PST Import Service.</span><span class="sxs-lookup"><span data-stu-id="bc11f-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>
---
title: Zmena nastavení obmedzovania EWS
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075912"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="d7f8d-102">Zmena nastavení obmedzovania EWS</span><span class="sxs-lookup"><span data-stu-id="d7f8d-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="d7f8d-103">Spustite náš automatický test, ktorý vám umožní upraviť politiku obmedzovania EWS počas trvania migrácie.</span><span class="sxs-lookup"><span data-stu-id="d7f8d-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="d7f8d-104">Všimnite si, že aj po spustení bude import EWS obmedzený na 150 MB na 5 minút na poštovú schránku. Ak chcete dosiahnuť vyššiu priepustnosť migrácie, migrujte viacerých používateľov súčasne.</span><span class="sxs-lookup"><span data-stu-id="d7f8d-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="d7f8d-105">Zmeny politiky obmedzovania EWS nemajú žiadny vplyv na nasledujúce typy migrácie (pomocou nástrojov od spoločnosti Microsoft): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Verejný priečinok alebo PST Import Service.</span><span class="sxs-lookup"><span data-stu-id="d7f8d-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>
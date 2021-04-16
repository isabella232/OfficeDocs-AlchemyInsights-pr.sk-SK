---
title: Samoobslužný nákup prostredia PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797736"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="3cdb0-102">Samoobslužný nákup prostredia PowerShell</span><span class="sxs-lookup"><span data-stu-id="3cdb0-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="3cdb0-103">Ak chcete používať modul MSCommerce PowerShell, musíte ho nainštalovať do zariadenia s Windowsom 10 s TLS 1.2 (vyžadujú sa povolenia lokálneho správcu).</span><span class="sxs-lookup"><span data-stu-id="3cdb0-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="3cdb0-104">Importujte modul MSCommerce a pripojte sa k jeho modulu.</span><span class="sxs-lookup"><span data-stu-id="3cdb0-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="3cdb0-105">Po zobrazení výzvy na prihlásenie je potrebné použiť poverenia roly globálneho správcu alebo správcu fakturácie.</span><span class="sxs-lookup"><span data-stu-id="3cdb0-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="3cdb0-106">Ak nemáte protokol TLS 1.2, pri pokuse o získanie alebo aktualizáciu politiky sa môže zobraziť nasledujúca chyba:</span><span class="sxs-lookup"><span data-stu-id="3cdb0-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="3cdb0-107">*ErrorMessage -Základné pripojenie sa zavrelo: Pri odosielaní sa vyskytla neočakávaná chyba.*</span><span class="sxs-lookup"><span data-stu-id="3cdb0-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>




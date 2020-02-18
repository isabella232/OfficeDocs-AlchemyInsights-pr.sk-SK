---
title: Samoobslužný nákup PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091761"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="4a8e9-102">Samoobslužný nákup PowerShell</span><span class="sxs-lookup"><span data-stu-id="4a8e9-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="4a8e9-103">Ak chcete použiť modul MSCommerce PowerShell, musíte ho nainštalovať na zariadení s Windowsom 10 s TLS 1,2 (vyžaduje sa povolenie lokálneho správcu).</span><span class="sxs-lookup"><span data-stu-id="4a8e9-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="4a8e9-104">Importovanie a pripojenie k modulu MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="4a8e9-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="4a8e9-105">Keď sa zobrazí výzva na prihlásenie, budete musieť použiť poverenia globálnej alebo fakturačnej roly správcu.</span><span class="sxs-lookup"><span data-stu-id="4a8e9-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="4a8e9-106">Ak nemáte TLS 1,2, môže sa zobraziť nasledujúca chyba pri pokuse o získanie alebo aktualizáciu politiky:</span><span class="sxs-lookup"><span data-stu-id="4a8e9-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="4a8e9-107">*Errormessage-základné pripojenie bolo zatvorené: Vyskytla sa neočakávaná chyba pri odosielaní*.</span><span class="sxs-lookup"><span data-stu-id="4a8e9-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>




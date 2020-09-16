---
title: Samoobslužné zakúpenie prostredia PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739985"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="0c524-102">Samoobslužné zakúpenie prostredia PowerShell</span><span class="sxs-lookup"><span data-stu-id="0c524-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="0c524-103">Ak chcete použiť modul MSCommerce PowerShell, musíte ho nainštalovať do zariadenia s Windowsom 10 pomocou TLS 1,2 (vyžaduje sa povolenie lokálneho správcu).</span><span class="sxs-lookup"><span data-stu-id="0c524-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="0c524-104">Importujte a pripojte sa k modulu MSCommerce.</span><span class="sxs-lookup"><span data-stu-id="0c524-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="0c524-105">Keď sa zobrazí výzva na prihlásenie, budete musieť použiť poverenia roly správcu globálnych alebo fakturačných správ.</span><span class="sxs-lookup"><span data-stu-id="0c524-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="0c524-106">Ak nemáte TLS 1,2, pri pokuse o získanie alebo aktualizáciu politiky sa môže zobraziť Táto chyba:</span><span class="sxs-lookup"><span data-stu-id="0c524-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="0c524-107">*Errormessage – základné pripojenie bolo zatvorené: na odoslanie sa vyskytla neočakávaná chyba*.</span><span class="sxs-lookup"><span data-stu-id="0c524-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>




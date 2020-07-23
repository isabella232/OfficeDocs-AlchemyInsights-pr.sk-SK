---
title: Riešenie problémov so synchronizáciou hesiel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387892"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="891eb-102">Riešenie problémov so synchronizáciou hesiel</span><span class="sxs-lookup"><span data-stu-id="891eb-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="891eb-103">Ak chcete riešiť problémy so synchronizáciou hesiel, začnite pomocou tejto úlohy riešenia problémov AAD Connect a zistite, prečo sa heslá nesynchronizujú.</span><span class="sxs-lookup"><span data-stu-id="891eb-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="891eb-104">Ak chcete začať, prejdite na [Spravovať priamu synchronizáciu](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="891eb-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="891eb-105">Otvorte novú reláciu prostredia Windows PowerShell na serveri Azure AD pripojiť a vyberte **možnosť Spustiť ako** správca .</span><span class="sxs-lookup"><span data-stu-id="891eb-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="891eb-106">Spustiť Set-ExecutionPolicy RemoteSigned alebo Set-ExecutionPolicy Neobmedzený.</span><span class="sxs-lookup"><span data-stu-id="891eb-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="891eb-107">Spustite Sprievodcu pripojením Azure AD.</span><span class="sxs-lookup"><span data-stu-id="891eb-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="891eb-108">Prejdite na stránku Ďalšie úlohy a > riešenie **problémov s ďalším**  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="891eb-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="891eb-109">Výberom položky **Launch** (Spustiť) otvorte ponuku na riešenie problémov v prostredí PowerShell.</span><span class="sxs-lookup"><span data-stu-id="891eb-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="891eb-110">Vyberte **položku Riešenie problémov so synchronizáciou hesiel**.</span><span class="sxs-lookup"><span data-stu-id="891eb-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="891eb-111">Problém je zvyčajne, že heslo nie je synchronizovaný pre konkrétne používateľské konto.</span><span class="sxs-lookup"><span data-stu-id="891eb-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="891eb-112">**Poznámky k používaniu** Synchronizácia hesiel zlyhá, ak bola posledná úspešná synchronizácia hesla pred nejakým časom.</span><span class="sxs-lookup"><span data-stu-id="891eb-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="891eb-113">Ďalšie informácie o riešení problémov so synchronizáciou hesiel nájdete v [téme Riešenie problémov so synchronizáciou hash hesla pomocou synchronizácie služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="891eb-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>
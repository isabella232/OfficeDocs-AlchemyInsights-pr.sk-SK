---
title: Riešenie problémov so synchronizáciou hesiel
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664941"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="d1891-102">Riešenie problémov so synchronizáciou hesiel</span><span class="sxs-lookup"><span data-stu-id="d1891-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="d1891-103">Ak chcete riešiť problémy so synchronizáciou hesiel, začnite pomocou tohto nástroja AAD pripojiť riešenie problémov a zistite, prečo sa heslá nesynchronizujú.</span><span class="sxs-lookup"><span data-stu-id="d1891-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="d1891-104">Ak chcete začať, prejdite na položku [Správa priamej synchronizácie](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="d1891-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="d1891-105">Otvorte novú reláciu prostredia Windows PowerShell na serveri Azure AD Connect a vyberte možnosť **Spustiť ako správca** .</span><span class="sxs-lookup"><span data-stu-id="d1891-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="d1891-106">Spustite set-ExecutionPolicy RemoteSigned alebo set-ExecutionPolicy neobmedzený.</span><span class="sxs-lookup"><span data-stu-id="d1891-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="d1891-107">Spustite Sprievodcu Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d1891-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="d1891-108">Prejdite na stránku ďalšie úlohy > **Riešenie problémov s**  >  **ďalšou**.</span><span class="sxs-lookup"><span data-stu-id="d1891-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="d1891-109">Ak chcete otvoriť ponuku riešenie problémov v prostredí PowerShell, vyberte položku **Spustiť** .</span><span class="sxs-lookup"><span data-stu-id="d1891-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="d1891-110">Vyberte položku **Riešenie problémov so synchronizáciou hesiel**.</span><span class="sxs-lookup"><span data-stu-id="d1891-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="d1891-111">Problém je zvyčajne to, že heslo nie je synchronizované pre konkrétne používateľské konto.</span><span class="sxs-lookup"><span data-stu-id="d1891-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="d1891-112">**Poznámky** Synchronizácia hesiel zlyhá, ak bola Posledná úspešná synchronizácia hesiel pred nejakým časom.</span><span class="sxs-lookup"><span data-stu-id="d1891-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="d1891-113">Ďalšie informácie o riešení problémov so synchronizáciou hesiel nájdete v téme [Riešenie problémov so synchronizáciou hash hesla pomocou synchronizácie služby Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d1891-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>
---
title: Synchronizácia služby Active Directory
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
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697644"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="8cc59-102">Synchronizácia služby Active Directory</span><span class="sxs-lookup"><span data-stu-id="8cc59-102">Active Directory not syncing</span></span>

<span data-ttu-id="8cc59-103">Ak dostávate chyby synchronizácie, ako napríklad "bez poslednej synchronizácie", alebo si všimnete stav synchronizácie adresárov na portáli pre správcov balíka Office, v časti naposledy synchronizované pred viac ako 3 dňami sa môže stať, že AADConnect má nesprávne nastavenie alebo nedostatočné povolenia na vykonanie synchronizácie.</span><span class="sxs-lookup"><span data-stu-id="8cc59-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="8cc59-104">Opätovná inštalácia AADConnect pomocou expresných nastavení môže problém vyriešiť rýchlo:</span><span class="sxs-lookup"><span data-stu-id="8cc59-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="8cc59-105">[Stiahnite si najnovšiu verziu balíka AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="8cc59-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="8cc59-106">[Postupujte podľa pokynov na expresné inštaláciu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="8cc59-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="8cc59-107">Ďalšie informácie o kontách služby AADConnect nájdete v téme [Azure AD Connect: kontá a povolenia](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="8cc59-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>

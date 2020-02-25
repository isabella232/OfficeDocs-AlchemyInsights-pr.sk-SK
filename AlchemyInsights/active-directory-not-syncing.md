---
title: Služba Active Directory sa nesynchronizuje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 02/25/2020
ms.locfileid: "42265271"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="efdc9-102">Služba Active Directory sa nesynchronizuje</span><span class="sxs-lookup"><span data-stu-id="efdc9-102">Active Directory not syncing</span></span>

<span data-ttu-id="efdc9-103">Ak dostávate chyby synchronizácie, napríklad "žiadna Nedávna synchronizácia" alebo oznámenie stav synchronizácie adresárov na portáli Office Admin hovorí: "naposledy synchronizované viac ako 3 dni," môže byť, že AADConnect má nesprávne nastavenia alebo nedostatočné povolenia na vykonanie synchronizácie.</span><span class="sxs-lookup"><span data-stu-id="efdc9-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="efdc9-104">Preinštalovanie AADConnect pomocou expresné nastavenie môže vyriešiť problém rýchlo:</span><span class="sxs-lookup"><span data-stu-id="efdc9-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="efdc9-105">[Prevezmite si najnovšiu verziu AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="efdc9-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="efdc9-106">[Postupujte podľa pokynov na expresnú inštaláciu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="efdc9-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="efdc9-107">Ďalšie informácie o kontách služby AADConnect nájdete v téme [Azure AD Connect: kontá a povolenia](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="efdc9-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>

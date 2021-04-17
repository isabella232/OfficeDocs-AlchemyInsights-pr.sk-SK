---
title: Nesynchronizuje sa Active Directory
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
- "9001688"
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822866"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="9f7cd-102">Nesynchronizuje sa Active Directory</span><span class="sxs-lookup"><span data-stu-id="9f7cd-102">Active Directory not syncing</span></span>

<span data-ttu-id="9f7cd-103">Ak sa vám zobrazuje chyba synchronizácie, napríklad "žiadna nedávna synchronizácia" alebo ak si všimnete stav synchronizácie adresárov na portáli pre správcov balíka Office, zobrazí sa hlásenie Posledná synchronizácia pred viac ako 3 dňami, môže to byť preto, že AADConnect má na vykonanie synchronizácie nesprávne nastavenia alebo nedostatočné povolenia.</span><span class="sxs-lookup"><span data-stu-id="9f7cd-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="9f7cd-104">Preinštalovanie služby AADConnect pomocou expresných nastavení môže problém rýchlo vyriešiť:</span><span class="sxs-lookup"><span data-stu-id="9f7cd-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="9f7cd-105">[Stiahnite si najnovšiu verziu aplikácie AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="9f7cd-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="9f7cd-106">[Postupujte podľa pokynov pre expresnú inštaláciu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="9f7cd-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="9f7cd-107">Ďalšie informácie o kontách služby AADConnect nájdete v téme [Azure AD Connect: kontá a povolenia.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="9f7cd-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>

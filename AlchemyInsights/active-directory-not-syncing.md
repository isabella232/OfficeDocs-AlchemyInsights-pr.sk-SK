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
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: sk-SK
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930990"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="09b71-102">Nesynchronizuje sa Active Directory</span><span class="sxs-lookup"><span data-stu-id="09b71-102">Active Directory not syncing</span></span>

<span data-ttu-id="09b71-103">Ak sa vám zobrazuje chyba synchronizácie, napríklad "žiadna nedávna synchronizácia" alebo ak si všimnete stav synchronizácie adresárov na portáli pre správcov služieb Office zobrazí hlásenie Posledná synchronizácia pred viac ako 3 dňami, môže to byť preto, že AADConnect má nesprávne nastavenia alebo nedostatočné povolenia na vykonanie synchronizácie.</span><span class="sxs-lookup"><span data-stu-id="09b71-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="09b71-104">Preinštalovanie služby AADConnect pomocou expresných nastavení môže tento problém rýchlo vyriešiť:</span><span class="sxs-lookup"><span data-stu-id="09b71-104">Reinstalling AADConnect by using express settings might resolve the issue quickly:</span></span>

1. <span data-ttu-id="09b71-105">[Stiahnite si najnovšiu verziu aplikácie AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)</span><span class="sxs-lookup"><span data-stu-id="09b71-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="09b71-106">[Postupujte podľa pokynov pre expresnú inštaláciu.](/azure/active-directory/hybrid/how-to-connect-install-express)</span><span class="sxs-lookup"><span data-stu-id="09b71-106">[Follow the instructions for express installation](/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="09b71-107">Nástroj Azure AD Connect musí byť nainštalovaný v systéme Windows Server 2012 alebo novšom.</span><span class="sxs-lookup"><span data-stu-id="09b71-107">Azure AD Connect must be installed on Windows Server 2012 or later.</span></span> <span data-ttu-id="09b71-108">Tento server musí byť pripojený k doméne a môže to byť radič domény alebo členský server.</span><span class="sxs-lookup"><span data-stu-id="09b71-108">This server must be domain joined and may be a domain controller or a member server.</span></span> <span data-ttu-id="09b71-109">Úplný zoznam požiadaviek a predpokladov služby Azure AD Pripojenie AD nájdete v článku [Predpoklady pre Azure AD Pripojenie.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)</span><span class="sxs-lookup"><span data-stu-id="09b71-109">For a full list of Azure AD Connect requirements and pre-requisites, review [Prerequisites for Azure AD Connect](/azure/active-directory/hybrid/how-to-connect-install-prerequisites).</span></span>

<span data-ttu-id="09b71-110">Ďalšie informácie o kontách služby AADConnect nájdete v téme [Azure AD Pripojenie: Kontá a povolenia.](/azure/active-directory/hybrid/reference-connect-accounts-permissions)</span><span class="sxs-lookup"><span data-stu-id="09b71-110">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
